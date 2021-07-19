#Title: Citadel's Clear Error
#Author: djk934
#Post URL: [https://www.reddit.com/r/Superstonk/comments/n7ap6e/citadels_clear_error/](https://www.reddit.com/r/Superstonk/comments/n7ap6e/citadels_clear_error/)


So for the past three straight days, millions of volume has been removed after hours in what appears to be a “glitch” – except it’s happened for a few straight days. Also, why would these transactions just disappear? The stocks with disappearing volume seem to be on the NYSE and it doesn’t seem to be only GME. An issue with the consolidated tape? I believe that's only partially true.

For more evidence on this being a thing that's showing up.

Check out u/ECSJay post ([https://www.reddit.com/r/Superstonk/comments/n5q0kf/negative_1_million_volume_in_afterhours/gxb85on/?context=3](https://www.reddit.com/r/Superstonk/comments/n5q0kf/negative_1_million_volume_in_afterhours/gxb85on/?context=3)) and u/bsw000 post ([https://www.reddit.com/r/Superstonk/comments/n6yfab/td_ameritrade_showing_another_negative_volume/](https://www.reddit.com/r/Superstonk/comments/n6yfab/td_ameritrade_showing_another_negative_volume/) )

As I was writing this, I also saw u/dlauer’s post on the same issue. ([https://www.reddit.com/r/Superstonk/comments/n772fg/negative_volume_prints/](https://www.reddit.com/r/Superstonk/comments/n772fg/negative_volume_prints/))

I'd love for some critiquing on my theory here as well.

**TLDR**

Based on public removal of volume from the consolidated tape (which normally doesn’t happen, especially not immediately after the trading day is done), I suspect that it is likely that Citadel Securities handling of GME transactions (which is showing these glitches among some other stocks reporting the same error that are under Citadel's purview) is resulting in trades being flagged as “clearly erroneous” and that the NYSE is stepping to review these trades and after that review are REMOVING them from the volume after hours and showing up as these weird negative volumes. 

**TLDR OVER**

Ok 🚀🚀🚀🚀🚀🚀🚀🚀 time. A bit of background on how the system software works behind the scenes in the stock market - but this is a simplified explanation. The CTA (Consolidated Tape Association) runs the CTS (Consolidated Tape System) and the CQS (Consolidated Quote System). Each of these are known as Securities Information Processors or SIPs.

The current Participants (of the CTA) include the Cboe BYX Exchange, Inc., Cboe BZX Exchange, Inc., Cboe EDGA Exchange, Inc., Cboe EDGX Exchange, Inc., Cboe Exchange, Inc., Financial Industry Regulatory Authority, Inc., Investors Exchange LLC, Long-Term Stock Exchange, Inc., MEMX LLC, MIAX Pearl, LLC, Nasdaq BX, Inc., Nasdaq ISE, LLC, Nasdaq PHLX LLC, Nasdaq Stock Market LLC, New York Stock Exchange LLC, NYSE American LLC, NYSE Arca, Inc., NYSE Chicago, Inc., and NYSE National, Inc. ([https://www.ctaplan.com/index](https://www.ctaplan.com/index) )

The CTS is an electronic service that reports the latest price and volume data on exchange-listed stocks. The CQS is an electronic service that provide quotation information. Both services were implemented back in the late 1970’s to help with the move to electronic trading. Each of these are known as SIP’s. 
([https://www.exegy.com/2019/12/consolidated-tape-nyse-feeds/](https://www.exegy.com/2019/12/consolidated-tape-nyse-feeds/) ) 

There are three tapes involved here called Tape A, Tape B and Tape C. GME is on Tape A (you can find this at this link [https://www.nyse.com/publicdocs/nyse/NYSE_Group_RLP.xlsx](https://www.nyse.com/publicdocs/nyse/NYSE_Group_RLP.xlsx)).

The Securities Information Processor's (SIP) link the U.S markets by processing and consolidating all protected bid/ask quotes and trades from every trading venue into a single data feed. It disseminates and calculates the National Best Bid and Offer (NBBO) and Limit Up Limit Down (LULD) prices. It also handles short sale restrictions and regulatory halts.

SIPs collect trade reports from ALL SRO (Self-Regulatory Organizations) INCLUDING OFF-EXCHANGE VENUES (i.e. Dark pools) reporting trades via FINRA trade reporting facilities. ([https://www.ctaplan.com/publicdocs/ctaplan/notifications/trader-update/Revenue_Allocation_Formula_Summary.pdf](https://www.ctaplan.com/publicdocs/ctaplan/notifications/trader-update/Revenue_Allocation_Formula_Summary.pdf) ) Basically this means that ALL QUOTATION AND PRICING INFORMATION FOR ALL TRANSACTIONS ARE INTENDED TO BE RECORDED BY THE SIPs. But shit seems like it is being removed right? We’ll circle back to this in a bit. 

We need a bit more background on the NYSE and SRO's.

Examples of SRO’s would be the current participants of the CTA, listed above. So the NYSE is an SRO, while it’s designated market makers are Citadel Securities LLC, GTS Securities LLC and Virtu Americans LLC, with Citadel Securities LLC being by far the largest. However, Citadel Securities is also a Supplemental Liquidity Provider, which will be important in a moment.

The NYSE runs something called the Retail Liquidity Program. There are two classes of market participants that “help” with handling retail orders, called RMOs (Retail Member Organizations) who submit retail order flow and RLPs (Retail Liquidity Providers) who provide price improvement. Funnily enough to be an RLP you must be a designated market maker or supplemental liquidity provider. Turns out Citadel Securities is BOTH, making them the likely primary candidate here, especially given their 40%+ handling of retail trades.

So the SIP’s record ALL of the transaction data regarding the NYSE and Citadel Securities has its finger intimately inside of the retail order flow at the NYSE level through its involvement as a DMM, SLP and RLP. This is slightly different than the payment for order flow (PFOF) stuff they conduct with other groups like Robinhood.

As a side note, the orders that come from RMO’s require a couple of interesting ORDER TYPES and cannot come from a trading algorithm. All three of these order types begin with “Remove order that interacts with Retail Liquidity”. Now I don’t think these actually remove volume, but I’d love for another person to dig into this or I will if I get more time. Basically at the NYSE level, there are special order types for retail trades and these can get handled by an RLP.

🚀🚀🚀🚀🚀🚀🚀🚀

Remember earlier how I said that GME is on Tape A? **Turns out you can download the document for Retail Orders from April 26-30, 2021 handled through the RLP from the NYSE website**. ([https://www.nyse.com/markets/liquidity-programs#:~:text=Retail%20Liquidity%20Providers%20\(RLPs\)%20who,do%20not%20receive%20enhanced%20economics](https://www.nyse.com/markets/liquidity-programs#:~:text=Retail%20Liquidity%20Providers%20\(RLPs\)%20who,do%20not%20receive%20enhanced%20economics)) 

*An unrelated to this topic but cool piece of data I came across here is in that 5 day interval on average retail put in orders to the NYSE's RLP system for 130,000 shares of GME every day. (It doesn’t say buying or selling, but we know how retail folks feel about selling GME) Tweaking that number to round out at only 100,000 shares bought per day (75% of orders are buys) would mean that the diamond hands likely locked up around 2% (500k/26 mil) of the available float that week. This little tidbit would also imply that about HALF of the shares being bought during that period didn’t come from other retail. Which either means that institutions are selling their shares to us OR the lovely DMM/NSCC is rehypothecating around 50-60k shares EVERY DAY that week. I’m suspecting it’s the latter, but let’s move on.*

Now we know a couple of things. We know that GME is on Tape A, retail trades are handled by an RLP (likely Citadel) and we’ve seen that millions of volume is showing up as “being removed” after hours. We know that Citadel has its sticky fingers in basically every aspect of the NYSE, particularly with handling retail orders due to its role as a DMM, SLP and RLP.

So how does volume actually get REMOVED from Tape A in order to show these after hour reductions? Why wouldn't Citadel just remove this from showing up with their special position? Turns out, I don't think they can. Only a NYSE exchange officer (higher up than Citadel) seems to be able to perform this clever magic by enforcing the following rule and they have to act since it's affecting a large group of tickers.

🚀🚀🚀🚀🚀🚀🚀🚀

**Clearly Erroneous Executions (Rule 128)**

You can find all of the rules ([https://www.nyse.com/publicdocs/nyse/regulation/nyse/NYSE_Rules.pdf](https://www.nyse.com/publicdocs/nyse/regulation/nyse/NYSE_Rules.pdf))
A transaction with an obvious error such as price, number of shares or any other unit of trading, or identification of the security. When transactions are classified as clearly erroneous it ends up being REMOVED from the consolidated tape. That does mean though that they hit the order book at some point before being removed.

From what I could find, this is the ONLY reason a transaction would be removed from the tape after hours. Remember that the tape records all the dark pool data as well. It records every transaction and requests for review of clearly erroneous transactions must be reviewed by an Officer of the Exchange. Importantly, this rule runs OUTSIDE of the reach of the sticky Citadel fingers. If a trade is flagged as obviously erroneous it needs to be rectified BEFORE THE BEGINNING OF THE NEXT TRADING DAY. This fits with the after hours theme. It also means someone has decided to enforce this rule specifically.

But why?

Interestingly a clause in Rule 128 is present that describes the thresholds for declaring a trade "clearly erroneous" but specify **that this can be threshold can be ignored, allowing the exchange to set their own reference price**. We've been trading sideways for awhile. Anyways, it reads that the threshold can be ignored “in other circumstances, such as, for example, relevant news impacting a security or securities, periods of extreme market volatility, sustained illiquidity, or widespread system issues, where use of a different reference price is necessary for the maintenance of a fair and orderly market and the protection of investors and the public interest.” ([pg. 426 of the NYSE rules](https://www.nyse.com/publicdocs/nyse/regulation/nyse/NYSE_Rules.pdf))

**I think it’s safe to say that Diamond Handing the stock has resulted in **Sustained Illiquidity** recently, with volumes around 3 million per day.**

💎💎🙌🙌

**It might interest you to know that Citadel Securities LLC has been fined six times by FINRA for abusing the exchange systems for CLEARLY ERRONEOUS transactions within different exchanges.**

Based on this, I believe that it’s likely that our missing volume blips are emerging from someone at the NYSE (cough Citadel cough) manipulating the price during the day, then batches of these trades are getting flagged as erroneous and then the NYSE is stepping in to remove them in the after hours before the next day begins. Since it's a few different tickers simultaneously, the NYSE HAS TO STEP IN TO FIX IT.

So why would Citadel submit clearly erroneous trades to get flagged? 

I think they've made a colossal mistake shorting GME, but are completely and utterly trapped. I don't see how this helps them get out of it. Could the NYSE itself be trying to stabilize things until the rules pass? End of the day it doesn't matter why cause shorts gotta cover baby.

But based on this, I damn well believe they ARE doing it.

*Tick fucking tock.* 

EDIT 1 - So apparently the CTA reported an error on the CTS tape for May 5th on Tape B (which GME isn't on). Hmm. ([https://www.ctaplan.com/alerts#110000353886](https://www.ctaplan.com/alerts#110000353886)) Credit to u/MonoshiroIlia

EDIT 2 - I've gotten a few messages and seen some comments about what happens to these trades and thought I would share my thoughts, even though I could be completely wrong. If these trades happened between complicit hedge funds or were wash trades with separate entities within Citadel, then the parties would agree that they were erroneous, and the clearly erroneous trades that are cancelled don't require the generation of additional shares so the Exchange would just nullify them after hours - no extra shares need to be made. If some of those trades went to retail though, it's likely that if the Exchange overrode the trade (normally both sides need to agree, but there are provisions that allow the NYSE to do this) then the NSCC would need to fill the order using (likely) rehypothecated shares.

EDIT 3

Holy crap - posted this and went for a few garage beers and woke up to lots of questions/comments - glad people reviewed this. 

u/Pouyaaaa sent a message that /uECSJay posted [this](https://www.reddit.com/r/fidelityinvestments/comments/n5qurg/how_do_you_get_a_negative_1_million_volume/gx7ah70/?context=3) which confirmed that Fidelity is aware of volume "disappearing". 

u/bluewhitecup sent a couple of interesting links that I have yet to dig through. 

u/Financial_Napalm posted about wash trades where the buy and sell are both cancelled - there's no way to tell this as far as I am aware as the data isn't specific enough. 

u/KompostMacho mentioned this as a good way to control price since the trades are declared erroneous. In fact it's even better for price control than that, since the NYSE can directly INTERFERE with the reference through the threshold clause - whether that would be to the GME investors benefit or not, there's no way to tell.

u/HoosierDaddy_76 asked about looking through retail trading data on the NYSE. I only found the one link that recorded trades conducted within the RLP that recorded trades from April 26-30, 2021. It's likely the other data exists somewhere, but I have been unable to find it. It may be paywalled by the NYSE and likely would be expensive to get access too.

I think I included most of the important ones to address now. 

For reference repeatedly submitting clearly erroneous trades is illegal and will result in fines (remember that Citadel's been fined 6 times for this). But like most illegal things in money land, these fines are not that large comparative to the benefits. 

🚀🚀🚀🚀🚀🚀🚀🚀