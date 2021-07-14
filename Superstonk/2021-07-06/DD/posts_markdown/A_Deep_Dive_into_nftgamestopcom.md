# Author: schismsaints
# Post URL: [https://www.reddit.com/r/Superstonk/comments/oezh1f/a_deep_dive_into_nftgamestopcom/](https://www.reddit.com/r/Superstonk/comments/oezh1f/a_deep_dive_into_nftgamestopcom/)


Like many, I was intrigued when I heard about GameStop dabbling in NFT - first, through the [job postings](https://finance.yahoo.com/news/gamestop-hiring-blockchain-analyst-specializing-075700175.html), then with ![nft.gamestop.com](https://nft.gamestop.com).  I did a [brief dive into some of the smart contract details](https://www.reddit.com/r/Superstonk/comments/nkxrhe/umm_guys_i_think_i_just_found_something/gzgpytb/?context=3) back when it initially came out but recently have gone much further down the rabbit hole.

I'll summarize some of the juicier bits and provide some speculation as to what it could mean as well as some resources to familiarize yourself with some of the details of blockchain, smart contracts, and tokens, but I have put together a [larger graphic](https://github.com/schismsaints/GME_NFT) in PNG/PDF/SVG formats visualizing some of the connections a little better (fair warning, I'm an engineer not an artist).  I recommend loading it in a full web browser on as large of a monitor as possible.  You'll understand why when you see it.

First, a few key terms/concepts.

**Blockchain**: In very simplistic terms, think of the blockchain as a ledger/record keeping system where each 'block' is a record and linked to the previous and next blocks in a chain.  The process of adding a new 'block' involves computing and verifying prior information in the chain to ensure that nothing has been tampered with and that the full history of the chain is intact.

