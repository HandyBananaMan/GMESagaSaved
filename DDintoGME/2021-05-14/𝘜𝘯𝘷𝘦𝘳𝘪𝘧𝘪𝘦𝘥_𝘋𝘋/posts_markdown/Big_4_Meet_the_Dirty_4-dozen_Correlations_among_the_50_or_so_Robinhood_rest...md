# Author: eightesix
# Post URL: [https://www.reddit.com/r/DDintoGME/comments/ncfmtp/big_4_meet_the_dirty_4dozen_correlations_among/](https://www.reddit.com/r/DDintoGME/comments/ncfmtp/big_4_meet_the_dirty_4dozen_correlations_among/)


**TL/DR:**

**(NOT FINANCIAL ADVICE) This is an analysis of correlations between GME and the 4-dozen or so other Robinhood-restricted stocks.  There are very strong correlations among these, which are changing over time.  Currently (month of May up to May 11), GME is inversely correlated with AMC.  GME's correlations with the other restricted stocks during March 2020 appear anomalous.**

&#x200B;

&#x200B;

**In The Beginning**

Apes and apettes.

Before I offer up some tasty DD to go with those crispy, tender tendies that you've been waiting so patiently for, I have to get something off my chest. See, I am very, very late to this party. A few weeks ago, I was skeptical there even was a party. So I joined Reddit, took a deep dive, and then another, and then another, and then another, and well, you know.

&#x200B;

https://preview.redd.it/ihc1jfafd4z61.jpg?width=251&format=pjpg&auto=webp&s=da55ab3110467c68b6d76f68b281b8ea84ad4a00

But I know what you're probably thinking.  Shill.  Fucking shill.  Late to the party, fake as fuck, full of shit.  This guy:

&#x200B;

https://preview.redd.it/bq5zgzujr4z61.jpg?width=615&format=pjpg&auto=webp&s=52a9a30558710de9ad7ef71ee01cd55ce30a9117

But don't worry apes and apettes.  I am actually a sophisticated sex robot sent back through time to change the future and jack the titties of one lucky shrewdness.  Wait, no.  Sorry.  That's the other guy.  His name was DFuckingV, right?

Ok, Enough fucking around.  Time for the goods. See, like most of you, I’ve been spending the last while (weeks for me, months for you) staring at charts. Since I was late to the party, I had a *lot* of catching up to do, including getting up to speed on the Bulgarian Boy’s personal pump and dump machine...

Not this one:

&#x200B;

&#x200B;

&#x200B;

&#x200B;

&#x200B;

&#x200B;

&#x200B;

&#x200B;

&#x200B;

