# Author: Rs_Spacers
# Post URL: [https://www.reddit.com/r/Superstonk/comments/mqb42g/i_know_a_lot_about_iex_let_me_explain_to_you/](https://www.reddit.com/r/Superstonk/comments/mqb42g/i_know_a_lot_about_iex_let_me_explain_to_you/)


Since this topic has been unnecessarily stigmatized recently, I've decided to do a proper writeup on the Investors Exchange ("IEX"). This past week I've been reading Flash Boys, written by Michael Lewis (Author of the Big Short). The book goes into great detail about the journey that Brad Katsuyama, the founder of the IEX, took from first discovering High Frequency Trading until the infancy of IEX.

All of my information comes from the book (Flash Boys). 

# Who is Brad Katsuyama?

Brad was born in Canada and had in the years prior to founding IEX been working at the Royal Bank of Canada ("RBC"). The first leap in his career was being allowed to start the Wall Street arm of RBC. What he learnt of there would within the coming decade make him the world's most knowledgeable person on High Frequency Trading ("HFT") that was not employed by a HFT company (NOTE: CITADEL IS A HFT COMPANY, AND A VERY SUCCESSFUL ONE, AS OUTLINED IN THE BOOK). In 2012 he left the company (and one hell of a wage) behind in order to, in simple terms, confront all of Wall Street.

# What did Brad discover about HFT?

The first time Brad was being affected by HFT was in 2006, after RBC had bought a company named Carlin Financial, which was a trading company with electronical trading capabilities. It was becoming very popular to shift trading over to being fully electronical, or at least mainly electronical, and RBC hadn't really done a great job of doing so. 

In the months following this, RBC had their trading platform go from a pen and paper style of trading (more or less, unsure of exactly how primitive it was) to something akin to what we do today: type in a stock and press buy to execute an order. Eventually, Brad (and many others on Wall Street) found problems with executing large block trades. What Brad experienced when he was trying to buy shares for his client was that they were kind of "disappearing" mid-way through the trade. Say for example that the client wanted to buy 1000 shares of IBM at a price of 30$. Brad would then take a look at the amount of stock available at each of the exchanges. He would find 100 at the BATS exchange, 400 at NASDAQ and 500 at NYSE, all listed for 30$. Great, right? He'd have just the right amount to fulfill his order. Brad sends out his order to the exchanges, and what does he find? The order for the BATS exchange went through... but at the other exchanges, the sell offers that were there only moments ago had disappeared. Brad was left with only 100 shares bought out of the 1000 that he wanted to buy. Afterward, when the buy order was left waiting, the price of the stock suddenly went up a few cents. It would leave Brad in a peculiar situation, having bought only 100 shares and with the price rising. What was going on!?

Brad would come to run experiments to figure out what was going on with this behaviour. It wasn't just him having this problem, nor was it only with the IBM stock, but all of Wall Street was facing the same issues, with every stock. What Brad found was that if you sent your order to a single exchange, it would always go through without any problems. He also figured out that the BATS exchange would almost always go through without problems, regardless if he sent orders to other exchanges or not in parallell.

Brad would then come to meet Ronan Ryan (current President of IEX). Ronan originally worked at a broadband company and was experienced with internet traffic and their routes. After being shown the problem, Ronan was able to figure out why BATS was the only exchange that wasn't having trouble. The reason why was simple; the BATS exchange was very close to the real-world location of where RBC was working from. It was the exchange that large buy orders would reach first. 

The underlying reason why Brad (and almost everyone, actually) were being swindled was because their orders were being "front-run" by HFT companies. Like in the example above, the reason why the shares on NASDAQ and NYSE were disappearing was because the 100-sized order on the BATS exchange was a bait, laid by the predatory HFT companies. After Brad had bought 100 shares on BATS, the HFT companies would quickly buy up all of the shares on NASDAQ and NYSE. They would then sell these orders at a markup, profiting massively in the process. 

