# Title: Gamestop NFT current state - Lets dive in
# Author: R_Hugh_High
# Post URL: [https://www.reddit.com/r/Superstonk/comments/or8nis/gamestop_nft_current_state_lets_dive_in/](https://www.reddit.com/r/Superstonk/comments/or8nis/gamestop_nft_current_state_lets_dive_in/)


**Preface:** I've only had a general understanding of Krypt0 for a while. Also am drunk so forgive any kind of typos etc. :) however since I heard about the nft news, I've kind of become obsessed with the idea and what goes on with the address containing it and also heard alot of confusion about it. So I'm trying to help the community in the only way I know how other than hodl of course.  Hopefully some more wrinkly brained kriptoe apes can come in here and clarify on some of the things I got wrong/help with questions.

======================================================================

Let's start at the only official hint from Gamestop that we have now: [nft.gamestop.com](https://nft.gamestop.com)

This is your only verifiable place to start. Now understand there are alot and I mean ALOT of scammers when it comes to anything regarding crytpo addresses. If you decide to delve in any further understand that more so than ever.

So lets plug that address (0x13374200c29C757FDCc72F15Da98fb94f286d71e)  that was at the [nft.gamestop.com](https://nft.gamestop.com) website just into google. The first thing that comes up is its 3threrscan address. (automod doesn't like the e      t   h e r word sorry)

Heres a fun picture of what it looks like on the scanner website!

&#x200B;

https://preview.redd.it/25kesmohmbd71.png?width=1914&format=png&auto=webp&s=7b52822c77a0ab3dd831ebcd31e987e278b64e1e

&#x200B;

&#x200B;

Now, that's cool and all, but whatever right? See that tab titled "contract" there? lets click it and see what it yields.

&#x200B;

https://preview.redd.it/oomi2eevmbd71.png?width=1673&format=png&auto=webp&s=cdcb92f60e83e2745bd6f51d3dc96ba99d25dd2b

Boom! this is the contract source code for 0x13374200c29C757FDCc72F15Da98fb94f286d71e(the official gme token) that got so hyped up because of it's \[get launchDate\] method back in may. The head of blockchain for gamestop made a [public tweet](https://twitter.com/finestonematt/status/1413615681489227779?s=20) leading up to the date that was a unix timestamp informed everyone that it was just a speculative date for a huge upgrade to the e th e re um upgrade(london fork if you want to research it). Being a programming student and looking at the code, the launchDate uint variable does nothing and that the official release was just a 'teaser' token. You can see that it was minted back in may if you click the 'events' tab under the contract page, so I'm inclined to agree with him. There's only one method in the source code that interacts with 'launchDate' and its a mutator method, which means it can't do anything except be changed. BUT! the unix timestamp was interesting for reasons I'll get into near the end.

&#x200B;

&#x200B;

So, if you're still on this page with the contract open (\*I hope you are\*)

See this little button that says "read contract"? go ahead and click that shit let me jack your tits.

https://preview.redd.it/tcdsns3robd71.png?width=668&format=png&auto=webp&s=54cf18219a0785728caf5a01e08e26d7d83bc8c9

&#x200B;

Now that you're here, you're going to see a bunch of methods that you can interact with, most of them yielding you nothingburgers. But there is one, and believe me, its a fun one. Go ahead and click the 'owner' method. That will show you an address: 0x10B16eEDe03cF73CbF44e4BFFFa3e6BFf36F1Fad 

&#x200B;

https://preview.redd.it/e7jce3nspbd71.png?width=1620&format=png&auto=webp&s=c1bd03521346d73b094d82b849ae814559a90081

Wouldja look at that. That's the address of the gamestop nft we heard about in may. This address is another contract. This contract is called a "gnosis safe". A gnosis safe is controlled by several different addresses and confirms or denies transactions. 

Now that we're here, let's poke around.

&#x200B;

before we go further: understand that ERC-721 tokens are NFT's and that all the scamcoins are ERC-20's. dont even pay attention to the erc20's imo.

&#x200B;

So here we are at what henceforth I'll call 10b, shortening the address. now that we're here, lets do what we did with the official address, click contract then click "read as proxy" (this ones weird with the proxy thing, im still learning.  Keep in mind this is a contract that owns the official contract, I know it can get confusing, don't go too far off track or you'll get lost.)

 Now we have a bunch of methods to interact with just like with the official contract. From here click the 'getOwners' method and you should yield this:

&#x200B;

https://preview.redd.it/goxv5wlfrbd71.png?width=1794&format=png&auto=webp&s=3acd77074ec570d5db2578ac3ea4e62dc0eff3c5

aint that cool?! we have 6 addresses that control the gnosis safe that owns the gamestop nft!

they are as follows:

 0x306192f216ff57bdb67c8e44fe306cfbe2c3eaf7

0x850aa0b86b8aa76b95cef283bcb2e7c008c7202b,

 0x97a89a96408078a81401cc909aa439b49fbd8da1, 

0x3092de8895d92eb271bf9372b1f1bab29d214322, 

0xdd9bdf825a4bb9851cdf58861214d433f92ba1db,

0x61a80d1792340c2a03e739202980e69467459a8b 

Now most of these aren't very interesting... for now at least. 

However the most interesting are the second to last(0xdd9) and the last (0x61a) addresses. These seem to be the "master" addresses. I would chew on the fat of that, but that's a whole 'nother subject, let's stay kindof focused. Since the inception of the gamestopnft.eth(the name of the ens for the official gamestop nft) our little 0x61a buddy has claimed it's own nft: powertotheplayers.eth

&#x200B;

https://preview.redd.it/oo2l187ksbd71.png?width=1420&format=png&auto=webp&s=e910d07d80b2240344b3b8c88eabcd7984cab17a

this address along with 0xdd9 seems to deal with some of the moderation I guess. I dont know enough about how safes work or hell, even kr i p toe for that matter but I've learned a decent amount by watching these addresses :) If you check the 'Events' tab under the safe account address, you'll see that dd9 and 61a have added and removed owners. bbd was the address that created the safe and has since been removed as of 9 days and 8 hours ago. (I suspect this was foobar but I can only speculate, dont go jumping to conclusions lol)

The 'Events' tab is my favorite to check.

This is where things get interesting: So, the unix timestamp that everyone was so hyped up about and got disappointed with(bs posts like "REEEE THE NFT DID LAUNCH ON 7/14") newsflash buddy, it was minted 61 days ago:

&#x200B;

https://preview.redd.it/5csm515pubd71.png?width=1609&format=png&auto=webp&s=9e95795be245e5d466b30d099c965383de149ed1

see: 'mint'

&#x200B;

But what people weren't looking at was the gnosis safe. our 0x10b buddy (or group of buddies rather). Later that night a new nft was added to our 0x10b: and it's ens is GME.eth

 

https://preview.redd.it/zworgh2fvbd71.png?width=1488&format=png&auto=webp&s=0281e2dc9e9bad4c8a0b967a9265f4218d644831

&#x200B;

![The new gme.eth added to the 0x10b group](https://preview.redd.it/35erd5irvbd71.png?width=527&format=png&auto=webp&s=5c67cc36520ce12760cebaa9207b522a13e90632)

&#x200B;

Now I know what you're thinking, "Anyone could give this account an nft or kri p to3 or whatever right?"

Yeah, you're right for the most part, but let's dive in and look at the address that added this.

&#x200B;

From the outside this just looks like some stranger right? I thought it was too, but check this fuckin shit out. The address that added the new "gme.eth" 9 days ago was added by this address:

0x381636D0E4eD0fa6aCF07D8fd821909Fb63c0d10

By scrounging through Matt Finestone's twitter (head of blockchain for gamestop) you'll find a [reweet](https://twitter.com/finestonematt/status/1389726384222769153?s=20) where he thanks the creator of an nft he purchased (which is also his current profile picture on twitter) in which the creator first thanked the buyer of it dropping our same address( 0x381..0d10). CONFIRMING THAT FINESTONE ADDED A NEW NFT ON THE LAUNCHDATE!!!! 

IMO: the gamestopnft.eth was a red herring and the nfteam is currently working on an implementation of the gme.eth.

&#x200B;

anyways, im drunk asf, wanted to clarify some things, and will possibly write more once i have typing drugs in me. Cant stop, wont stop, gamestop.
Ok
wont flair this as DD, because I want the community to help with this, that is our strongest tool.

Plz dont ban this post automod :(