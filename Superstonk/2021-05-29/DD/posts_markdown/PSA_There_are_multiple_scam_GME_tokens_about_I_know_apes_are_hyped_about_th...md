# Author: Safisynai
# Post URL: [https://www.reddit.com/r/Superstonk/comments/nnmf9b/psa_there_are_multiple_scam_gme_tokens_about_i/](https://www.reddit.com/r/Superstonk/comments/nnmf9b/psa_there_are_multiple_scam_gme_tokens_about_i/)


**Mods:** I flaired this DD, but please let me know if another flair would be more appropriate.

**Edit:** Added links to the transactions mentioned in this post to back up what was said.

I tend to mostly lurk and don't comment or post things on Reddit a huge amount, but I've been involved with crypto for some time, and GME since January, and this needs to be said before someone ends up getting scammed.

With the recent teaser about the GameStop NFT (The actual, legitimate token contract address can be found on nft.gamestop.com), people are naturally pretty excited. Many apes are not overly familiar with crypto, and the combination of excitement, FOMO, unfamiliarity with crypto and likelihood of having money to spend (given that apes are buying GME), apes are very attractive targets for crypto scammers.

Please be super careful at any new token you see bearing the label of "GME", "GME Coin" or similar. There are a few very important things all apes should be aware of regarding crypto (particularly the E-hereum (name censored because of automod's wordfilter) platform, on which the *actual* GME NFT contract is deployed) to reduce your risk of falling for scams.

**First and most important:**

**Anyone can deploy a token contract, and they can give this token any label they want.** The `name` and `symbol` fields of an ERC-20 (the standard which all fungible (these are different from NFTs, which are covered by the ERC-721 standard) follow) token contract can contain **arbitrary** values set by the deployer of said contract.

Just because a token's symbol is "GME" or it's name contains the word "GameStop" **does not mean the token has anything whatsoever to do with GameStop Corp.**

**Secondly:**

You can send a token to any address on the network. The receiving address does not have to actually do anything to receive/accept this token, and indeed, may not even be aware they have been sent this token. Sending tokens to random addresses is a pretty common guerilla marketing tactic for crypto projects, and more often than not, one employed by particularly shady projects (scams, pump & dumps, etc). This is such a common thing that "token spam" is a well known phenomena to folk in the crypto space at this point.

**Just because some token is sent to the actual GME NFT contract, does not imply any kind of association with GameStop Corp. Any spammer can send whatever random tokens they want to it.**

**Finally:**

At the time of writing this message, no legitimate GME NFT units exist; a token contract has been deployed, one unit was created in the [same transaction](https://etherscan.io/tx/0x89df343d7e245d42a09de2c790c8c471a0956f32b55631a53a15268c56a74c2d) as the deployment of the contract (likely either a mistake or a test), and was ![burnt](https://etherscan.io/tx/0x39cc33bf2eb46bb2dc483c9f685e5f04307ebb9526f6be9027f71bdb71e3e6b6) (permanently, irrevocably destroyed) shortly thereafter.

**Anyone trying to sell your any kind of "GME" token at this point in time is almost certainly trying to scam you.**

To help explain this, here is an example of just one type of scam that you could potentially fall for:

1. The scammer creates a worthless ERC-20 token and gives it a name and symbol that make it look like it has something to do with GameStop Corp. e.g. they may give it the symbol "GME" or name it "GameStop coin" or similar. As the creator of this token contract, they can give it whatever rules they want (i.e. they can give themselves as much of it as they desire).
2. The scammer sends some of these worthless tokens to the actual GME NFT token contract address, to give some extremely thin veneer of legitimacy to it in the eyes of apes who are unfamiliar with crypto. Apes come along, see the actual GME NFT contract has this token and assume that this is proof of legitimacy (**it is not**).
3. The scammer sells their worthless tokens on a decentralised exchange. On most decentralised exchanges, any ERC-20 token can be traded from the moment it's created; no one needs to manually list the token on the decentralised exchange, nor does anyone need to verify it's legitimate, or even look at it in any way.
4. Excited apes FOMO into the token and end up giving their money to the scammer, receiving nothing in return but a worthless token.

I've already seen at least one likely attempt at this scam mentioned in the comments here (feel free to look through my comment history where I've been pointing this out). I know everyone is excited, but please, be very careful; crypto transactions are irreversible and if you are scammed, you will not see those funds again - there is no way to undo a transaction, and any competent scammer will likely immediately launder their profits via an anonymous crypto such as M-nero, rendering attempts to track them down impossible.

Whenever handling tokens **always** verify the address of the contracts with which you interact, and compare these against addresses from **known legitimate** sources (such as nft.gamestop.com).

**TA;DR: Don't FOMO into random "GME" tokens without actual proof they are legitimate. Stay safe out there!**