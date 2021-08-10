# Title: 37% of NYSE Order Types "Dark" in June 2021
# Author: jsmar18
# Post URL: [https://www.reddit.com/r/Superstonk/comments/otyfcq/37_of_nyse_order_types_dark_in_june_2021/](https://www.reddit.com/r/Superstonk/comments/otyfcq/37_of_nyse_order_types_dark_in_june_2021/)


Let's go through the June update for NYSE order types, things are BAU in terms of manipulative order types being used, *but a very odd anomaly has appeared*, namely the Dark Primary Pegged order. It suddenly increased from 0% to 37% in June. Let's get into it, shall we?

Before we get started, here are the order type definitions in ape speke. If you’ve read my DD before, as usual, skip this part.

# 📚 Order Type Definitions

**IOC ISO (Immediate or Cancel Intermarket Sweep Order)**

For those who have not read my previous post find an excerpt below.

[Intermarket sweep order](https://ibkr.info/article/1734)’s are generally a large quantity order that is sent to multiple exchanges.This is how it functions:

* An order is submitted in the pre market to sell at a price of 40.80 and is sent to exchange A.
* The best offer price on exchange A is 40.63.
* Exchange B receives an intermarket sweep order to buy 800 shares of the stock at a limit price of 40.88.
* The best offer price on exchange B is 40.88

To make it more complicated this is an order with a modifier (ISO is the modifier), so let’s understand an IOC. These are orders which attempt to execute immediately and cancel any unfilled portion. E.g. place a buy for 10 @ $180.01 , it’s only able to be filled to a portion of 5 @ $180.01 and then canceled straight away.

A key part to these types of orders is derived from the following.

"The intermarket sweep exception enables trading centers that receive sweep orders to execute those orders immediately, without waiting for better priced quotations in other markets to be updated."

This is [derived from a response](https://www.sec.gov/comments/sr-nyse-2014-32/nyse201432-2.pdf) to change how ALOs work by the NYSE, as they’ve been a thorn in their side since 2014. 

In essence, these types of orders are great for HFT traders due to how they work.

&#x200B;

**Limit Non-displayed**

An order to buy or sell stock at or better than a specified price, these orders are HIDDEN from us apes and others. They also don’t care about [lock or cross situation](https://www.investopedia.com/terms/l/lockedmarket.asp) cases. Refer to my [previous post](https://www.reddit.com/r/GME/comments/mdnph0/more_proof_the_115_billion_buy_order_was_real_and/) for an understanding of this.

This means the HFT (high-frequency traders) can effectively jump the line by posting [“hide not slide”](https://docs.google.com/document/d/1QmoFpdq9HeGJ-cdPP7y808uWxVufJNr2b69J0GY_-SQ/edit?usp=sharing) orders instead of visible orders. This is because a hidden order will not be slidden, resetting the timestamp. So if I placed an order at $120.01 for GME, they then place a hidden order for $120.01 as well, I get my timestamp to reset as I’ve placed a locked/cross order, but the hidden order does not get their timestamp reset therefore essentially skipping the fucking line.

Yet another bread and butter tool when it comes to HFT. The key here though is the fact that it’s HIDDEN and how this plays out with ALO order types.

&#x200B;

**Add Liquidity Only (ALO)**

First of all, major thanks to [u/SmithEchoes](https://www.reddit.com/u/SmithEchoes/) on this bad boy as it’s a complicated beast.

Now this order type is a doozy and is currently being used for “highly questionable” purposes.

ALO follows a strict “If,then” rule set based on if it locks [(7.31(e)(2)(b)iii-iv)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37) OR crosses [(7.31(e)(2)(b)ii)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37). This ruleset forces the ALO to perform these trades until it is fully consumed, or the order is cancelled. Rule [7.31(e)(2)(C)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37), once ALO is resting on the exchange AND it was forced to change its price in accordance with [7.31(e)(2)(b)i-iv](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37) THEN it now gets to be priced in accordance with [7.31(e)(1)(A)iii and iv](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37). This is the equivalent of HFT when ALO “activates” BUT it comes with a built-in safety feature that IF the price goes UP(Sell ALO) or DOWN (buy ALO) the ALO limit price is no longer locking or crossing at the values it was getting moved to, it REVERTS back to its original limit order price.

**Monke speak translator:** These orders create sell/buy walls that have a nifty function that essentially “flips the safety switch” back to the original limit order price if too much buy/sell pressure is applied.

# June NYSE Order Type Update (Stop scrolling here)

First off, we’re focusing on NYSE Chicago exchange. Why? Because it has low volume, Citadel are based there so it’s a fair assumption that it’s likely one of their stomping grounds and the low volume makes it easy to pick up patterns in order type behavior compared to other higher volume exchange locations.

&#x200B;

![NYSE Chicago https:\/\/www.nyse.com\/markets\/nyse\/trading-info#equities-order-types](https://preview.redd.it/h6iuikxau5e71.png?width=1247&format=png&auto=webp&s=2c3e657c2ddda3f6c9eeeed534bceb9b8578f4f5)

**1.** IOC ISO remains high, after switching from Limit non-routable IOC orders as the largest % back in September-2020, just before GME started to take off in retail interest. This shows that HFT activity really started to ramp up in terms of change in behavior, likely nefarious as defined above in terms of how ISOs can be abused.

**2.** ALO orders are trending lower and lower after it spiking up, this indicates to me that they are less inclined to try and control GMEs price. Why? Unsure could be many reasons. My theory is that we’re at such a price level and as us retail users have entered a cyclical buying pattern, we’ve highly likely become predictable in buying pattern and therefore buy/sell walls are not as frequently required on their behalf to control buy/sell pressure.

**3.** Limit Non-displayed orders, these have remained high since GME retail started to pop off in late 2020. Hidden from retail, able to “skip ahead of the queue”, this along with the other sus order types remaining high is all the indication you need to arrive at a conclusion.

# 37.46% of NYSE Orders are Dark?

Funnily enough, I don't usually check all the exchanges and just glance over them and head straight to the NYSE Chicago tab. What I found in my glance was a really strange “anomaly”, that showed Dark Primary Pegged order spike to 37.46%. 

Is this an error? Possibly. BUT, I’ve been tracking these updates since February, and this is the first time I’ve seen such a huge number appear at a specific percentage. It does make the total go over 100%, which is where the error logic comes through, but if this excel is powered by a macro, vlookups, whatever, it’s kinda odd that this would suddenly show up, and get published to their [website](https://www.nyse.com/markets/nyse/trading-info#equities-order-types) for all to see (assuming that it also goes through several approvals given it’s published 15 days in delay after month-end).

&#x200B;

![NYSE https:\/\/www.nyse.com\/markets\/nyse\/trading-info#equities-order-types](https://preview.redd.it/aj5lwkt6u5e71.png?width=1150&format=png&auto=webp&s=0f2d56a89e08c5b726d6192ba32471060aca9a7a)

So, saying this. It could very well be an error. Take it with a grain of salt, but it’s odd that this type of non-live data that takes 15 days to prepare and publish would show this…. \*tinfoil hat is on, because hey, errors are the bane of my existence (fuck you TD TOS Bug)\*

# Anywho, what even is a Dark Primary Pegged order?

Primary pegged orders are not generally used that much. A peg order is one that follows the best bid when buying a security and best offer when it comes to selling a security. Pretty much ensures that it **allows traders to get the best possible price as the price moves**.

If you’re thinking, what I’m thinking - we’re on the same wavelength (if this is not actually an error). Peg orders are used by traders in volatile markets, the peg comes in a literal sense as it “tracks” either the bid or ask depending on if you’re buying or selling to ensure you always get the best price. 

# What about the dark part?

Well, you can guess… It’s not shown on the order book until **after** it has been executed, so they don’t contribute to a ticker symbols quote (bid/ask). 

# What wavelength am I meant to be on?

Assuming this is not an error, this indicates to me that during June, traders were using dark primary pegged orders to get the best prices they can during various sell-offs that we’ve observed - without freaking out other traders looking at the order book due to the nature of the dark component of the order.

As you can imagine, and that we know, when large orders come through on order books, it can trigger flash crashes, which are then propelled by HFT picking up on this. How to avoid this and get the best bang for your buck during sell-offs? Dark primary pegged orders.