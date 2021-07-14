# Author: devdevgoat
# Post URL: [https://www.reddit.com/r/Superstonk/comments/nv8h3t/introducing_dduplicate_an_immutable_dd_backup/](https://www.reddit.com/r/Superstonk/comments/nv8h3t/introducing_dduplicate_an_immutable_dd_backup/)


Hello my dear Apes, HAPPY 300!!!! I come bulling gifts!!

TLDR: In the event of MOASS disruption, go here for DD, it can't be taken down now. Not by  me, not by shills, not by anyone. It's backed up to Git, IPFS, and Wayback!

* [ipfs://Qma6rwZ4nM79MS62ZQBsE8q26dr2CKeMFBbceoL14b3gLx](https://dweb.link/ipfs/Qma6rwZ4nM79MS62ZQBsE8q26dr2CKeMFBbceoL14b3gLx)
* [https://github.com/rlamb2/SSDDScraper](https://github.com/rlamb2/SSDDScraper)

Also, maybe we should use a decentralized chat app like [iris.to](https://iris.to) ([invite link](https://iris.to/?channelId=fa88c760-c1d1-4cc6-ab97-fa125296168a&inviter=eVG59A0lM_xoTmDC-6KHe_knfuy8BAmVfIh9GPNJZf0.pDiCCkNp8GYw8fES089y4YOITmV03r8VpG9CPvYJdyg&s=fEUAO58l3zQv4SEuDvVrX5DgD_rCFZM5gieaW77Z1m0&k=X9kKDXMdYvVT))

\--- TLDR done ---

As we all saw this morning, one little snip here, or fat check there, and our entire network crumbles. This is not acceptable, and this WILL happen when the MOASS starts. So what is there to do??

I know I know, everyone is all "go gingham style!!" but when that goes down too, and we're scattered amongst twitter trying to share Dropbox links, people will get nervous. Did that DD ever actually exists?!?! HOW DO I KNOW FOR SURE?!?! IT"S BEEN 10 MINUTES!!!

We need something safer, more robust, and more importantly, not owned by anyone who can go shill at the drop of a dime... especially me!!

[So here's what I built](https://ipfs.io/ipfs/Qma6rwZ4nM79MS62ZQBsE8q26dr2CKeMFBbceoL14b3gLx). I'm not some fancy-smancy financial analyst, or a badass micro-expression expert, but I can scrub web content with cobbled together code snippets from StackOverflow! So I copy and pasted my way to a V1 one of a DWeb site that supports the following features:

&#x200B;

* [Hosted and pinned on IPFS](http://ipfs.io/), which means the content is spread across hundreds of nodes, you can even host your own in Brave Browser. I can delete it off my machine and it won't matter, someone else has already replicated the content and it [can't be modified!!](http://docs.ipfs.io.ipns.localhost:8080/concepts/immutability/)

[So many peers!!](https://preview.redd.it/j7qmcs7jk2471.png?width=1193&format=png&auto=webp&s=07821be5134364fdb035fa55d9ee417bbe412b35)

* All (or nearly all) evidence downloaded and stored on IPFS locally, so if someone deletes shit from imgur or reddit images, fuck 'em, we got our copy and that shits INLINE! (except for albums/gallery's, that shits complicated, but see last bullet for workaround)

[notice the local reference?? It's stored here: ipfs:\/\/bafybeifoypyt7xdtvpi5nzrtiyjghsx276knrsa3bpqms2kqdddrdzlj2e\/img\/vrpqxaonn6u61.png](https://preview.redd.it/r1xlwf4wk2471.png?width=1481&format=png&auto=webp&s=d1ad6f7a511df8a8bfaf4344f2ffa2535085841f)

* While copying the content I went ahead and re-published all DD to Wayback machine, and grabbed the links closest to original posting time! Seriously, this made the export soooooo much longer... worth it!

[Wayback ranked by: Near OP Date \> Latest \> Day of Archive \(6\/8ish\)](https://preview.redd.it/529gk29el2471.png?width=1286&format=png&auto=webp&s=23f828bdffbb6fef7f112f6798d835dc6ce98ba0)

* And since I was spamming wayback anyway, I did the same for [ALL embedded links](https://github.com/rlamb2/SSDDScraper/blob/master/archives.json), creating a new wayback archive (unless one near posting existed already)! However, I still need a solution for YouTube links, I backed up [all the youtube links](https://github.com/rlamb2/SSDDScraper/blob/master/youtube-list.txt) to a file so we can scrub those separately... maybe use a web-torrent video solution for these?? Suggestions welcome!

https://preview.redd.it/hil2dxink2471.png?width=1295&format=png&auto=webp&s=39c2292b03d2fee44f4600a926da7e5037df3537

* Oh, and I injected the wayback links inline to the post as well, so if you're readding HOCII and the fuckers tried to edit Investing.com's definition of "fuk'd" you can see the original

&#x200B;

Couple things to note:

* You can use the direct Qxx links, but one problem with the immutability concept, we can't add NEW DD to that Qxxx page, so I have to build a new one and republish with the updated list of DD, which means a new CID. Thus, if I update with new DD, I'll try to periodically update the an ens address/URL, though it costs like 5-10$ each time, so wont' be updating often.  Not sure if we can use an OrbitDB node in browser to solve this or not??
* Further more, I think there needs to be a more resilient communication system. Twitter is great, but I think iris.to might be better? Especially compared to discord that can be shut down with a few shill reports. I've not really used it much (none of my -3 friends want to test it with me :( ), and I'm not affiliated with it in anyway, but I created a room called Superstonk here, might be useful idk:

[https://iris.to/?channelId=fa88c760-c1d1-4cc6-ab97-fa125296168a&inviter=eVG59A0lM\_xoTmDC-6KHe\_knfuy8BAmVfIh9GPNJZf0.pDiCCkNp8GYw8fES089y4YOITmV03r8VpG9CPvYJdyg&s=fEUAO58l3zQv4SEuDvVrX5DgD\_rCFZM5gieaW77Z1m0&k=X9kKDXMdYvVT](https://iris.to/?channelId=fa88c760-c1d1-4cc6-ab97-fa125296168a&inviter=eVG59A0lM_xoTmDC-6KHe_knfuy8BAmVfIh9GPNJZf0.pDiCCkNp8GYw8fES089y4YOITmV03r8VpG9CPvYJdyg&s=fEUAO58l3zQv4SEuDvVrX5DgD_rCFZM5gieaW77Z1m0&k=X9kKDXMdYvVT)

Mods, contact me via verifiable means and I'll make your iris account the owner of this group. I don't want this to be a shill vector by adding some rando to the mix (me). The whole point of this is that I can disappear and it doesn't matter!!

hmmm lets see...what else. Oh, I published the whole thing (included DD text, but not images...sry I'm on a free account till MOASS) to [GitHub here](https://github.com/rlamb2/SSDDScraper). DONT LAUGH AT MY CODE, IT WORKS DAMNIT!

Welp, that's it.. Be free my little data project... go off into the wild and grow big and strong like a single GME share!!

Oh and if you don't mind, if anyone is hosting an ipfs node, please pin it: Qma6rwZ4nM79MS62ZQBsE8q26dr2CKeMFBbceoL14b3gLx

Edit: some wurds