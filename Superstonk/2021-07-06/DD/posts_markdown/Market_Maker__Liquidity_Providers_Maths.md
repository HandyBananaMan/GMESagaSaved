# Title: Market Maker / Liquidity Providers Maths
# Author: ammoprofit
# Post URL: [https://www.reddit.com/r/Superstonk/comments/oequz8/market_maker_liquidity_providers_maths/](https://www.reddit.com/r/Superstonk/comments/oequz8/market_maker_liquidity_providers_maths/)


Once again, I am [replying to a comment](https://www.reddit.com/r/Superstonk/comments/oeahh2/rcs_tweets_are_timed_with_etf_ftds/h47asll/) and have exceeded the 1500 character limit, so you get a DD.

# TL|DR?

Honestly, I'm not sure what to conclude from this, and until we can confirm the LP's criterias and obligations, we should be careful  arriving at any conclusions.

As near as I can tell, this changes the total shares owned, and introduces a new, mostly invisible, combination metric of LP Owed Shares and LP Strike Price, similar to derivatives.

If there's a timeframe obligation to repurchase, then it gets an Open Interest type metric, too. Otherwise, it's just Volume & Price.

I tried to come up with a scenario where I could reasonably argue the SEC should make this information publicly available in a timely manner, but because of the legal and financial impact to the underlying asset's parent company, *LP privileges should be revoked entirely*.

I might consider LP privileges (LPP) in a scenario where you have acquired the shares but are waiting on T+3 settlement, but I don't see why LPP is needed for that.

&#x200B;

# Edit #3

There's a [comment](https://www.reddit.com/r/Superstonk/comments/oequz8/market_maker_liquidity_providers_maths/h487fi1/) suggesting I am conflating Maker Taker with PFOF.  The discussion is ongoing.  I strive for accuracy, and I am awaiting feedback.  (Not sure I can tag the username without triggering the automod.)

I expect Maker Taker and PFOF revenue to be roughly comparable.  Given my conclusion, I don't think it matters.  Once I have more information, I'll adjust the post accordingly.

&#x200B;

# Meat & Potatoes:

Today we are looking at Liquidity Providers.  Liquidity Providers have bothered me since I first found out about them.  LPs have an exemption that allows them to sell shares of stock (equity) today, even shares that do not ~~exist~~ own, as long as certain criteria are met and they repurchase the shares later.

This is incredibly weird for a lot of reasons that mostly pertain to market manipulation and undercutting sellers.

But, primarily, this allows both good and malicious LPs to perform share offerings on behalf of companies **without filings or authority**.  We, the public, rely heavily on those filings to make informed decisions, and there is *no* insight into this behavior, it's volume, it's frequency, when it occurred, or anything else metric-ly substantial.  We are almost 100% in the dark, and the companies are largely in the dark, too.  (Arguably, they knew this raw deal when they entered the stock exchange, but holy fuck.  What a blind spot!)

&#x200B;

# Let's figure out what we know.

A Market Maker will charge a fee per transaction.  That means they are primarily volume based.  This is important because MM are incentivized to have transactions flowing through their markets.  If there is no volume or liquidity, the MMs don't eat, and they're hungry.

[Investopedia says](https://www.investopedia.com/articles/active-trading/042414/what-makertaker-fees-mean-you.asp), emphasis added, mine:

>Makers typically are **high-frequency** trading firms, whose business models largely depend on specialized trading strategies designed to capture payments. Takers generally are either large investment firms looking to buy or sell big blocks of stocks or hedge funds making bets on short-term price moves.  
>  
>The maker-taker model runs counter to the traditional “customer priority” design, under which customer accounts are given order priority without having to pay exchange transaction fees. Under the customer priority model, exchanges charge market-makers fees for transactions and collect payment for order flow. Order flow payments are then funneled to brokerage firms to attract orders to a given exchange.  
>  
>The maker-taker plan harks back to 1997, when Island Electronic Communications Network creator, Joshua Levine, designed a pricing model to give providers an incentive to trade in markets with narrow spreads. Under this scenario, makers would receive a $0.002 per share rebate, and takers would pay a $0.003 per share fee, and the exchange would keep the difference. By the mid-2000s, rebate capture strategies had emerged as a staple of market incentive features, **with payments ranging from 20 to 30 cents for every 100 shares traded.**

In English?  We know ~~MM~~ Exchanges act as the middle person between a buyer and seller, and one party pays $0.30 and the other receives $0.20, and the ~~MM~~ Exchange gets the difference ($0.10) per 100 shares.

(If your keen eye caught that the LPs act when there is a buyer without a seller, we cover that at the end.  For now, we are focusing on profits that exceed their normal revenue streams, assuming three parties.  Trust me.  You'll see why it doesn't matter in the slightest.)

&#x200B;

We also know:

1. A dollar today is worth more than a dollar tomorrow (yay! inflation!)
2. Shares have Share Price
3. Most stocks are sold in lots of 100 (like a pound of flour at the grocery store)
4. If an LP sells a share for liquidity, it has to purchase it back when the share price drops below that sold price
5. There are 365 days in a \[non-leap\] year

Yay.  Now we get some math.

* Inflation per day = 3.5% / 365 = 0.009589% per day
* Δt = Number of Days between when an LP sells the shares and when it buys them back
* Let's assume the LP sold 100 shares and bought 100 shares later at the same price.  The difference is $0.00.

This gives us an equation of roughly...

( # of Shares Sold / 100 ) \* Share Price \* Δt \* 0.009589% > $0.10

( # of Shares Sold / 100 ) \* Share Price \* Δt \* 0.00009589 > $0.10

( # of Shares Sold / 100 ) \* Share Price \* Δt > $1,042.86

\# of Shares Sold \* Share Price \* Δt > $104,286.16

===================================================================

Edit #4: I originally did the math for 10c per 100 shares sold for Market Makers, but I got the relationship wrong.  Because the LP can be either a buyer or seller, they can either pay 30c per 100 shares or receive 20c per 100 shares.  Oddly enough, it really doesn't change the math, and I'll highlight that point down below.  Keep reading.

===================================================================

&#x200B;

Ok, great, but how does this help us?  Turns out u/FreezYourMind cranked out the image below in this [great post](https://www.reddit.com/r/Superstonk/comments/o9l10s/gme_t21_as_it_becomes_clearer_it_seems_its_not/):

&#x200B;

https://preview.redd.it/2dk4pggvuj971.png?width=1872&format=png&auto=webp&s=b4d74b9b51bca0526e1b6a3832142c8fe13f02d5

If the LP is behaving according to the rules, every sale should generate a support now *and the same support later*.  (I still have trouble wrapping my head around explaining this part.  Apologies.  I haven't had my coffee yet.)

That image shows a series of resistances.  The last resistance was just under $200.  Let's use $200, because it's a nice round number.

\# of Shares Sold \* Share Price \* Δt > $104,286.16

\# of Shares Sold \* $200 \* Δt > $104,286.16

\# of Shares Sold > 521.43/Δt

If an LP sells shares today at $200, and buys them back tomorrow ( Δt = 1 ) at $200, in a world with a flat 3.5% inflation per year, they need to sell more than 521.43 shares to make a profit.  If the delay is 2 days, they need to sell at least 260.72 shares.

In restaraunt work, you are limited by your seats. Turnover is how many tables you can flip.  People sitting around drinking coffee aren't buying things.  Here, it's the reverse.  The longer the turnover (Δt), the longer you get to play with your money before you spend it on shares you owe, and the more favorable your numbers get.

&#x200B;

These shares are sold in lots of 100, so let's round up.  Always be conservative.  For every 600 shares per 1 day turnover at $200 each, an LP will generate more money than their traditional business model.

If you share price goes down, your volume or turnover must increase.  If we assume 1000 shares, we get...

1000 Shares Sold \* Share Price \* Δt > $104,286.16

Share Price > $104,286.16 / 1000 / Δt

\> \~$104.29/Δt per 1000 shares sold

I think this is a particularly neat equation with huge ramifications for stocks with both low liquidity *and* share prices under $10.  Especially penny stocks - ho-*ly* fuck.

&#x200B;

&#x200B;

But some of you had a keen eye and realized MMs act as the middle between a buyer and a seller.  We know there is a Buyer because the MM is creating and selling the shares, and we know there isn't a Seller because there is no volume or liquidity.  That means we're not getting either the $0.30 or $0.20 and taking the difference of $0.10.  Instead we're receiving one payment of either $0.20 or $0.30.  Assuming $0.20 instead of $0.30 (most conservative), that doubles the result to > \~$208.60/Δt per 1000 shares sold.

&#x200B;

# LP Revenue absolutely dwarfs Maker-Taker Revenue

We're assuming the LP buys back the shares, and we're assuming they buy them back at the same price they sold them for.  There's no gaurantee either of these assumptions are true.  The price may never drop back down.  They may only purchase a portion of the shares before the price rises again.  The LP may be nefarious and never intend to repurchase the shares.  We don't know.

&#x200B;

Profit = ( Sold Share Volume \* Sell Price ) - ( Buy Share Volume \* Buy Price )

You can take a look again at Freez' image with the supports and resistances and fiddle with the math.

&#x200B;

Regardless, *when* the shares are never purchased, the equation changes dramatically.

Profit = (# of Shares Sold \* Share Price ) + ((# of Shares Sold / 100) \* 0.10)

&#x200B;

First, they're selling N shares for some price. Second, they get $0.10 per 100 shares sold for being the middle person.  Third, they never repurchase the shares, so we can drop the inflation portion of the equation entirely.

Let's compare apples to apples from our previous equations.  We'll assume 500 shares this time, using the most conservative block of 100 shares for the 521 shares from before, and we'll use the same share price of $200.

Profit = (500 shares \* $200 per share) + (500 shares / 100) \* $0.10)

Profit = $100,000 (LP sale) + $0.50 (Maker-Taker)

Even if the MM LP cut is $0.30 per 100 shares, that increases the Maker-Taker revenue to $1.50

Let's be real.  You don't care about the Maker-Taker revenue.  *That's a fart in a hurricane.*

==== \^\^  See Edit #4 down below \^\^ ====

Now take a look at the resistance image again.

https://preview.redd.it/ayq8hwogvj971.png?width=1872&format=png&auto=webp&s=23c2932705e45b29f32183025fbe6ab1af5211fd

I never understood how the daily drops' volume was always so much higher than the [available borrows](https://iborrowdesk.com/report/GME), even when accounting for the \~10M shares in ETFs.  And I never understood why the resistances kept increasing.  I could understand the resistances to some effect, because each % we eat of their borrows increases their overall short position, but the two pieces never added up.

Retail, simply put, does not have the power to effect that much volume in either direction right now.  (Yes.  Effect with an E.  I will fight you.)

Even though our math is rough, at best, I think Liquidity Providers' actions and obligations explains the supports and liquidity.

I'm not really sure where to go with this next.  I hope someone finds language in one of the previous or new rulings that says something like, "LPs must close their positions within timeframe," similar to the FTD mechanics for equities (stocks) and their derivatives (options), but I'm not sure where to look for that language.

&#x200B;

Edit: Formatting changes and cleaned up redundant formulas.  Also edited TLDR to reflect my personal take.

Edit 2: Longer TLDR

# 

# Edit #4:

Both Maker-Taker and PFOF are competing for roughly the same market inventory.  It might be weird to think of transactions as market inventory, but it is.  They've got their pros and cons between them, but they're either a flat fee or a percentage take.  Either way, the revenue from this is large enough to make a business (or augment existing revenue streams), but small enough that it doesn't drive business away.  That means there's no reasonable way either MT or PFOF could realistically compete with selling purchased shares for profit (ΔShare Price), much less selling \[as of yet\] unpurchased shares for profit.

I wish I had similar metrics for PFOF so we could do both maths side by side, but I don't.  But we know the numbers should be similar because they are competing for the same market inventory.  Even if we give PFOF 10x the revenue impact ($15.00) as MT ($1.50), the example provided demonstrates *it just doesn't matter.*

Details matter *for so many reasons*, especially when we try to convey important points accurately to people who understand these systems well.  But these details don't change the big picture.

When you can sell something you don't own and don't intend to purchase, you make money hand over fist.