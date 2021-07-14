# Author: djk934
# Post URL: [https://www.reddit.com/r/Superstonk/comments/ofwnfd/citadels_connection_to_retail_orders_and_retail/](https://www.reddit.com/r/Superstonk/comments/ofwnfd/citadels_connection_to_retail_orders_and_retail/)


Previously I did a [DD on retail interest on GME](https://www.reddit.com/r/Superstonk/comments/oabdv7/gmes_retail_interest_examining_the_retail/) that focused on the numbers and  some of the information here is a repost from that write up, but with a couple of new important points. Since the retail interest continues to update, I also wanted to break off the educational part of that previous post about the Retail Liquidity Program that I could just link back too in the future. Hopefully I will also educate folks about this program that the NYSE runs since it gives us apes special information about how many shares retail is putting in orders for each week. This will also allow me/some other ape to move to more weekly updates on the actual data from the retail liquidity program.

Much of this is a more focused and shorter write up on Citadel being the most likely RLP. Though I record in detail how the RLP works and that part of this post could have been a separate Education/Data post, I felt that I should mark it as DD since there important inferences made based on how the program works and [another DD](https://www.reddit.com/r/Superstonk/comments/od4bb1/the_sun_never_sets_on_citadel_part_2/) done by /u/swede_child_of_mine 

This post includes many abbreviations, but was included to shorten things a bit. This DD was already getting long.

* CADV – Consolidated Average Daily Volume
* CTA – Consolidated Tape Association
* DMM – Designated Market Maker
* GME – GAMESTONK
* IoC – Immediate or Cancel (order type)
* MPL – Mid-Point Passive Liquidity ([MPL Image](https://imgur.com/DIiE0is))
* NYSE – New York Stock Exchange
* OBV – On Balance Volume
* RLP – Retail Liquidity Providers/Program
* RMO – Retail Member Organizations
* RPI – Retail Price Improvement ([RPI Image](https://imgur.com/CsAjdBF))
* SHF – Shitty/Short Hedge Funds
* SLMM – Supplemental Liquidity Market Maker
* SLP – Supplemental Liquidity Provider
* SLP-PROP – Supplemental Liquidity Provider Proprietary

**TLDR** 

The NYSE runs a program called the retail liquidity program which handles orders marked by brokers as originating from retail. Citadel is almost guaranteed to be the RLP for GME. These orders are filled within the program as much as possible but are generally adjusted to an IoC order depending on how the broker marks the order. These orders seem to end up filled anyways even outside of the program and I now suspect this is done within Citadel Connect. 

**Additionally, if you want a quick and dirty approximation of how many shares retail put in orders for (as an absolute minimum number), it's around 1.75% of the CADV (including both buys/sells) on a daily basis within the RLP. You can likely use this to very roughly approximate future retail share orders submitted within the retail liquidity program, but remember this is an absolute bare minimum number.**

Retail continues to amass more and more shares as time goes on.

**TLDR DONE**

**Previous Attempts at This**

There have been a few attempts on Superstonk at examining retail interest in GME. I believe u/HomeDepotHank69 was examining orders submitted with the first 30 minutes of the day to look at retail interest, but the results seemed to be inconclusive. ([https://www.reddit.com/r/Superstonk/comments/nu9qq9/hanks_big_bang_quant_apes_glitch_the_simulation/](https://www.reddit.com/r/Superstonk/comments/nu9qq9/hanks_big_bang_quant_apes_glitch_the_simulation/))

I also remember reading a post by u/jsmar18 ([https://www.reddit.com/r/Superstonk/comments/nar8dc/odd_lots_show_that_gme_interest_is_not_subsiding/](https://www.reddit.com/r/Superstonk/comments/nar8dc/odd_lots_show_that_gme_interest_is_not_subsiding/)) that was examining GME trades using odd lots as a marker for retail interest. He correctly acknowledges that both retail and HFT firms use odd lots frequently, however the data that I’ve looked at here indicates that a specific program run by the NYSE for retail orders only (called the retail liquidity program) seems to be filling retail orders in larger batches, while at the same time barely executing any orders within the program at all. While it could be a statistical anomaly of large retail whales skewing up the average, but I don’t really think this is the case after looking at execution.

**Data Source**

All data was obtained from [https://www.nyse.com/publicdocs/nyse/NYSE_Group_RLP.xlsx](https://www.nyse.com/publicdocs/nyse/NYSE_Group_RLP.xlsx) (this will download the data) found on [https://www.nyse.com/markets/liquidity-programs](https://www.nyse.com/markets/liquidity-programs) over the past several weeks. I was able to collect 7 out of the last 10 weeks of data, including the last 4 straight weeks. Unfortunately, there doesn’t seem to be a place to collect these documents (historical ones). I started to log them at [https://web.archive.org/web/*/https://www.nyse.com/publicdocs/nyse/NYSE_Group_RLP.xlsx](https://web.archive.org/web/*/https://www.nyse.com/publicdocs/nyse/NYSE_Group_RLP.xlsx) since the NYSE doesn’t seem to make this available or post it anywhere after the week they are posted is complete. I would encourage others to try to help log this going forwards as I missed a couple of weeks due to life. I will continue to try to preserve this data but any help is appreciated.

**Background**

The NYSE runs a program called the retail liquidity program. Brokers who are eligible as RMO’s (Retail Member Organizations) can mark orders as coming from retail, which are then serviced by the NYSE Retail Liquidity Providers (RLP’s). This is carried out with tons of securities and recorded against the tape and the program itself is not only for GME. GME is on Tape A if you’d like to look at the data yourself.

The most important point is that the Retail Liquidity Program will help establish the **ABSOLUTE MINIMUM** number of share orders submitted by retail, since it is not guaranteed that the broker you are using is an RMO and it is not guaranteed that your order is filled within the program.

**So how much of the CADV is retail?**

It looks like only around 1.75% of the CADV is the retail orders inside of the RLP. (remember this is the bare minimum since not every broker is an RMO).

[CADV vs. Retail Orders](https://imgur.com/LY404kv)

**Who can be a Retail Liquidity Provider?**

To become a Retail Liquidity Provider at the NYSE, you need to be either a Designated Market Maker (DMM) or SLP (Supplemental Liquidity Provider). However, the NYSE doesn’t actual reveal who their RLP’s are – I scoured the website, if you can find it I will add it to the post but I couldn’t. So, let’s infer who it could be based on the evidence we can gather.

**NYSE DMM’s**

* Citadel Securities LLC
* GTS Securities, LLC
* Virtu Americas LLC

**NYSE SLP’s (SLP-PROR or SLMM)**

* HRT Financial LLC
* IMC Chicago LLC
* Latour Trading, LLC
* Tradebot Systems, Inc.
* Virtu Americas LLC
* Citadel Securities LLC (SLMM)
* Goldman, Sachs and Company (SLMM)
* Virtu Americas LLC (SLMM)

Citadel and Virtu account for nearly 22.8% of market share by volume as individual firms, and then they also carry out special roles at the NYSE which accounts for another 19.9% of the market share. ([https://qz.com/1969196/citadel-securities-gets-almost-as-much-trading-volume-as-nasdaq/](https://qz.com/1969196/citadel-securities-gets-almost-as-much-trading-volume-as-nasdaq/) )

Based on previous claims that Citadel Securities completes nearly half of U.S retail volume and 26% of all U.S equities volume ([https://www.citadelsecurities.com/products/equities-and-options/](https://www.citadelsecurities.com/products/equities-and-options/)).

Virtu also claims to handle approximately 25% of all retail order flow in the US. ([https://www.virtu.com/market-making/client-market-making/](https://www.virtu.com/market-making/client-market-making/)) Virtu is also the preferred execution service for IBKR Retail Equity Volume ([https://s21.q4cdn.com/422114427/files/doc_financials/2021/q1/Virtu-Financial-Earnings-Presentation-2021-Q1.pdf](https://s21.q4cdn.com/422114427/files/doc_financials/2021/q1/Virtu-Financial-Earnings-Presentation-2021-Q1.pdf), see pg. 10). Just for clarity, Virtu Americas LLC’s parent organization is Virtu Financial LLC.

Based on these pieces of evidence, it is highly likely that the two larger RLP’s for the NYSE are Virtu Americas LLC and Citadel Securities LLC. Not surprising, but it’s good to back things up with evidence. RLP’s are also tied to specific securities, so it is likely one or the other in this case. However, I believe that Citadel is the RLP for GME since they are also the DMM for GME ([https://www.reddit.com/r/Superstonk/comments/n68ooc/did_you_know_citadel_is_the_nyse_dmm_for_gme/](https://www.reddit.com/r/Superstonk/comments/n68ooc/did_you_know_citadel_is_the_nyse_dmm_for_gme/)). 

It would be an easy addition for them and does not make sense for Virtu to poach this one from them given that Citadel dwarfs them and that Citadel would want control over the ticker that they shorted into the ground.
I didn’t realize right away that I couldn’t access old data once it was gone (I thought I could get it from [https://ftp.nyse.com/](https://ftp.nyse.com/) but no dice), so I have some missing data points with no apparent way to reconcile these. 

As I said earlier in the post, I have been archiving the files as they are posted now each week so hopefully will be able to continue examining this going forwards.

**So how does this program actually work?**

Suppose your broker is an RMO. They mark your order as originating from retail, with the order falling into one of 3 categories. An important feature is that the special tags by the RMO mark your order as NOT coming from an algorithm or HFT Firm. The orders listed in this data are from retail investors only and get classified one of three ways. (see pg. 369 of [https://www.nyse.com/publicdocs/nyse/regulation/nyse/NYSE_Rules.pdf](https://www.nyse.com/publicdocs/nyse/regulation/nyse/NYSE_Rules.pdf) for complete descriptions, I include an image)

[Retail Order Designation Image](https://imgur.com/PZibOUC)

**Type 1** – the retail order will only interact with available contra-side (i.e. buy matched to a sell and vice versa) RPI orders and MPL (Midpoint Passive Liquidity) orders. If the order is not completely filled, the portion that does not execute is immediately and automatically cancelled.

**Type 2** – the retail order will first interact with available contra-side (i.e. buy matched to a sell and vice versa) RPI orders and MPL orders. If the order is not completely filled, the remaining portion is the executed as a Reg NMS Immediate or Cancel (IoC) Order. This would fill as much as possible in the NYSE Exchange book, then the remainder gets cancelled.

**Type 3** - the retail order will first interact with available contra-side (i.e. buy matched to a sell and vice versa) RPI orders and MPL orders. If the order is not completely filled, the remaining portion is the executed as a NYSE Immediate or Cancel Order. This would fill as much as possible in the NYSE Exchange book and then through other markets if the execution is protected. Then the remainder of the order gets cancelled unless it is completed filled in other markets.

Note the part about orders being "immediately and automatically" cancelled. This based means that all of these order types effectively work as types of IoC orders.

**How many orders get filled in the RLP for GME?**

[Fill Rate Image](https://imgur.com/LFbGlDO)

From looking at the data, it appears like the fill rate for GME orders within the RLP program is averaging about 12.8% from April 26th to July 2nd.

**Why does this happen?**

[IOC Image](https://imgur.com/A802uCL)

I listed the order classifications here, because as you saw in the table a significant number of orders placed for GME are resulting in cancellations within the retail liquidity program due to how the orders are marked by the RMO and cancellations would happen when THERE ISN’T ENOUGH LIQUIDITY in the RPI and MPL order types. So even though over 85% of the retail orders were "cancelled" within the retail liquidity program, I would hazard an educated guess that your orders got filled anyways. Since the RMO is potentially submitting orders as batches, smaller orders are just straight up getting filled with no cancellations (the average size of an executed order is around 30 shares which seems reasonable but the submitted orders are like 200+ shares), while larger orders are taking more time to actually fill OR are being ported out of the program into a *non-disclosing portion of the market* that's hidden... 

**I am 140% SHF positive that it would have been posted about on Superstonk if apes trying to purchase GME were consistently getting orders cancelled in line with the percentages indicated in this data.**

It was unclear to me exactly how these “cancelled orders” from the retail liquidity program end up getting filled anyways, since it appears as though (after exhausting the RPI and MPL orders) they would convert into order types that always end up with a portion that could get cancelled if the liquidity is not there. However, after reading "[The Sun Never Sets on Citadel, Part 2](https://www.reddit.com/r/Superstonk/comments/od4bb1/the_sun_never_sets_on_citadel_part_2/)" and chatting with /u/swede_child_of_mine I suspect that the orders that are “not executing” in the RLP are being internally filled within Citadel Connect because they are primarily IoC orders and do not require disclosure. (Read their post for details on that) Given that the average fill rate within the program is <15%, that means that Citadel would be processing >85% of orders within Citadel Connect for GME. 

I look forward to someone with better data access or who is wrinklier than I am verifying this part (if that is even possible), but given the evidence within the RLP, it definitely looks like Citadel is hiding the vast majority of the retail trades for GME within Citadel Connect.

HEY NYSE, SEC AND FINRA...

HOW THE FUCK WAS THIS ALLOWED TO HAPPEN?

HOW IS IT BEING ALLOWED TO CONTINUE?

![I mean...](https://imgur.com/xdv3qf4)

🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