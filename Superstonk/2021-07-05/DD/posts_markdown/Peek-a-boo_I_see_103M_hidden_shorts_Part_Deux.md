# Author: WhatCanIMakeToday
# Post URL: [https://www.reddit.com/r/Superstonk/comments/oenvoh/peekaboo_i_see_103m_hidden_shorts_part_deux/](https://www.reddit.com/r/Superstonk/comments/oenvoh/peekaboo_i_see_103m_hidden_shorts_part_deux/)


Part Uno (you might want to read it first for background): [https://www.reddit.com/r/Superstonk/comments/odsded/peekaboo\_i\_see\_you\_79m\_hidden\_shorts/](https://www.reddit.com/r/Superstonk/comments/odsded/peekaboo_i_see_you_79m_hidden_shorts/)

I'm BAAACK!

After finding 79M hidden shorts in married puts, I asked myself "Can I do better?"  I didn't disappoint.  Don't get me wrong, I'm disappointed (yet also happy) that I found more shorts.

In Part Uno, I searched for new deep OTM Put Options that have no business being opened and found 79M shares worth of options (about 792k opened Put options) opened during the Jan GME spike.  I used a rather crude approach which was assuming worthless options are at the deepest OTM Put strike and then expanded that to strikes <= $5.  Crude, but it worked fairly well.

Here in Part Deux, I've improved on it by growing a wrinkle about options greeks.  

Using the same GME Options Data set I bought for about $21 from [https://www.historicaloptiondata.com/](https://www.historicaloptiondata.com/) for 2021 up to end of June, I did the following:

1. Filtered the data set down to get two snapshots in time: Jan 19th, 2021 and Feb 1st, 2021.  This is effectively bracketing the week before and week of the huge GME Jan spike.  Whatever happens in here *should* 100% be tied to that crazy spike.  (I just realized I'm undercounting a bit because the spike, T, was Jan 28th and Feb 1 is only T+2.  I'm too lazy to rerun the process right now to expand out and you'll get the picture.)
2. Filtered out only for Puts (duh) because we're looking for Married Puts.
3. (NEW for Part Deux!) Filtered by *delta* which is an option greek that represents how much the option value changes per $1 change in the underlying stock price.  I filtered for *delta* < 0.01 which means if the stock price moves by $1, the price of these options moves by a penny ($0.01) or less.  These options are *literally* **worthless**.  
Grow wrinkles about option greeks here: [https://www.investopedia.com/terms/g/greeks.asp](https://www.investopedia.com/terms/g/greeks.asp)
4. Summed up the total Open Interest for all remaining Puts.

Total Open Interest for Puts with delta <= 0.01:

|As of Jan 19, 2021|As of Feb 1, 2021|
|:-|:-|
|58,970|1,096,066|

*Wut mean?*  Over 1M **worthless** junk put options were opened in the 2 weeks (from Jan 19th to Feb 1st, 10 trading days) of our January spike.  **1,037,096 worthless put options were opened.**  Sink that in because those brand spanking, newly opened, absolutely worthless options are capable of hiding over **103,700,000 (103M) shares**.

Updates:
1) Why worthless puts?  See https://www.reddit.com/r/GME/comments/mgj0j1/the_naked_shorting_scam_revealed_lending_of/
2) The prior 79M is a subset of this 103M.  This approach is a more accurate way to count worthless options.