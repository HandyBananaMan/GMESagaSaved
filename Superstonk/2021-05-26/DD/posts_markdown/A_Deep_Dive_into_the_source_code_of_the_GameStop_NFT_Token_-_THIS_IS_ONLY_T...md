# Author: bigmike02
# Post URL: [https://www.reddit.com/r/Superstonk/comments/nlh60l/a_deep_dive_into_the_source_code_of_the_gamestop/](https://www.reddit.com/r/Superstonk/comments/nlh60l/a_deep_dive_into_the_source_code_of_the_gamestop/)


All this talk of crypto dividends and NFTs being used for a second-hand game market has gotten me extremely curious about what this GameStop NFT actually is. Thanks to blockchain explorers such as [etherscan.io](https://etherscan.io), we can actually look at what the developer of this token has created. The token is an ERC721 token written in Solidity using openzeppelin's libraries. The issue is that the contract in it's current state does not hold any function at all for the gaming market. The ERC721 standard only allows for a single owner of the token. Before you call me out for FUD, there is still a platform for GME to launch an NFT of stratospheric proportions, so stay tuned until then.

# GameStop NFT Contract

The first 925 lines of the contract come directly from [openzeppelin](https://openzeppelin.com), an organization that has created a simple library for making your own ERC721 tokens. These are the files included from the library in the contract:

    // File: @openzeppelin/contracts/utils/introspection/IERC165.sol
    // File: @openzeppelin/contracts/token/ERC721/IERC721.sol
    // File: @openzeppelin/contracts/token/ERC721/IERC721Receiver.sol
    // File: @openzeppelin/contracts/token/ERC721/extensions/IERC721Metadata.sol
    // File: @openzeppelin/contracts/utils/Address.sol
    // File: @openzeppelin/contracts/utils/Context.sol
    // File: @openzeppelin/contracts/utils/Strings.sol
    // File: @openzeppelin/contracts/token/ERC721/ERC721.sol
    // File: contracts/Gamestop.sol

Only the last 34 lines of the contract (from *contracts/Gamestop.sol)* are original and are really the only ones that contain valuable information. Here's the first line of the actual GameStop contract block:

    address public owner = 0x10B16eEDe03cF73CbF44e4BFFFa3e6BFf36F1Fad;

As you might have seen before, the above [contract's first transaction](https://etherscan.io/tx/0x56e648aff2144469a97ed0d131882ab63a1a14ff03d72ccbe9b64ee8ba74157d) was for 0.42069 ETH, which at the time of writing is worth about $1,200. The transaction took place around 4 days ago, probably in preparation for the launch of [nft.gamestop.com](https://nft.gamestop.com) Take from this what you will, but you can't ignore the significance of that number. Let's also not forget that the actual contract begins with "0x1337420" (1337 = leet short for elite, as you probably already know).

We can actually trace where this ether came from by clicking the *from* column. Etherscan shows that it was withdrawn from Binance, the most popular retail crypto exchange globally. Whether this was from [binance.com](https://binance.com) (not available in the US) or [binance.us](https://binance.us) (available in the states) I am not sure. I assume that their addresses are the same on both platforms but I could be wrong.

Nothing else of great value is available from the blockchain explorers other than around 40 people who have tried to send their eth to the GME contract, only to have the transaction reverted.

Let's take a look at the next line:

    string public ipfsLocation = "ipfs://QmaLEchFaE7FWhc4MCvYMqoTdK8rV1yfjEC5Bz4jzQRbjS";

This is an IPFS address. What is IPFS you might ask? IPFS stands for Inter-Planetary Filesystem and it is sometimes used to store the actual file for the digital asset that you would want to sell as an NFT. It's similar to the address that's at the top of your web browser. Sadly you can't just type it into chrome and visit it. However, [brave](https://brave.com/) (my favorite browser) has started to implement IPFS and you should be able to type it in view it. This address stores the landing page animation. Nothing really interesting to see there, but still intriguing that they've added it and also implemented a function for it:

    function setIPFSLocation(string memory _ipfsLocation) public onlyOwner {
        ipfsLocation = _ipfsLocation;
    }

Next, we have the *launch date* line:

    uint public launchDate = 1626261600;

Other posts have already discovered this, but this is a Unix timestamp.

From [unixtimestamp.com](https://unixtimestamp.com):

>The unix time stamp is a way to track time as a running total of seconds. This count starts at the Unix Epoch on January 1st, 1970 at UTC. Therefore, the unix time stamp is merely the number of seconds between a particular date and the Unix Epoch. It should also be pointed out (thanks to the comments from visitors to this site) that this point in time technically does not change no matter where you are located on the globe. This is very useful to computer systems for tracking and sorting dated information in dynamic and distributed applications both online and client side.

It's very simple to convert to a human-readable date and time using the website above or [https://www.epochconverter.com/](https://www.epochconverter.com/). 1626261600 Wednesday, July 14, 2021, 11:20:00 AM Greenwich Mean time. Convert that to Pacific time and you get, you guessed it, 4:20 AM.

What's interesting about this launch date is that it's only used twice - once in the declaration in the line above and once in the setter function below:

    function setLaunchDate(uint _launchDate) public onlyOwner {
      launchDate = _launchDate;
    }

Setters are commonly used in Object-oriented programming to protect data and ensure that no invalid data is being put into a variable. However, in the case of our GME token, there is no such logic. Herein lies the conundrum. This contract essentially has no function other than having a single owner. This is how most NFTs work, but the current implementation is essentially useless for what we are hoping the GME token to be. Most Ethereum tokens that you're used to are based on the ERC-20 standard, and are *fungible,* meaning they can be split up, but they don't have a single owner like an NFT. For the ability to have many people own GME NFTs, a better standard like ERC-2309 would have been used. So unless GME is planning to sell a single token to the highest bidder, this contract probably won't actually be used.

From [openzeppelin](https://docs.openzeppelin.com/learn/upgrading-smart-contracts):

>Smart **contracts** in **Ethereum** are immutable by default. Once you create them there is no way to alter them, effectively acting as an unbreakable **contract** among participants.

What I'm essentially getting at is that this is just a teaser for what is to come. This contract doesn't have any function as a gaming NFT and can't easily be minted to many users. It doesn't have any additional metadata other than the IPFS address that would make it useful to developers or retailers - although the argument could be made that all of that data could be store in the IPFS address. Still, the

# The unlimited possibilities of a gaming NFT

GameStop undoubtedly has the ability to turn the gaming industry on its head with a new NFT gaming market. You could essentially have the ability to Buy Ninja's copy of Fortnite, or Shroud's copy of CSGO. *Not only that* but you could buy the skins that they used on an open market. This is where I think the true value lies. Until now, NFTs have very limited, but still reasonable amounts of use with digital art. GameStop has the unique platform to offer game developers an easy-to-use SDK (software development kit) that would allow them to trade and buy in-game assets like skins. This would save them the hassle of implementing their in-game item shops, payment systems, and in-game currency. A sort of universal in-game currency could be created, which if you remember was one of the main draws to the NFT world.

Recently, Epic Games sued Apple over this very issue. Epic spent a shitload of $$$$$ on the lawsuit because of the 30% cut that Apple takes from the App Store. Using NFT and crypto as your in-game currency completely cuts out the middle-man and allows for the transaction to take place on any platform, on any device, website, in any in-game store, or even physical store. That's right - ***physical store***. If implemented correctly, I could go buy a CSGO skin off the shelf in a brick and mortar store and have the cashier scan my crypto address at the register to put it on my account. From that point, I own the skin and could sell it to anyone on a marketplace.

In summary, the NFT that GME published on their landing page is just a preview and most likely a teaser for what they are going to develop in the future. The July 14th date could simply be a date for when they will launch the platform but does not hold any function in the current context of the source code.