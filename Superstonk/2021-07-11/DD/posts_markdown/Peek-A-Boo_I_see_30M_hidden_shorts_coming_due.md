# Title: Peek-A-Boo! I see 30M+ hidden shorts coming due!
# Author: WhatCanIMakeToday
# Post URL: [https://www.reddit.com/r/Superstonk/comments/oiemiu/peekaboo_i_see_30m_hidden_shorts_coming_due/](https://www.reddit.com/r/Superstonk/comments/oiemiu/peekaboo_i_see_30m_hidden_shorts_coming_due/)


**Question:** How many of the upcoming July 16 options expiring this Friday are worthless deep OTM puts used to kick cans down the road?

**Answer:** At least **302k options**, capable of hiding up to **30.2M shares** are coming due this Friday, July 16th.

Let's walk through the analysis and show off some Google Sheets spreadsheet magic.

In order to answer the question, we need to (a) determine that an option opened up is worthless, which means we also need to know (b) when options were opened to know the *delta* for those options.

**Why** ***delta?***  Delta is an option greek that represents the change in price of an option based on a change in price of the underlying stock.  ([Grow a wrinkle here](https://www.investopedia.com/terms/g/greeks.asp).) If delta is close to 1, that means when the underlying price of GME moves by $1 then the price of the option moves by about $1. On the other end of the spectrum, if delta is close to 0, then that means when the underlying price of GME moves by $1, the price of the option doesn't move. If the option price isn't moving with the stock, it's probably not very valuable.

**Delta <= 0.01.** I'm setting the threshold criteria for |delta| <= 0.01 to determine an option is worthless.  Basically, if the price of GME moves by $1, the option price moves by less than a penny (if at all).  As there's no reasonable reason to trade these near-zero delta options, it stands to reason that all of them are being used for nefarious can kicking purposes. (FWIW, using bigger values of delta didn't really add too much to the count so I'm running with the penny threshold.  You can see the other delta calculations in my Google Sheet.)

Making use of my trusty $21 data set for all of GME option history for 2021 up to June 30, I filtered out all of the puts expiring July 16th.  (Why puts?  Because SuperStonk has been discussing using *married puts* to hide short interest or straight up naked short shares. For more background, see my previous post: [Peek-a-boo! I see 103M hidden shorts! (Part Deux)](https://www.reddit.com/r/Superstonk/comments/oenvoh/peekaboo_i_see_103m_hidden_shorts_part_deux/).)

Loaded those July 16th puts into Google Sheets [here](https://docs.google.com/spreadsheets/d/12U7I2bMKZ3nYchNsCZGsl8fYlj8PhMVAvFYhXiWjWYQ/edit#gid=2112568586) and then worked some Sheets magic.  Basically, I calculated the daily change in each option's Open Interest for all of the puts expiring this Friday, July 16th. Then, by adding up the change in Open Interest each day for options that have a |delta| <= 0.01, we find **302,464 Worthless Put Options** were opened up in 2021 up to June 30th.  The really neat bit is we can see exactly which days those worthless puts were opened.  Here's a chart:

![Daily Open Interest Change for Worthless \(delta \< 0.01\) July 16 Puts](https://preview.redd.it/ujgxmw2gvna71.png?width=4242&format=png&auto=webp&s=f6669b9c1d4b01a9357d4ef4b14f17194cc84926)

Notice an interesting date there? Jan 28 there's a gigantic spike.  We also see spikes near other major options expirations in March and June.  (See my other post [Peek-A-Boo! I Track You Kicked Cans!](https://www.reddit.com/r/Superstonk/comments/of1zn4/peekaboo_i_track_you_kicked_cans/) if you want to follow up on those.)

**tl;dr:** This chart shows *exactly* when SHFs were opening up worthless July 16th Puts that line up with the original GME squeeze in January.  SHFs have been kicking these cans down the road ever since and *at least* 302k married puts are coming due this Friday, July 16th. Those 302k puts are equivalent to **30.2M shares,** which is a pretty big deal as that is more than the free tradable float coming due.  Also, considering this is *just one approach* Kenny's been using to kick cans down the road, we're looking at interesting times coming with a few possible catalysts happening soon.

One last thing: keep in mind this analysis finds *at least* 30.2M shares from these 302k married puts that are worthless.  u/NatesAnApe posted a few days ago in [This should be all the confirmation bias you need to set your phone down and relax on this fine Wednesday afternoon. HODL tight apes ????????????????](https://www.reddit.com/r/Superstonk/comments/ofmqeo/this_should_be_all_the_confirmation_bias_you_need/) that up to 42.9M shares may be coming due (if you assume *all* 429k expiring OTM options are hiding shares to get an upper bound).

EDITS:

\- Fix typo.  credit u/Sufficient-Bowler741 & u/Froggy__2