[Exhibit A: Robinhood: v.01](https://preview.redd.it/4tus6zfde4z61.jpg?width=280&format=pjpg&auto=webp&s=d6aac082161e652487e50b9656d2e7504220838c)

...and things like it.  So along these lines, one of my favorite things to do lately when I should be working has been to try to spot the obvious pump and dumps in the comments section of WeBull (not my broker, for the record) and try to figure out what makes them tick. And it’s impossible not to notice just how *similar* so many of the charts are post-January. Obviously, I'm not the only one who’s noticed this. [u/Nice-Violinist-6395](https://www.reddit.com/user/Nice-Violinist-6395/)  did a nice write up pointing this out for four of our beloved Stonk’s more well-known cling-ons, which you can find here:

![https://www.reddit.com/r/GME/comments/nay4zw/presenting\_the\_big\_four\_four\_separate\_stocks\_four/](https://www.reddit.com/r/GME/comments/nay4zw/presenting_the_big_four_four_separate_stocks_four/)

Finally, the point of all this stupidity. Violinist showed us a chart and pointed out the similarity, and I’m going to expand on that more or less by slapping some numbers (specifically, **correlation coefficients**) on that similarity for your crayon-munching pleasure.  The purpose of this is to show that, on the one hand, your eyes are most definitely not deceiving you and that the pattern is real and quantifiable.  And on the other hand, to point out that that pattern is changing somewhat over time in some very interesting ways that pertain to where we are right now in this whole saga.  And of course, there will also be a hint of *fuckery*  just to keep things spicy.

**In The Middle**

So to set the stage in more specific terms. Violinist showed us that GME’s price follows a pattern that looks eerily similar to that for KOSS, EXPR, and AMC.  Just to quickly re-hash some points that are pertinent to what you'll see in this post:

· The restricted stocks don’t follow the pattern of the market or the pattern of others in their respective industry. **(NOT ADDRESSED HERE)**

· The restricted stocks appear to follow a similar downward trajectory. (**DIRECTLY ADDRESSED HERE)**

· Relative volatility may be implicated, causing the restricted stocks to move in bunches. **(INDIRECTLY ADDRESSED HERE)**

· KOSS appears to be the most similar to GME. (**DIRECTLY ADDRESSED HERE)**

These are all things we can quantify pretty easily by calculating the **correlation coefficient** between the charts (or parts of the charts). But before we get into that, remember the golden rule: **correlation does not equal causation**. So even though the numbers here will tell a story, it’s hard to pin down exactly what the cause of the patterns might be, especially when we’re talking about a dynamic system that’s as complicated as the stock market. That said, correlations among a bunch of different components of a system can be *indicative* of some underlying deterministic process that’s causing things to move together in some way (e.g. a trading algorithm). So even if we can’t pin down causes, this is still a useful exercise to help us get to grips with what’s going on.

Ok, now that the disclaimer is out of the way, onto correlation. When we’re talking numbers, correlation measures the tendency of two paired sets of measures to vary together. I.e. do they go up at the same time? Down at the same time? Or does one go up when the other goes down? When we’re talking about time series like stock price charts, correlation’s also an accepted way of **quantitatively summarizing their similarity**. Without going much further, you should know that a correlation of 1 means that the two series are more or less identical (e.g. the correlation of something with itself is always 1), while a correlation of -1 means that they’re perfect opposites. If the correlation’s 0, then the two series are unrelated. So, with that, onto the goods.

**Methodology**

Data : Daily closing prices, downloaded from yahoo finance for the 50 or so stocks that Robinhood restricted trading on

Analysis: Correlation coefficients between GME and the other tickers, with data binned by *month*.  Doing things by month is kindof arbitrary, but I chose it because it's relatively easy to do and it still gives us a picture of how this whole similarity picture is changing over time.

**The Goods.  Lots of Goods.**

To start off, let's look at the correlation between GME and the rest of the dirty 4-dozen during the month of January.

&#x200B;

https://preview.redd.it/k7e3s8dri4z61.png?width=900&format=png&auto=webp&s=a18ce2aa4be1e559304b9310b32944ea3a3ae9f5

Remember, 1 means the two time series have the same shape. SHLS, XM, and TIRX have two datapoints for January, for the 28th and 29th, so safely ignore those (although it is weird that there’s perfect correlation for those two days). But in any case, there we have it. GME, AMC, KOSS, and EXPR. Along with INO and TR. That’s right. Tootsie Roll.  Everyone's favorite flavored crayon.

Really, this is nothing new, but now we have some numbers to put to the visual similarity that we can all see with our own eyes. One way to think about the January events is that the price action in GME was like a giant pulse that dragged the action of the others with it – coupling them together – the high levels of correlation across the board are symptomatic of this.  It's a lot like a tsunami grabbing and overtaking smaller waves as it moves along.

But a question worth asking is how (or if) this pattern changes over the course of the rest of the year. If you look at the graph below, you see that it definitely does change once we get into February. But, again, chopping things up by month is somewhat arbitrary, and doesn’t necessarily focus on any particular events or time windows that could be of potential importance. I chose monthly because it’s easy and tractable, and basically just a decent place to start with this kind of analysis. In the future I’d like to get more principled about this, and potentially tie this in with the other amazing DD out there on FTD cycles etc. But for now, I’m sticking with the monthly view.

&#x200B;

https://preview.redd.it/urwvw20gj4z61.png?width=900&format=png&auto=webp&s=1c3018ef49cb23b0d1c488ef3e3255729eefa645

The pattern changes in February, with a lot of the correlations dropping out or becoming negative. But the big four are all right there, with correlations above 0.8. Come March, we get another shift.

&#x200B;

https://preview.redd.it/wm50llvij4z61.png?width=900&format=png&auto=webp&s=64e1e19879ebb2e99a2a57fa8c656050bdcfc098

Where it’s worth pointing out that the pattern with respect to the big 4 breaks – the correlations aren’t nearly as strong at this point.

Then in April:

&#x200B;

https://preview.redd.it/jx2aznbnj4z61.png?width=900&format=png&auto=webp&s=5beda97903c704a6931e17983b6270c8bb4cdedf

A pattern similar to March, overall, but with notably stronger correlations across the entire set. And this ramps up going into May (up to the 11th, I don’t have data from the 12th onward included here).

&#x200B;

https://preview.redd.it/8r4s70ipj4z61.png?width=900&format=png&auto=webp&s=4b28fac5c661f5fc5251c2bf53a15a7429c3b622

At this point, the big 4 are NO LONGER THE BIG 4. In particular, look at AMC. The strongest negative correlation. Meaning that when AMC goes up, GME goes down, and vice versa. As I’m writing this, AMC has been threatening to take off and we’ve been seeing a lot of MSM FUD that seems to be trying to shake people off the GME rocket to get them to jump over to AMC. AMC might very well jump, but my takeaway from this is that **THIS IS REALLY IS A POTENTIAL TRAP**,  or at the very least a dynamic that can be exploited, and the numbers here show it. Remember, if AMC hurts the shorts, that’s good for GME. And if GME hurts the shorts, that’s good for AMC.  If the shorts get hurt, GME and AMC both win. The game that’s being played by the SHF is divide and conquer.

And if you haven’t had enough of the blue crayons yet, here are October, November, and December 2020. I’m not going to say anything about these, but if anyone has ideas that might be worth including or looking into, please comment or pm to let me know.

&#x200B;

https://preview.redd.it/pgsrcl5xk4z61.png?width=900&format=png&auto=webp&s=e4638e9e4c0546db01021d880c3d4ee715680432

&#x200B;

https://preview.redd.it/t6fq3yfyk4z61.png?width=900&format=png&auto=webp&s=3f5f5f1f22b5ac683483dc3ab181bb4ed6083485

&#x200B;

https://preview.redd.it/qp7yn1a0l4z61.png?width=900&format=png&auto=webp&s=44be7c6e9ba40b8d7aca22e0df394f89ae59a139

**Time Traveling.**

So to recap, the pattern is most definitely there, but it’s also changing over time, and the correlation coefficients show us that definitively.

No big surprise, maybe some interesting wrinkles here and there, but where is the promised *fuckery*.

Let’s go back in time to where this all started, when the world was in the midst of a slow burn that looked like the inevitable death of brick and mortar retail. Apes and Apettes, I present to you, February 2020.

**EDIT: Accidentally had Feb 2021 in here before.  Here's Feb 2020**

https://preview.redd.it/vpe3tdzs36z61.png?width=900&format=png&auto=webp&s=43b35df55664153cb9e64c0e07ba74bc86920791

Yeah that's not it.  Titties tingling yet?  Wait for it....

&#x200B;

https://preview.redd.it/bcj88q73m4z61.png?width=900&format=png&auto=webp&s=93742c6292835d5115a10c517d94dc11faeb3437

During the month of March, GME has a single positive correlation with AAL. And that correlation might well be insignificant (there are statistical tests for this kind of thing that I’m not going to do because it’s time consuming and I need to make sure to do some work on my *actual* job today so I don’t get fired). But for all intents and purposes, this looks like an anomaly. Especially when we look at April 2020, where things are more like what we’ve gotten used to seeing up until this point.

&#x200B;

https://preview.redd.it/m0ph1mqcm4z61.png?width=900&format=png&auto=webp&s=fc285b4d2d9aca39bb8cbbfd23e16424bc12bb63

So, what’s going on in March? Maybe everything is on fire and all the rest of these restricted stocks look like GME, and nothing's correlated because of all of the chaos? Nope. Look at the correlation matrix, which basically contains this same correlation information for all of the restricted stocks with data for March.

&#x200B;

https://preview.redd.it/yn9dlemum4z61.png?width=1000&format=png&auto=webp&s=5fa67b49abf05a4a37860d470d203e5ce7e571f3

While the rest of the market was on fire (including the other Brick and Mortars and the Big 4), GME and the basket of healthcare/pharma stocks in the mix here went sideways, while Tootsie Roll rose. The healthcare makes sense (pandemic - duh). Tootsie Roll I can see (consumer staples). But GME? While the other brick and mortars burn? This seems strange on the face of it.

Why would GME suddenly decorrelate with the rest of these and then suddenly snap back into place? Honestly, I don’t know. But I’ll throw out a couple of points for speculation. Be warned, I’m pretty smooth-brained when it comes to finance, and do not have a background in financial engineering:

1. Stability in the price action would have implications for options pricing that could potentially be exploited vis a vis the rest of the dirty 4-dozen.
2. Decorrelation with a group of targeted stocks would likely have lots of algorithmic advantages – again, not a financial engineer, but having an initial state for your system which is (largely) unaffected by external influences makes models easier to formulate. Something like that could be going on here. In statistics/machine learning there’s a transformation called ‘whitening’ that’s commonly applied to data when you feed it as input to a model. The point of whitening is to get rid of correlations among the inputs to your model, which is (in general) helpful for predicting outputs. This looks a lot like whitening.

I’m going to leave this dangling here so that others who are more qualified to speculate and/or run with this on more solid footing can do their thing.  Superstonk says I'm not old enough to party, and I'm almost old enough to ride the rollercoaster at GME but not quite.  If anyone wants to cross-post this for more visibility, go for it.