This led to Brad and his team developing a software they named THOR. THOR was a tool to help send orders that would arrive at the different exchanges at the same time. For example, if BATS had a latency of 50 microseconds, whilst NASDAQ and NYSE had 200 and 250 microseconds latency respectively, THOR would send the orders to the different exchanges independently of each other, making them arrive at the same time (in this example, the NASDAQ order would be sent 150 microseconds before the BATS order, and the NYSE 50 microseconds before the NASDAQ one). This technology was the first real weapon that Brad (or anyone, really) ever developed to fight against HFT. 

# The rabbit hole goes deeper

HFT was not only done by companies specialized in it, but was also done (although less effectively, only profiting off their own clients) by big banks. They did this by opening dark pools, which would be used to front-run their own clients. The big banks would "drive past" their client's order and effectively pump the price of the underlying stock before it went through, before selling their own client the stock at a markup. This practice was done by ALL of the big banks, and any opposition was dramatically opposed by any means necessary. 

# What does the IEX do differently?

The primary selling point of the IEX is that they use a 61 km long cable in order to artificially inflate the latency of everyone using the exchange. This cable would provide all users an extra 350 microseconds to their latency, which is enough for the IEX to race past any HFT trying to profit off others. So what happens when you route an order to the IEX?

Say you want to buy 1000 shares of GME. You tell your broker to route your trade through IEX. There happens to be 100 for sale at IEX, 100 at BATS, 400 at NASDAQ and 400 at NYSE (which all happen to be at the National Best Bid or Offer (NBBO, regulation that was meant to make the market more fair but really only made it easier for HFT companies to manipulate it)). After your broker sends your order to IEX, they immediately execute the 100 shares available there. They then re-rout your order to the other exchanges using something akin to THOR (THOR became a patent by RBC, iirc) to the other exchanges. Before anyone can even react, your order has gone through at all exchanges at the same time, with HFTs being left in the dust because of the 350 microsecond extra latency. According to the book, it'd take approximately 320 microseconds for the order to travel from IEX to the farthest exchange, making it impossible to play catch up by the HFT (becuase of the 350 microsecond delay). Your order stays protected and no one can fool you of your money.

# Why is the IEX not mainstream already?

The book goes into detail as to why this is the case. As outlined by the book as a whole, the financial system is very combative of changes that threaten their income. The IEX was essentially attacked by financial terrorists from the day it started, both in media and on the exchange itself. One example from the book is that the big banks would send their client's orders in chunks of 100 over a period of time (a lot larger than 350 microseconds). What this did was that the HFT companies could catch the big orders and profit off of them, like normal. What the banks effectively did was to show their hand in a game of poker, in order to screw their own client of their money. This tactic was used in order to "prove" that the IEX was fraudulent, since buying shares there (using the terrible 100-at-a-time method) was more expensive than buying on other exchanges. There have been many more attempts to discredit the IEX, which obviously succeded, since they currently only execute about 2% of all trades.

# Conclusion/TLDR

The IEX is exactly what it advertises itself as: an exchange for investors. They utilize two methods for preventing High Freaquency Trading companies from profiting off of other investors orders: a 61km long cable (which introduces a 350 microsecond delay to all users of IEX) and a program that re-routes the trades through the IEX to other exchanges and make them execute simultaneously (disallowing HFT companies from "front-running" others and profiting). In my opinion, the founding members are literal saints, which deserve NO CRITICIZM. Wall Street is run by a bunch of phonies, and if there are any people that you can trust, it is the founders of IEX. They are not doing it for the money, they are doing it because **no one else** that knows what they do are willing to cast aside what they're able to make at HFT companies.

Edit: comment by PM_ME_NUDE_KITTENS
I'm probably too late to get visibility, but posting anyway.

Michael Lewis, the author of Flash Boys, runs a podcast called Against the Rules where he looks at exactly the kinds of rules manipulation we're seeing with Shitadel.

One of the episodes, called [The Magic Shoebox] (https://www.pushkin.fm/episode/the-magic-shoebox/) (podcast producer site), has a condensed retelling of the IEX story.

Audio for all the apes, like me, who never learned to read. ???????????? ????????????

If your moral outage meter isn't already pegged from the f**kery afoot in the markets, this entire podcast is a romp through how it only gets worse from here. Lewis, as he does, provides a lot of stories of apes trying to survive in the jungle despite losing the home-field advantage in every aspect of life.