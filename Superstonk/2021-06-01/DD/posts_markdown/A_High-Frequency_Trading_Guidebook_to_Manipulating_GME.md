# Title: A High-Frequency Trading Guidebook to Manipulating GME
# Author: jsmar18
# Post URL: [https://www.reddit.com/r/Superstonk/comments/npv6wy/a_highfrequency_trading_guidebook_to_manipulating/](https://www.reddit.com/r/Superstonk/comments/npv6wy/a_highfrequency_trading_guidebook_to_manipulating/)


Your resident Analytical Ape here to not rain on a parade, for once.

NYSE Order Types are out again for the month of April! Is fuckery afoot? What’s so special about April? It’s the first month where we did not see any insane price action like in January, February and March. This can be observed below through some 1-month candles, consolidation has been much more pronounced over the past two months.

The title was low-key clickbait, you'll find out why - but we go through A LOT of methods that are applicable to HFT and how it is and can be used.

&#x200B;

![GME Monthly Candle Chart](https://preview.redd.it/oitl8n65vn271.png?width=1072&format=png&auto=webp&s=747f9800b84345cf535541840ce92d51f43b75db)

I’m trying out a new format, given market structure gets complicated. For complicated sections there will be a 🍌🦧 **Monke Speke** section and a 📈🧠 **Technical Speke** section. So for those that want the nitty gritty, stick around for the technical speke.

What’ll we go through?

* Order Type Breakdown (ISOs & ALOs) \[Skip if you’ve read my previous posts\]
* April NYSE Order Type Update
* Hidden Rates - SEC Market Structure Data
* Cancellation Ratio - SEC Market Structure Data
* Odd Lots - SEC Market Structure Data

What does the candle chart above have to do with order types? Well as always, let’s start with two key definitions, **skip ahead if you understand these based on my previous posts**.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

# Acronym List

**ALO:** Add Liquidity Only

**HFT:** High-Frequency Trading

**IOC:** Immediate or Cancel

**ISO:** Intermarket Sweep Order

**MM:** Market Maker

**NBBO:** National Best Bid and Offer

**NYSE:** New York Stock Exchange

**Reg NMS:** Regulation National Market System

**PBBO:** Protected Best Bid and Offer

**SIP:** Securities Information Processor

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

# IOC ISO (Immediate or Cancel Intermarket Sweep Order)

🍌🦧 **Monke Speke**

It fills the lowest alternate exchange price before filling the order at the higher price.

📈🧠 **Technical Speke**

[Intermarket sweep order](https://ibkr.info/article/1734)’s are generally a large quantity order that is sent to multiple exchanges.This is how it functions:

* An order is submitted in the pre market to sell at a price of 40.80 and is sent to exchange A.
* The best offer price on exchange A is 40.63.
* Exchange B receives an intermarket sweep order to buy 800 shares of the stock at a limit price of 40.88.
* The best offer price on exchange B is 40.88

*The trader that enters the intermarket sweep order would be required to fulfill their Regulation NMS requirement by executing the maximum available quantity on exchange A at 40.63 and then may execute the balance of the order on exchange B at 40.88 even though it is at a price that is inferior to the 40.80 order resting in the book on exchange A. The 40.80 price is not the inside quote and is therefore not "protected" in terms of the balance of the sweep order executing at exchange B at a price of 40.88.*

To make it more complicated this is an order with a modifier (ISO is the modifier), so let’s understand an IOC.

These are orders which attempt to execute immediately and cancel any unfilled portion. E.g. place a buy for 10 @ $180.01 , it’s only able to be filled to a portion of 5 @ $180.01 and then canceled straight away.

A key part to these types of orders is derived from the following.

"The intermarket sweep exception enables trading centers that receive sweep orders to execute those orders immediately, without waiting for better priced quotations in other markets to be updated."

This is [derived from a response](https://www.sec.gov/comments/sr-nyse-2014-32/nyse201432-2.pdf) to change how ALOs work by the NYSE, as they’ve been a thorn in their side since 2014.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

# Add Liquidity Only (ALO)

First of all, major thanks to [u/SmithEchoes](https://www.reddit.com/u/SmithEchoes/) on this bad boy as it’s a complicated beast.

🍌🦧 **Monke Speke**

These orders create sell/buy walls that have a nifty function that essentially “flips the safety switch” back to the original limit order price if too much buy/sell pressure is applied.

📈🧠 **Technical Speke**

ALO follows a strict “If,then” rule set based on if it locks [(7.31(e)(2)(b)iii-iv)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37) OR crosses [(7.31(e)(2)(b)ii)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37). This rule set forces the ALO to perform these trades until it is fully consumed, or the order is canceled. Rule [7.31(e)(2)(C)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37), once ALO is resting on the exchange AND it was forced to change its price in accordance with [7.31(e)(2)(b)i-iv](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37) THEN it now gets to be priced in accordance with [7.31(e)(1)(A)iii and iv](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37). This is the equivalent of HFT when ALO “activates” BUT it comes with a built in safety feature that IF the price goes UP(Sell ALO) or DOWN (buy ALO) the ALO limit price is no longer locking or crossing at the values it was getting moved to, it REVERTS back to its original limit order price.

The “repricing behaviour” which we refer to as the safety switch above also has time priority because the repricing or follow up action is handled on the exchange side (instead of canceling and resubmitting at the back of the queue as an example). So yeah, it can get “ahead” due to this exchange side handling. Ripe for misuse all round.

Funnily enough, the NYSE has tried to [amend how ALO orders work](https://www.federalregister.gov/documents/2014/10/16/2014-24547/self-regulatory-organizations-new-york-stock-exchange-llc-nyse-mkt-inc-order-approving-proposed-rule), because of how they can be used for nefarious purposes…. \*cough\* Citadel \*cough\* The amendment would force to cancel the ALO once it crosses or locks, and not perform how it currently does in accordance with [7.31(e)(2)(b)i-v](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37). Which means no buy/sell wall capability for them to use and abuse.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

# STOP SCROLLING HERE

# NYSE Order Type Data

&#x200B;

![NYSE Chicago Order Type Data](https://preview.redd.it/frriegpevn271.png?width=1081&format=png&auto=webp&s=75bb3cf585fd2f3b13cc2dcbb3b4c1090755e729)

**Assumption:** As usual, this is the NYSE Chicago exchange, I focus on this exchange as it has the least volume and it’s easier to see how order type behaviors move. I also hypothesise that it’s one of Citadel’s and others stomping grounds for GME as well given we saw an adverse change in October which is when Retail interest really started to lift dramatically.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

# April ALO Orders

Let’s take a step back to the candle chart above, what we can see is consolidation as the months move on from January, April-2021 was really the first month that we did not see any insane price movements. This also coincides with a huge drop in ALO order % from 16% in March to 9% in April.

Using what we know of ALO orders, it suggests that there has been fewer and fewer reasons to use ALO orders to create various walls to try and contain buy/sell pressure. I hypothesise that this may mean that at this price range, retail buy power diminishes significantly and we’ve entered a more cyclical phase of purchasing shares (I know i’ve been purchasing the same amount every paycheck since January).

**Conclusion:** Liquidity is drying up, retail is entering a (likely) cyclical purchasing cycle, the current price point is likely the optimal price to retain GMEs price at (so not to spur buying) - therefore ALO dependence has decreased drastically.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

# April ISO Orders

I have not historically given IOC ISOs much love, given they represent 40% of order types on NYSE Chicago, kinda unfair!

&#x200B;

![NYSE Chicago Order Type Data](https://preview.redd.it/ypmc8c6kvn271.png?width=1098&format=png&auto=webp&s=0314e6ffdec6a6dd6c56918a1d72114fd15d801c)

These orders have had their fare of flack, causing stock prices to crash previously due to the [imbalance they cause](https://www.wsj.com/articles/BL-MB-21819). Possibly a correlation with [higher information share](https://sci-hub.se/https://www.researchgate.net/publication/306222250_Clean_sweep_Informed_trading_through_intermarket_sweep_orders) than non ISOs which results in them being preferenced.

To start to unwrap this, the first thing we need to understand is that there are exemptions to [rule 611](https://www.sec.gov/spotlight/emsac/memo-rule-611-regulation-nms.pdf). ISO orders in particular are exempt from Reg NMS in regards to protecting the NBBO. Hold on a sec while I explain an example.

**Normal NMS Scenario:** I want to buy stock at $180.01, but I can’t until displayed liquidity is exhausted at $180.00.

**ISO NMS Scenario:** I want to buy stock at $180.01, I place the ISO order and it this tells the exchange that I've already checked availability on other exchanges for $180.00 - woo! Order filled!

So what this implies is and from the huge increase above on NYSE Chicago (for reference compare it to the \~20% of NYSE Arca), a HFT would have decided which way a market is going, and then get in line first.

&#x200B;

![NYSE Arca Order Type Data](https://preview.redd.it/pwuz981nvn271.png?width=946&format=png&auto=webp&s=1e5ee275df5470b09a9f7b19040c1ac7fe774573)

**Conclusion:** Given NYSE Chicago sits at 20% above Arca and there was also a 20% shift upwards from Sep-20 to Oct-20, when GME started to gain retail attention - i’m going to sit on the side of the fence, which is HFTs are using IOC ISOs for more nefarious purposes.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

# Hidden Rate

Switching over to another data source, [SEC Market Structure Data](https://www.sec.gov/marketstructure/market-structure-analytics). Before we get into data, consume this cool graphic. Since it’s much more fun than a written explanation.

![Sorry, can't find the source, from a news site back in the days](https://preview.redd.it/v5uhhzavvn271.png?width=637&format=png&auto=webp&s=b5a23010a1caad91550fc6382cd78063d52cba53)

And here is a written version

HFTs can effectively jump the line by posting [“hide not slide”](https://docs.google.com/document/d/1QmoFpdq9HeGJ-cdPP7y808uWxVufJNr2b69J0GY_-SQ/edit?usp=sharing) orders instead of visible orders. This is because a hidden order will not be slidden, resetting the timestamp. So if I placed an order at $120.01 for GME, they then place a hidden order for $120.01 as well from another exchange, I get my timestamp reset due to the market now being locked, but the hidden order does not get their timestamp reset therefore essentially skipping the fucking line. Slightly different wording to the above as I’m introducing timestamps, which is the actual function and how it works.

Now for some data. What we’re looking at is the hidden rate across all exchanges on a daily grain for four different stocks.

&#x200B;

![SEC Hidden Rate Data](https://preview.redd.it/b6e21nb1wn271.png?width=1063&format=png&auto=webp&s=c417fb78a68e1eb5086283405f7f06dd76b5fb9e)

Given the knowledge of hidden orders, it’s a clear indicator of non-retail trading taking place, namely by HFTs. Let’s put some commentary to each, shall we?

**TSLA:** Truly an OG meme stock in my opinion, retail interest is wide-reaching and has resulted in it’s rally, so there’s no surprise that HFTs are active in this stock to take advantage of that fact.

**AMC:** Sensitive topic, judge it for yourself.

**AAPL:** Retail probably have a small part in this stock, Avg volume is 103M, so it’s more likely institutional trading that represents the highest %, as a result of a generally, much lower hidden rate - as and this is an assumption, hide and slide orders are perhaps not the most useful quant strategy for this particular stock.

**GME:** I think the chart says it all. \~15% up until January, it has remained high ever since, which is an indication that GME is still of interest to HFTs. I believe this is still the case heading into April at least given hidden order % is still being high in April within the NYSE Chicago data.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

# Cancellation Ratio

HFTs are responsible for the majority of cancellations, market makers (MM) specifically. Let’s go through a simplified example of how this works.

Citadel places a buy order on an exchange for 100 shares of GME at $179.99. They also place a sell order of 100 shares at $180.01. You, a lowly retail trader, comes along and can sell immediately to the market maker for $179.99 or buy it for $180.01. Another lowly retail trader comes along on the other side of that trade and the market maker collects $0.02 as the middle man.

Where do cancellations play into this? Market makers need to decide what orders to send and at what price. Based on their algos, they’ll aim to balance supply and demand.

So if someone buys at $180.01, that means their sell order has executed and they might be looking to move up ask, therefore the MM cancels their buy order. Say this happens again, but flip the scenario around, another cancellation ensues. Repeat this thousands of times and you’re gonna end up with a lot of cancellations while the MM is managing supply and demand.

This means that the ratio of cancellations to lit trades is always going to be at least one. Factor in that this happens across many many exchanges, say there are 10 exchanges, 10 sells and 10 buys are placed. If someone buys at $180.01 on **one** exchange, the MM raises all the buys and sells on each of the exchanges and cancels the rest.

As you can imagine, it’s not odd to have a cancel to trade ratio of >10.

&#x200B;

![SEC Cancel to Trade Data](https://preview.redd.it/y96mehp6wn271.png?width=1077&format=png&auto=webp&s=17f8c65ba7a23267f1dfdd4249d4a89b41a82b55)

This is visualised above, through four tickers, all ratios are well above 1 and often sit above a cancel to trade ratio of 10.

The odd bunch of the pack is GME. AMC and GME dipped low during the late January retail hype, however GME has remained low ever since in comparison to AMC (draw your own conclusions on that point, i don’t really follow AMC).

**Why the low cancel to trade ratio?**

&#x200B;

![&#37; of Total Lit Volume by Exchange \(exchanges greyed ou](https://preview.redd.it/8b30waw9wn271.png?width=1084&format=png&auto=webp&s=2c3e491a083f761d3028a684d86b8a08d5f0cf6e)

The chart above is looking at the exchange's % share when it comes to GMEs weekly lit volume. The main trend we can see is that Edge-X has been increasing since retail hype sparked in September-2020. Thanking u/dlauer here, as he put forward reasoning that suggests orders are being routed through Edge-X due to the rebates given on that particular exchange. MMs not only make money off the spread, they also look to make money through rebates.

So this suggests that retail interest is obviously still high and MMs are taking advantage of it through getting some dough back on rebates.

What does this have to do with the cancel ratio though?

It shows retail is still active, us retail traders don’t cancel orders and adjust constantly to a moving market, we place a limit buy and bob’s your uncle (assuming it executes). This naturally means less cancellations as a result. This correlation is on display when you compare Edge-X market share to GMEs cancel ratio in the two graphs above, pretty much mirror images of one another.

I open it up to your thoughts on your interpretation, especially given AMCs rise again in cancel ratio while showing a similar exchange distribution to GME.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

# Odd Lots

**Why are odd lots important?**

Well, “lucky” for you, I'm gonna educate you on some Reg NMS stuff before we even get to that. Let’s start off with some definitions.

[NBBO](https://www.investopedia.com/terms/n/nbbo.asp): A quote that shows the highest bid price and lowest ask price.

[PBBO](https://www.investopedia.com/terms/o/order-protection-rule.asp): The rule is meant to ensure that investors receive an execution price that is equivalent to what is being quoted on any other exchange where the security is traded. The rule eliminates the possibility of orders being traded through, which means executed at a suboptimal price.

**Why should I care about the NBBO though?**

Eh, you should, but we all HODL, so it’s not that much of a biggie. It’s still good to understand though as it does have a direct effect on the cost to trade. When you are looking to place a trade for GME, the SIP shows you the NBBO. The quote thingy that flashes on your screen with numbers flicking back and forth.

This should be the best bid and ask regardless of which exchange they are chilling in. BUT it needs to be for a round lot, 100 shares. These round lots are also protected as well, e.g. you won’t get fucked over by worse prices to trade at other exchanges.

At this point you should be asking yourself, when did I last place a trade that reached 100 shares?

If you’re like me, not once - Auspoor here after all. What I'm alluding to is that investors/brokers using the SIP won’t actually know there are us fishies swimming around at slightly better prices in the market due to the majority of our orders being odd lots as we as retail traders have far less capacity to order huge quantities of GME to qualify as even lots (100 shares) (I wish I kept on hand the chart that showed low average trades, if you got it PM me).

&#x200B;

![NASDAQ Response to Reg NMS II](https://preview.redd.it/9z6co24oxn271.png?width=1051&format=png&auto=webp&s=6b453abd61c15b01cd27b58daea7db442f9e9a1e)

For reference, take this picture above, it’s an example that shows investors can be protected at the NBBO thanks to even lots, but odd lots can exist at better prices.

The SEC adopted a new rule to change how this is applied to the NBBO and PBBO, but it’s only applicable to securities with a price greater than $250. They did however mandate that the exchanges must publish all odd lot prices to the SIP, as long as they are better than the NBBO. This is highlighted below.

&#x200B;

![https:\/\/www.sec.gov\/news\/press-release\/2020-311](https://preview.redd.it/qoudtqlrxn271.png?width=683&format=png&auto=webp&s=48d60f9df9b831bd0eb5f4e153d4642287827cea)

**What does this mean?**

I interpret it as better price discovery as a result of the odd lot inclusions into the SIP specifically.

**What does this mean for retail?**

Not really that much. These small incremental differences don’t matter all that much for retail traders placing smaller orders and HODLing GME in my eyes.

**HFT and Odd Lots**

HFTs use odd lots in a myriad of ways, [order shredding](https://www.jstor.org/stable/43612955?seq=1) is pretty typical when it comes to algo trading, splitting larger orders into smaller orders, using odd lots to test how reactive a ticker is, pinging dark pools to find larger orders, hiding a large order within small odd lot orders etc… So they are useful to a HFT.

I think we all know why dark pools exist, so larger institutions can place large block orders without affecting a stock's price. The logic we can work out from this (and is [quoted here as well](https://blog.themistrading.com/2011/08/odd-lots-another-weapon-in-the-hft-arsenal/)) is that larger orders have a larger impact on prices than smaller odd lot orders.

We’ll touch on the hypothesis of how this could play out below in relation to GME.

**To the chart… Finally...**

The main thing to note is a stock’s price is a large driver in odd lot rate. This explains 80% of what we can interpret below, along with retail interest.

&#x200B;

![SEC Odd Lot Rate Data](https://preview.redd.it/vhhw2n7vxn271.png?width=860&format=png&auto=webp&s=9f5e0aa7b81dbad8f7194bbace92709399e34780)

**GME:** 80-90% odd lot rate since January shows a great deal of retail interest still exists (whether buy or sell, but going from fidelity, it’s most defs buy).

As mentioned above, HFT's use odd lots. The odd thing is that in February, we saw GME trade between \~$40-$50, with that - I'd expect to see the odd-lot rate drop-down much further than it was currently trading at.

Using the logic we worked through above, I hypothesise it may be as a result of HFT activity, order splitting retail orders further, which can have an adverse impact on a stock’s price (remember this was the time when they really wanted to convince us they covered and has been happening ever since). Saying that, i have no doubt that retail was still actively buying in Feb (I sure was).

**TSLA:** HFT is associated with odd lots to take advantage of the whole NBBO situation, so no surprise it’s consistently at \~90% along with the fact TSLA is what I view as an O.G. meme stock, so naturally, lots of retail placing odd lot trades due to the high share price.

**AMC:** Given it has returned back to its lows of 30% in July 2020, I'm scratching my head a bit. This returning back to its average AND cancel ratio doing the same is saying something, but i don’t want pitchforks aimed at me, so draw your own conclusions.

**AAPL:** Makes sense the odd lot rate sits below GME since the squeeze as stock price is around that \~$100 mark, so relatively expensive, but lesser in comparison to GME.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

# Conclusion

That was fun, wasn’t it?

What to make of all of this?

Your main takeaway should be that MMs who are HFTs use whatever tools available to them to make money. They have more data than us, with much greater fidelity (no, not the broker). There’s not one data point in this analysis that does not indicate that GME has radically changed in how MMs treat the stock and that retail interest has obviously not subsided, in fact it remains ever so pronounced (odd lots being the main data point there).

Nothing forward-looking sadly, but I guess I can leave you my thoughts for next month in terms of how I believe the data may change over May (yes, still the past, but still the future in relation to the data we got 😉).

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

# Predictions (not the bad kind)

**NYSE Order Type Data**

ISOs remain at the same % distribution, no reason for that to decrease, more likely to increase as I believe ALO will continue to decrease as May enters further consolidation compared to April - sweet point hit. Saying that, the run up the last week of May might throw that off, but hey - who knows.

**Hidden Rate, Cancel Ratio, Odd Lot Rate**

I don’t think these will change heading into May, for the most part, the reasons why they are now for GME since January are the same now, so until the squeeze, these should remain at their relevant positions. Will be interesting to see if they heavily deviate like AMC did back to it’s pre-retail hype average - don’t think it will, but interested if it does nonetheless.

See you next month for the May update (and in July if we are not on andromeda already for an SEC Market Structure update)

&#x200B;

**Edit:** Changed title to bold