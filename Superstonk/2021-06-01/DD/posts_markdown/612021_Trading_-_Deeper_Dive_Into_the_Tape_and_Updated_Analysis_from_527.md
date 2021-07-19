# Title: 6/1/2021 Trading - Deeper Dive Into the Tape and Updated Analysis from 5/27
# Author: myplayprofile
# Post URL: [https://www.reddit.com/r/Superstonk/comments/nq5xf8/612021_trading_deeper_dive_into_the_tape_and/](https://www.reddit.com/r/Superstonk/comments/nq5xf8/612021_trading_deeper_dive_into_the_tape_and/)


The correlation between the movies and GME continues to breakdown. I originally posted on 5/27 taking a look into this, and have made an update to the models since then. I've copied the original analysis and included the original post at the end. This does mention the movies, but is very much a GME story, and in no way is financial advice. My 🧠 is smooth.

&#x200B;

Since the 5/26 close, AMC has significantly outperformed GME and other "meme" stonks, so much so that the cross asset correlation between these stonks has begun to break down in a critical way that will cause institutional risk management reassessment. As of 5/26, AMC price movements were strongly correlated to GME, making the year to date R^(2) value between the two 76%. In 🦍 speak, statistically a price change in GME was 76% dependent on a similar change in AMC, and vice versa. Over the last 3 trading days, that R^(2) value has decreased nearly 20% to 62.5%.

&#x200B;

