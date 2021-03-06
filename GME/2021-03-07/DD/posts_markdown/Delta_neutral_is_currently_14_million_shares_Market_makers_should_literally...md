# Title: Delta neutral is currently 14 million shares! Market makers should literally own half of actively traded shares right now
# Author: kmoney41
# Post URL: [https://www.reddit.com/r/GME/comments/lzv4k4/delta_neutral_is_currently_14_million_shares/](https://www.reddit.com/r/GME/comments/lzv4k4/delta_neutral_is_currently_14_million_shares/)


Delta neutral is currently 14,384,617 to be precise. If market makers account for the vast majority of written contracts, that means they could own nearly 50% of the actively traded float RIGHT FUCKING NOW. This makes my confirmation bias rock hard.

The important bit upfront for all you hyper-rational investors: market makers are an unaccounted for metric in all your Bloomberg terminals and 13F filings and your shitty Morningstar data. The fact that they should own half of actively traded shares right now gives retail an insane amount of power to move the markets that people might not even realize. In other words, it's safe to say that liquidity is dryer than my wife when her boyfriend's not around.

So how did I come to this conclusion? One thing that sucks about being a retail investor is that figuring out the state of the market is like reading goddamn tea leaves. So I took it upon myself to help give people one more piece of information; I wrote a script to pull the numbers for all option contracts.

u/boneywankenobi recently made [an excellent post](https://www.reddit.com/r/GME/comments/lzj00a/super_conservative_calculation_puts_gme_short/) that corroborates this 14 million number that you should absolutely read.

The math isn't crazy. I'm taking the current delta of each option (both puts and calls) and using shares (which have a delta of 1) to offset the net delta to 0. So, if an option's delta is .03, then the MM would have to buy 3 shares to delta hedge against it. If its delta is -.03 (puts are negative), the MM needs -3 shares. I'm using Tradier sandbox data, which appears to be accurate but just not realtime.

**Caveat**

This assumes that all options were written by MMs. So, if anyone can find hard sources on this question, that could help make this estimate more realistic:

What percentage of options are generally written by market makers? In essence, I want to know what percentage of these are likely to have been written with the intention of being delta neutral? Are there estimates out there for how much retail tends to write covered calls, for instance?

Calls could also be written by hedge funds that aren't staying delta neutral. If that's the case, they're essentially in an undisclosed short position.

**Extra credit**

For the fucking nerds out there, I went a little further and decided to figure out how price changes would affect MMs given the current greeks. Things to note with this data: This doesn't take into account anything to do with theta or other time decay or volatility greeks. It also doesn't take into account any third-order derivatives. I just used delta and gamma at each $1 increase in the price of the stock.

The interesting conclusion: If GME were at **\~$330** a share right now, MMs would need to be holding **\~30 million shares** to be delta neutral. That's the whole fucking traded float just to hedge.

Another piece of extra credit on leverage: Curious which options currently have the most leverage? Here are the biggest hitters at each expiration

|expiration|description|leverage|
|:-|:-|:-|
|2021-03-12|GME Mar 12 2021 $250.00 Call|6.05|
|2021-03-19|GME Mar 19 2021 $280.00 Call|3.53|
|2021-03-26|GME Mar 26 2021 $285.00 Call|2.62|
|2021-04-01|GME Apr 1 2021 $300.00 Call|2.40|
|2021-04-09|GME Apr 9 2021 $360.00 Call|2.29|
|2021-04-16|GME Apr 16 2021 $800.00 Call|2.39|
|2021-04-23|GME Apr 23 2021 $290.00 Call|1.99|
|2021-07-16|GME Jul 16 2021 $800.00 Call|1.79|
|2021-10-15|GME Oct 15 2021 $360.00 Call|1.51|
|2021-11-19|GME Nov 19 2021 $800.00 Call|1.73|
|2022-01-21|GME Jan 21 2022 $800.00 Call|1.67|
|2023-01-20|GME Jan 20 2023 $500.00 Call|1.46|

Here are the smallest hitters:

|expiration|description|leverage|
|:-|:-|:-|
|2021-03-12|GME Mar 12 2021 $780.00 Call|0.27|
|2021-03-19|GME Mar 19 2021 $1.00 Call|0.98|
|2021-03-26|GME Mar 26 2021 $5.00 Call|1.03|
|2021-04-01|GME Apr 1 2021 $5.00 Call|1.03|
|2021-04-09|GME Apr 9 2021 $5.00 Call|1.03|
|2021-04-16|GME Apr 16 2021 $0.50 Call|0.99|
|2021-04-23|GME Apr 23 2021 $5.00 Call|1.03|
|2021-07-16|GME Jul 16 2021 $0.50 Call|0.97|
|2021-10-15|GME Oct 15 2021 $1.00 Call|0.97|
|2021-11-19|GME Nov 19 2021 $3.00 Call|1.00|
|2022-01-21|GME Jan 21 2022 $0.50 Call|0.98|
|2023-01-20|GME Jan 20 2023 $2.00 Call|0.96|

What the fuck is leverage? This is an indication of how much your buying pressure is amplified by a market maker having to hedge against the option you bought. In other words, if you bought a 03/12 $250c, your money would be having 6 times the impact than just buying shares outright.

Interesting notes: a lot of these expirations have no calls with less leverage than buying shares (any of the expirations that show leverage > 1 for the smallest hitters). Another important note: your shitty 03/12 $780c are doing fuck all to put pressure on this stock. You'd literally be 3 times as effective buying shares. This goes for all your deep OTM FD calls. Fuck right off with that shit.

Disclaimer: I'm not saying buy calls, that shit is riskier than buying shares if you don't know what the fuck is going on. In fact, I'm not saying you should do jack shit with this data. Just read it and move on with your life. Buy GME if you like the stock. Sell GME if you don't (if nothing else, it'll help [this poor fucker](https://www.reddit.com/r/wallstreetbets/comments/loio0b/i_am_going_to_buy_gamestop_all_of_it_dont_upvote/) out).

EDIT - to make something clear: For a price increase, there would need to be a balance of calls and shares being bought. It's totally possible that Citadel (big MM at play here) is just writing totally naked options and disregarding delta neutrality because they realize they're fucked either way. Either the price doesn't go up naturally and they win big or it does and they go bankrupt regardless of whether they'd written the contracts or not (because of their short positions).

This theory is implied by the DTCC's recent rule change (but, again, just a theory): [https://www.reddit.com/r/GME/comments/lzebps/new\_rules\_imposed\_by\_dtcc\_signed\_yesterday/](https://www.reddit.com/r/GME/comments/lzebps/new_rules_imposed_by_dtcc_signed_yesterday/)

If that's the case, then buying shares could actually have more pressure since they may not be delta hedging at all. In this case, those leverage numbers would be near meaningless.