[Blockchain Definition: What You Need to Know (investopedia.com)](https://www.investopedia.com/terms/b/blockchain.asp)

**Fungible**: "being something (such as money or a commodity) of such a nature that one part or quantity may be replaced by another equal part or quantity in paying a debt or settling an account " (src: dictionary.com)

**Token**: This is probably the part most people understand, though there are some nuances.  There are two types of tokens and a number of differing implementation standards.

* Fungible Token - ERC-20: A token that is one of a pool of identical tokens.  They can be split, transferred, or exchanged and are commonly used as currencies.  Most established mainstream or alt- coins fall into this category.
   * [Cryptocurrency Definition (investopedia.com)](https://www.investopedia.com/terms/c/cryptocurrency.asp)
* Non-Fungible Token (NFT) - ERC-721/ERC-1155: A non-fungible token is a unique entity on the blockchain.  There are no others exactly like it, and it has its own record of ownership, attributes/metadata, and cannot be substituted for another token identically.  [CryptoKitties](https://www.cryptokitties.co/) is one of the most popular examples as they basically pioneered the ERC-721 standard.  NFT artwork is another recently popularized example of this.
   * [Non-Fungible Token Definition: Understanding NFTs (investopedia.com)](https://www.investopedia.com/non-fungible-tokens-nft-5115211)

[Non-Fungible Kitties!](https://preview.redd.it/frjg3859im971.png?width=300&format=png&auto=webp&s=f348dbe6d884a59ea2017cb889df592c750bb54d)

**Smart Contract**: A smart contract is a way to automate 'stuff'.  That 'stuff' can be any number of tasks but some of the most common ones include creating (minting) or destroying (burning) tokens from an available pool.  This can be fungible or non-fungible tokens (or, in the case of ERC-1155, both/either).

[Smart Contracts Definition (investopedia.com)](https://www.investopedia.com/terms/s/smart-contracts.asp)

The GME NFT story started in earnest with GameOn Anon, the smart contract address posted at ![nft.gamestop.com](https://nft.gamestop.com)

&#x200B;

[Power to the Players](https://preview.redd.it/zftk714bim971.png?width=268&format=png&auto=webp&s=f044bd9c9e8381d7d2e626ef299089e3a95165dd)

[0x13374200c29C757FDCc72F15Da98fb94f286d71e](https://etherscan.io/address/0x13374200c29C757FDCc72F15Da98fb94f286d71e)

There are a lot of interesting threads from the smart contract, the most well known of which is the "launchDate" variable which equals 04:20 PDT 7/14/21 (come on, that can't *not* be intentional).

&#x200B;

https://preview.redd.it/90uf327cim971.png?width=633&format=png&auto=webp&s=b6210524ec98857e20717ac5e4208420b9fe5909

The [owner](https://etherscan.io/address/0x10b16eede03cf73cbf44e4bfffa3e6bff36f1fad) of the smart contract is also interesting.

It owns the only GME ERC-721 token, 420.69 of the GME ERC-20 token, an E t h e r e u m Name Service record ([gamestopnft](https://etherscan.io/token/0x57f1887a8bf19b14fc0df6fd9b2acc9af147ea85?a=0x10b16eede03cf73cbf44e4bfffa3e6bff36f1fad#inventory)), and the 1337 [email signature](https://etherscan.io/token/0xc9ff785a33f2000652d0336e476a06ccd909317a?a=0x10b16eede03cf73cbf44e4bfffa3e6bff36f1fad#inventory) prefix used for several blockchain constructs.

It also received 0.00001337 E t h e r on 5/25/21 from andrwyng (wut doing Andrew Yang??)

Edit: Not actually Yang - [https://mobile.twitter.com/andrwyng?lang=en](https://mobile.twitter.com/andrwyng?lang=en) \- thanks [/u/No-Information-6100](https://www.reddit.com/u/No-Information-6100/) 

https://preview.redd.it/f20fgc1dim971.png?width=759&format=png&auto=webp&s=411a0885caa8b1774f679644625e5d1c57b890b3

There are three GameStop specific tokens they appear to be working with, along with a number (>20) altcoins and other tokens.

* [GME Coin (ERC-20)](https://etherscan.io/token/0xd4596454a0e145842d1319d6921399e8e1622ad7) \- Qty 12,000,000
   * Possible online store/digital currency?  Would be interesting if it functioned similar to a [stablecoin](https://www.investopedia.com/terms/s/stablecoin.asp) pinned to the dollar
* [GameStop (ERC-20)](https://etherscan.io/token/0x5b7d043ecb3a694069cc01e763159ea1bde0541d) \- Qty 69,420,000
   * They moved a large amount of this (>50%) to [Uniswap](https://en.wikipedia.org/wiki/Uniswap) which in layman's terms can be considered as kind of an escrow/holding/forex account but in the crypto realm.  Quite a few have been distributed from here to over 60 different destination addresses.
   * Yahoo! Finance lists the 'Implied Shares Outstanding' for GME as 69.38M, which is preeeeeetty close to the 69.42M tokens minted here.  Could this be used as a shareholder dividend, potentially exchangeable between GameStop and GME Coin/USD?

https://preview.redd.it/o377yvulim971.png?width=336&format=png&auto=webp&s=67c5f337f72a52c90a8dc235e83c99a17cbf21e3

[GME ERC-20 Token Holders](https://preview.redd.it/lnhnub7nim971.png?width=1334&format=png&auto=webp&s=26151aac8411c26ca823c7eb1b656a9b396110e9)

[GME ERC-20 Token Activity](https://preview.redd.it/y8dxdtxnim971.png?width=1347&format=png&auto=webp&s=e2e143155c28184e528fe578f81231b3ea6809d7)

* [Gamestop (ERC-721)](https://etherscan.io/address/0x13374200c29C757FDCc72F15Da98fb94f286d71e) \- Qty 1
   * There is only one of these in existence at this point with no clear use for it yet, but there are some interesting possibilities I've considered such as blockchain-based share tracking (i.e. each NFT would have a 'share # X' value on it) or as a shareholder ID token ('shareholder # X').  This one has the least clear forward looking use case at this point for me.

**Possible Business Uses**

* In-store currency - GME Coin can be used as an in-store currency/reward system
* Crypto swap/exchange - Partner with an established cryptocurrency company to facilitate listing and conversion/exchange between stablecoins such as USDC or miscellaneous established coins or altcoins, and GME specific tokens.  Use a GME app to manage a crypto wallet and exchange between various tokens/coins/currencies.
* NFT Collectibles - i.e. CryptoKitties, Gods Unchained, etc.  Facilitate in-person trading (either in-store or via app to app trading) of digital items and collectibles between platforms.
* Digital game licensing - revolutionize DRM by hosting a record of your game license on the blockchain
* In-game item transfer/entitlement - Imagine if there was a way to trade/sell your CounterStrike skins in-person for cash, or exchange a cool knife skin for a new CryptoKitty

**Possible Shareholder Uses**

* Shareholder record keeping - have a token proving your status as a shareholder
* Share/securities record keeping - similar, but for shares.  Kind of a stretch but could be a proof of concept for blockchain based trading
* Crypto Dividend - Provide GameStop (ERC-20) tokens, even fractional ones, as a shareholder dividend.  Allow conversion to USD or GMECoin/USD to cash out.  Provide a way to purchase or 'auction' GameStop tokens and you now have a shareholder perk with monetary value that could appreciate over time.

Here's the PDF of the chart/diagram I put together, the github link also has PNG and SVG versions of the image.

[GME\_NFT/GME\_NFT.pdf at main · schismsaints/GME\_NFT · GitHub](https://github.com/schismsaints/GME_NFT/blob/main/GME_NFT.pdf)

TL:DR; GME doing crypto stuff.  Lots of crypto stuff happening especially in the last week.  Crypto stuff has lots of options, most of which will print money.

&#x200B;

[I like money.](https://preview.redd.it/m5kf78utim971.png?width=492&format=png&auto=webp&s=f261c660c01332c063076409dd5fb6bccd950272)

Edit: to answer a good point brought up by /u/haydonny1 \- the alt coins could be sent by any random source and aren't concrete proof of anything.  I still maintain that the three GME tokens are legitimate and all have ties back to the original Smart Contract either one or two levels removed.  I haven't investigated the altcoin sources enough to be able to say whether or not they're being worked on by GME at this point.

0x13374200c29C757FDCc72F15Da98fb94f286d71e

* Is the address posted on ![nft.gamestop.com](https://nft.gamestop.com)
* Owns 69,420.69 GameStop ERC-20 tokens
* Owns 2,000,000 GME Coin ERC-20 tokens

0x10B16eEDe03cF73CbF44e4BFFFa3e6BFf36F1Fad

* Is the Smart Contract address listed in the source code of the ![nft.gamestop.com](https://nft.gamestop.com) smart contract.
* Holds 1 Gamestop ERC-721 token
* Holds 420.69 GameStop ERC-20 tokens
* Holds gamestopnft and 1337

Between just these two smart contracts are I believe enough evidence to prove that all three of the GME tokens (GameStop ERC-20, Gamestop ERC-721, and GME Coin) are all legitimate and being worked on by the NFT team.

&#x200B;