![6\/1 Update - Plot of AMC and GME closing prices - R\(square\)= .625](https://preview.redd.it/0hl7n1nazp271.png?width=726&format=png&auto=webp&s=51b088cc255891714c87fa7dfe76e2ccb30177fe)

This is a massive decrease in the strong correlation that has held all year over the last three trading days and will have lasting implications to HF risk management, especially a fund that is short GME. I will touch on Kenny/Shitadel in a bit, but it is important to understand they are not the only fund short GME, and after 3 straight days of the correlation between the two stonks breaking down, **any fund using AMC as a hedge against a GME short will now have to either reduce their short GME exposure by 20%, increase AMC long by 20%, or some combination of the 2 to avoid blowing out their VaR (Value at Risk).** It's important to realize, this type of risk management adjustment is more applicable to HF that take positions for short to intermediate/long term trades, and not to high frequency trading shops that take positions for microseconds at a time, such as 💩a🔔 and other MM with HFT algos.

&#x200B;

Now, what has caught my attention over the last few days is the impact of after hours/pre market moves that have contributed to the outperformance of AMC over GME, and during regular trading hours the algos are still very much tuned to maintain almost a tick for tick movement in AMC and GME. Even more interesting, **AMC seemed to lead each area I have circled in pink below** \-

![6\/1 Minute Candles of GME & AMC, Pink Circles Highlight Algo Control](https://preview.redd.it/cik94qa63q271.png?width=762&format=png&auto=webp&s=ced056a2917d50aa727edec577ad81088e6127b8)

So, what does this mean? There is clear evidence in the tape that market makers, aka SHITADEL, are still VERY interested in maintaining the trading correlation between the two securities. I believe this is a primary function of the legacy correlation between the 2 stonks that held up until last week combined with AMC's massive volume compared to GME and the fact the HFT algo's can sniff out incoming GME price spikes because they handle 50% of all retail orders. They use that info to front run AMC higher to remain indirectly hedged against their GME short to keep Marge from picking up her 🍌 phone that has 💩a🔔 on speed dial. Also, I think the reason the MSM has been ALL OVER the AMC rally and continues to pump the story is to keep GME FOMO somewhat at bay.

&#x200B;

However, because the cross asset correlation between the two stonks has broken down for several days now, I anticipate this strategy is also going to break down soon as other HFs will now need to begin to either cover more GME shorts or buy more AMC, putting more pressure on the algos and making it more difficult to keep the tick for tick movements between the two. I think 💩a🔔 has become net long AMC, but given the 5 million put options they hold, once their HFT algo senses the bids under AMC are drying up they will dump their long positions quickly to cause a crash similar to GME on 3/10 to turn net short and try to bring their puts back into the money. Plus, remaining long AMC at these levels is a bit dicey since they can easily sell even more stock (8 million+ shares last Fri) to take advantage of the recent price rise. Again, not financial advice, and I in no way mean to cause any hard feelings towards 🦍 that like movies.

&#x200B;

EDIT1: Forgot to include chart of GME modeled price using AMC price input. Notice the recent extreme divergence -

&#x200B;

![Actual GME Price Shown by Solid Black, Modeled Price in Dashed Blue;    GME\(model\)=\(AMC\)\*11.751+29.3](https://preview.redd.it/jii3dzxicq271.png?width=748&format=png&auto=webp&s=8da361c2175caa34112ae57bcf6460ae498add26)

&#x200B;

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

**5/27/2021 POST** [(Original Post Link)](https://www.reddit.com/r/Superstonk/comments/nmjvy7/5272021_trading_deeper_dive_into_the_tape_and/?utm_source=share&utm_medium=web2x&context=3)

Today was an important day in this saga, and will have lasting impacts on how shorts play this game moving forward. I want to congratulate anyone that was hodling their favorite movie theater stonk today, and want to make it clear this post in not intended to cause any division. I once held that stock, and have since exited that position, bought more GME, and currently hold put options on AMC as a hedge to my GME position. This is not financial advice.

I made a post about a month ago on why I believe everyone with stocks investments should own GME to hedge their portfolio you can check out [HERE](https://www.reddit.com/r/GME/comments/n1ctl5/gme_has_become_a_hedging_tool_and_should_be_owned/), but isn't necessarily required to understand this post. To give some context on why I am sharing this to everyone, I worked on a commodity trade floor for 7 years, and left that job in 2019 after my son was born. I was not a trader, but did spend over a year as a risk analyst where I kept tabs on the positions of several different trader books, reported daily profit/loss (PnL), and determined position exposure to calculate the value at risk (VaR) of those positions. Proper risk management is critical to long term trading success, and institutional traders have teams of people dedicated to tracking their position exposure and calculating the VaR generated by their positions. In simple terms, VaR is typically a 90 day lookback at price volatility and cross-asset correlations to give a 95% confidence interval on the maximum expected drawdown your portfolio may have from one day to the next. Institutions set positions limits based on these numbers and will not exceed a VaR limit unless there are extraordinary circumstances and approval from those at the top. A simple example, if two securities have a 100% correlation and you are long security A and short security B by the same amount, the VaR on the position would actually be 0 because they would perfectly offset each other. In reality, no such correlation exists, and statistics guide institutions on ways to manage risk through long and short exposures.

Now its time for the tea. It is widely accepted by 🦍 and onlookers that GME has traded highly correlated with other meme stocks, meaning when GME is up, good chance AMC and other "meme" stocks are up. How correlated? Since the start of the year - over 70%. Here is a plot of GME and AMC with closing prices I pulled from Yahoo -

&#x200B;

![Plot of AMC and GME closing prices - R\^2 = .7163](https://preview.redd.it/r5krynlkwp271.png?width=726&format=png&auto=webp&s=22f30cc851f4bd5a46ec61d9a9370dca111e596d)

&#x200B;

AMC is not the only other "meme" stock that looks like this. Here is another example of KOSS, another retailer that hasn't quite gathered the same MSM attention as AMC -

&#x200B;

![Plot of KOSS and GME Closing Prices - R\^2 = .6368](https://preview.redd.it/0pbwvaymwp271.png?width=729&format=png&auto=webp&s=27ecec85d4435b9a79ca6f7be602af99b7556747)

&#x200B;

I'll come back to KOSS soon, but for now I am going to dig a bit deeper into what's going on with AMC. From the linear fit line, you can use the AMC price point to model the price of GME. How does that look you may wonder?

&#x200B;

![Actual GME Price Shown by Solid Black, Modeled Price in Dashed Blue](https://preview.redd.it/001vwgvowp271.png?width=748&format=png&auto=webp&s=0fe8bc6c98924efe2249b4ee2bcaa864eed82b8a)

&#x200B;

This data can be interpreted in many ways, but I think the most important thing to look at is those large red bar spikes. Due to Robinhood market manipulation in Jan, I first want to highlight how in Mar the AMC spike was a precursor to the GME spike, and also an indicator that GME was due for a pullback to closer align with AMC. Now look at what has taken place this week, and specifically today.

I have a few theories into what's going on, but also note that AMC did not just outperform GME, it rocketed past all other meme stocks as well, like KOSS, BB, BBBY. This is the largest outlier move in AMC this year, on no news or fundamental reason. Why?

Now this is just theory, but if it looks like 💩, smells like 💩, and trades like 💩, then there's a good chance its Shitadel. How is 💩a🔔 involved with AMC? Well, they increased their holdings by 164% last quarter according to their 13F to 725k shares, along with a big increase in option contracts -

&#x200B;

![Citadel 13F showing 724,599 AMC shares](https://preview.redd.it/r4n1qhc5jq271.png?width=2509&format=png&auto=webp&s=37f8dde0e63e97d19d75b82bdd8ce486575ff332)

&#x200B;

Interestingly, I wanted to drill down a bit more on what the AMC-GME relationship was before Citadel became more involved with AMC, so I looked at the pricing data for this year just through Mar 31 and this is what it looks like -

&#x200B;

![Plot of AMC and GME closing prices - R\^2 = .7932](https://preview.redd.it/988uo3s3jq271.png?width=726&format=png&auto=webp&s=9cd4eb5cfb5292cc13162e9924dae9ec2b5c95fd)

&#x200B;

Now its important to remember that correlation does not necessarily mean causation, and many things have contributed to the AMC/GME price movements, but being a smooth 🧠 like I am, it sure seems like AMC and GME moved in even closer lock step with each other BEFORE Citadel became more involved. And why would Citadel want more involvement with a "dying movie theater chain on the verge of bankruptcy"? You'd have to ask Ken, but my assumption is they need a hedge to their unescapable black hole of a short on GME, and what better security to use than a low price stock caught up in the same squeeze narrative that happens to have 500 million shares outstanding and is one of the most active names traded on the brokerage app Robinhood that funnels all retail orders to them so they can use their HFT algo to rip off unsuspecting victims when Marge picks up her phone. Isn't it also interesting how the MSM keeps taking about AMC, and how the MSM outlets Citadel is invested in suddenly flipped their narrative on "meme" stocks?

Its time to start wrapping this up, so I want to highlight more of today's action. AMC significantly outperformed all meme stocks, and had a more extreme move than GME than any other day this year. There was nothing fundamental about AMC to cause this. In fact, given GME's extremely bullish fundamental news regarding NFT's, logic would dictate the opposite should be true, but it's not, and there hasn't been a day this week where GME trended above the modeled price based on AMC (1st chart). From a risk management perspective, this means the correlation is breaking down and all the VaR models across institutions will begin reflecting this starting tomorrow. It's also worth noting, GME did not significantly deviate from other meme stocks performances, so those correlations are relatively unchanged.

Me personally, as I stated above, I think GME and AMC will need to close the wide performance gap in a mean revision type trade and I hold AMC puts as both a hedge and trade. I am not saying I expect AMC to fall, or if you hold you should sell and get into GME, please don't misinterpret what I mean. I do not have any certainty why the pair trade is breaking down, just my theory stated above, but do recognize the statistical significance and wanted to share. Regardless if you're involved with GME or AMC, I don't recommend FOMOing between the two. Have a plan, own both, own one, or just enjoy the show as an onlooker. This is not financial advice.

BONUS CONTENT -

I also want to highlight Citadel's top holdings because it is very important to watch these as they continue to bleed money and approach a margin call -

* TSLA - $2.6B
* FB - $1.6B
* AMZN - $1.5B
* GOOGL - $1.5B
* AAPL - $1.4B
* MSFT - $1.1B
* XLE - $710MM

In particular, I'm watching TSLA because of the size and AMZN because it was one of Citadel's largest position increases (Added \~200k shares) and the high price/relatively low volume on AMZN makes it much easier for them in move the price where they need it to go or offer quick liquidity to raise cash.

&#x200B;

![Normal TSLA close, no way it was ramped to increase 💩a🔔AUM at close since Marge is closely monitoring positions](https://preview.redd.it/13j533d7jq271.png?width=1271&format=png&auto=webp&s=3e7b8fd0ca464feedd4baa2f2ab649bc76ca6a9c)

&#x200B;