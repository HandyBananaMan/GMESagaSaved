# Author: dentisttft
# Post URL: [https://www.reddit.com/r/Superstonk/comments/ofi0yw/deeper_dive_into_etf_ftds_and_t35/](https://www.reddit.com/r/Superstonk/comments/ofi0yw/deeper_dive_into_etf_ftds_and_t35/)


*This post is for education purposes only. Not financial advice.*

**TL;DR-**

* Operational shorting allows for 5 business days of ETF FTDs before the T+35 timer starts
* Stock can be shorted through an ETF by going short on the ETF, breaking it apart, and buy-to-cover the underlying (outside of the stock you want to short) back into the market
* GME's negative beta comes from the ETF FTDs

&#x200B;

For the last few weeks I’ve been looking into ETF FTDs to figure out the details. There’s a lot going on. This post will be mostly informational. If you already know about certain topics, feel free to skip over the section.

&#x200B;

# Preface

I’ve gotten a lot of good information about ETFs using this video: [https://www.youtube.com/watch?v=ncq35zrFCAg](https://www.youtube.com/watch?v=ncq35zrFCAg)

&#x200B;

# Operational Shorting

Market Makers are allowed to fail-to-deliver ETF shares and hold them as failures for three extra days in the name of liquidity! It is due to a market maker exception allowing this. The way this looks is: (a) trade date, (b) becomes a FTD on T+2, (c) allowed T+3 more days of holding it as an FTD, (d) cover the FTD on the sixth day (in our case, opening puts to delay T+35 more days).

[MM’s are allowed to keep FTDs open for a few extra days.](https://preview.redd.it/3khunklh8s971.png?width=632&format=png&auto=webp&s=af873b5aab526ee1bb885794851a208312d437ce)

***Important Note:*** In the video he mentions T+6 a lot, but in the footnote of his paper he points out the rule is actually T+5, but they collected all of their data before the rule was changed. So they presented it with T+6 still.

They don’t HAVE to keep it open for the extra days, but they often do. Looking at the weighted ETF FTD heatmap, you will see groups of 2-3 days showing this exact thing.

&#x200B;

[The darker green signifies a higher weighted amount of FTDs within the ETF.](https://preview.redd.it/m2se9inm8s971.png?width=1328&format=png&auto=webp&s=230da391dd110850c884d027b0f21fba91e9870f)

&#x200B;

&#x200B;

# How to short a stock through an ETF

Authorized Participants (AP) have the ability to create and break apart the ETFs (watch the twinkie example from the video for a simple explanation. Twinkie example starts here: [https://youtu.be/ncq35zrFCAg?t=540](https://youtu.be/ncq35zrFCAg?t=540) ) The ETFs can only be broken apart or created in groups, called creation units.

If an AP borrows ETF shares and pays a small fee, they can break groups of ETF shares into all the individual underlying stock. They then buy all of the underlying stock back from the market EXCEPT for the stock they want to short. This creates a short position through the ETF. After a few days (+ another 34 days if they open puts), they’ll need to buy back the underlying stock, create the ETF shares, and return them.

Here is a graph showing the day-to-day number of shares in existence of the three GME ETF’s with the most FTDs.

[XRT and IWM shares outstanding drop at the end of January while XSVM is steadily climbing over time.](https://preview.redd.it/85e90mur8s971.png?width=892&format=png&auto=webp&s=e7ba654d253bc83d1b8536d332860ad31496da54)

*\*\*\**

***Side note:*** *Today is the first day I noticed XSVM has been steadily climbing in the number of shares outstanding. It makes me wonder if this is normal or if SHFs are hiding their FTDs into XSVM as time passes. There is a huge spike in XSVM shares outstanding around 6/16-6/21, which we don’t have FTD data for yet. But the last time it did something like that was 12/18-12/21 which happens to be 35 days before 1/22. 35 days following 6/21 would be 7/23. Not going to lie, this seems pretty important… but I must continue with this post. Maybe I can circle back around and look into this on a different post.*

\*\*\*

# Short Sale Restricted and ETFs

When GME drops 10% during regular trading hours compared to the closing price of the day before, it goes on Short Sale Restricted for the rest of the day and the next day. When this happens, SHFs can’t short GME directly so they short it through the ETFs.

Here is a chart of the ETFs weighted by the GME weighting within the ETF as of the beginning of June. I didn’t adjust the weights over time, but hopefully this should get pretty close. Ignore the units, just look at the relative sizes.

[FTDs counts from the more shorted ETFs](https://preview.redd.it/w432hjy19s971.png?width=891&format=png&auto=webp&s=40c53affede24ce37ddf8acc8beab9288a475272)

And here is the same chart with SSR days marked in green.

&#x200B;

[Green boxes around SSR periods.](https://preview.redd.it/4n9yk0w59s971.png?width=891&format=png&auto=webp&s=cf08aace6c62a10bad5ee76b5677938ab1d1e798)

This chart is a little confusing and not super obvious, but the important part is that ETF FTDs go up after a 5 day delay due to operational shorting.

# What happens after FTDs jump on ETFs?

It gets taken care of the same way as I explained in my original T+35 theory DD.

[T+35 is the one true "cycle"](https://www.reddit.com/r/Superstonk/comments/o155a6/t35_is_the_one_true_cycle_evidence_to_back_my/)

The difference is that GME FTDs start the 34 timer when they show up as FTDs while ETF FTDs don’t start the 34 day timer until they get cleared.

[Start the 34 day countdown on the day the ETF’s FTDs drop.](https://preview.redd.it/sz0zqklj9s971.png?width=834&format=png&auto=webp&s=52cfa8213e6485da19e0097bb9b25398438f9a32)

&#x200B;

But let’s continue with my old T+35 DD and first let’s double check that puts are being opened. I’m only going to show one example, but this can be done on other days too. Here is XRT. FTDs stack up from 1/28 and 1/29. On 2/1, 2/3 and 2/4 the FTDs drop.

&#x200B;

[Three different days where a lot of FTDs are “cleared”.](https://preview.redd.it/6jb1s8hq9s971.png?width=716&format=png&auto=webp&s=e655d9fc9cf2e9f8e5e6fe033d710e95275c7160)

&#x200B;

So let's look for puts. They are almost always on the first monthly expiration that is more than 35 DTE. In this case, March 19, 2021.

&#x200B;

[ Puts opened on Feb 1](https://preview.redd.it/28vugmmy9s971.png?width=1565&format=png&auto=webp&s=8193d13ea0b56f48545d073178a9913db2ff23ca)

[ Puts on Feb 4](https://preview.redd.it/va7x74dz9s971.png?width=892&format=png&auto=webp&s=a969728ad8de054dcbff09ef55380d9b52bd4b76)

&#x200B;

# T+35 and ETF FTDs

Now that puts have been confirmed to be opened, it's time to check out what XRT does after 34 days. If the puts for XRT are opened from Feb 1 to Feb 4, then T+35 would give the 34 day cover to be 3/5 to 3/10.

[T+35 of ETF FTD leads to a jump](https://preview.redd.it/ow9v8ny8as971.png?width=939&format=png&auto=webp&s=2785b90b52103276ef518bf21f2aea5454bf8324)

&#x200B;

Cool, the good ol' T+35 jump. And we all know what happened to GME during those times. But let’s look at another stock that’s in the XRT ETF. It doesn’t seem to move.

&#x200B;

[It doesn’t move.](https://preview.redd.it/6gopjc3fas971.png?width=994&format=png&auto=webp&s=0571b6e71700273bad93164bf325f14536895e4e)

&#x200B;

And this has been the hardest part of tracking ETFs. The underlying doesn’t always behave how you would expect. Some underlying does move with XRT during these times, some moves opposite of it.

&#x200B;

Also, interestingly enough, you can find 35 day gaps on the XRT Shares Outstanding graph.

https://preview.redd.it/pqhiopyqas971.png?width=889&format=png&auto=webp&s=28c98f3e1c1a431a66436e07d1a3f79ce6bfa5c9

My guess is that SHFs short the ETF. Then FTDs come due, GME goes up, and they re-short the ETFs to control it again.

&#x200B;

# Underlying vs ETF

Which leads me to some helpful tips when looking at this stuff:

* If the ETF goes up, but the underlying stays the same: The ETF is being bought to break apart and the underlying is sold back to the market.
* If the ETF drops, but the underlying stays the same: The underlying is being bought up, created into ETF shares, and the ETFs are being sold back into the market.
* If ETF goes down and the underlying goes down, the market is just dropping or the ETF is being shorted along with that particular underlying stock.
* If the ETF goes up and the underlying goes up, the market is going up in general.

It doesn’t always follow this, but you have to remember that ETFs are bought and sold like shares. So when the ETF and the underlying differ by a significant margin, then there’s probably something creation/destroying related that is happening.

&#x200B;

# Negative Beta

At this point it is well known that GME has a strong negative beta. I believe this ETF stuff is the reason why. The negative beta posts started showing up around February/March and that’s when the effects of ETF FTDs started coming into play. That’s also when the price and volume disconnected.

When GME is going up, ETFs get shorted and the price of a lot of underlying stock will drop or stay flat leading to SPY to drop. When GME’s ETF FTD’s get covered, the ETF drops, but the underlying rises leading to SPY to rise.

Let’s look at one last chart. I *attempted to* line up the ETF FTDs with their T+35 cover dates on SPY.

[ETF FTDs with their T+35 dates on SPY. ](https://preview.redd.it/9qszoed8bs971.png?width=987&format=png&auto=webp&s=cb2643e327fa06c591673f59a23ff4f9301396ff)

ETF FTDs line up with rises in SPY. Pretty cool, eh?

&#x200B;

# Bonus Material #1

An ape by the name of u/isnisse messaged me with something about T+42. At first, I didn’t think much of it. Then it clicked… T+5 from operational shorting into T+35 from puts, leads to just about 42 calendar days. They did some analysis to show correlation with GME’s price and 42 days. I think what they actually picked up here was the ETF FTD cycles. Here is the post:

[https://www.reddit.com/r/Superstonk/comments/oa2ks6/t42\_is\_likely\_the\_new\_black/](https://www.reddit.com/r/Superstonk/comments/oa2ks6/t42_is_likely_the_new_black/)

# Bonus Material #2

Another ape by the name of u/BurningMist plotted cumulative FTD value vs GME stock price. I have no idea what it means, but I figured I’d let people see it for themselves. Could this mean that the only price movements we see are based on FTDs? And retail has 0 effect because all our orders run through Dark Pools? I don’t know. Here's his message with imgur links to the graphs.

&#x200B;

>There also seems to be a relation with the cumulative GME FTD notional value and the daily low price 35 days later. I summed up the $ value of all cumulative GME FTDS from 12/1/20 until 6/15/21 and if you plot that vs the log price 35 days later you get [this](https://i.imgur.com/Gjyp5Rk.png). I also made another trendline from 1-4-21 to 6-15-21 and got [this](https://i.imgur.com/rMJhUDe.png).  
>  
>I've been running on the exponential increase assumption before now but using T+35 instead follows the price closer than an exponential increase over time has been able to. I used that slope and intercept from the 1-4-21 graph to predict the GME log10 price 35 days later and then plotted it with the trendline of the GME log10 price over time in this [graph](https://i.imgur.com/KwSlhTZ.png). I used an average increase of $5,500,000 per day after 7-18-21 to project until 9-1-21. Not exactly sure why the cumulative GME FTD $ follows the price 35 days later but thought I would share.

&#x200B;

[GME’s price plotted against cumulative FTD notional value](https://preview.redd.it/9w08xnpzbs971.png?width=1766&format=png&auto=webp&s=4e80f7d033a49b1945c4497ba2a6a84681a1498c)

&#x200B;

\----------------------

&#x200B;

Alright that’s all I got for today! If you want to get a hold of me, tag me in a comment.

&#x200B;

**EDIT 1:** Originally I was saying break the shorted ETF and "sell" the underlying back to the market. But some people have corrected me in the comments. They actually buy to cover the underlying they don't want to short.

&#x200B;

pce\~\~

\- u/dentisttft

&#x200B;

My Twitter has some random daily thoughts/price predictions that don’t require a full post.

![https://twitter.com/dentisttft](https://twitter.com/dentisttft)

&#x200B;

*PS. I’d love to look into the XSVM stuff more, but if someone wants to get to it before me then go ahead. I have one more post planned for this next week that pulls everything I’ve been posting about together. I personally think the MOASS is right around the corner and I’m going to do my best to prove why that’s the case.*

*Oh yeah, XRT has been on the threshold list for a while now. I don’t know if that means anything. It hasn’t so far… but I’m sure it will come into play eventually.*