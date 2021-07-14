# Author: glide_si
# Post URL: [https://www.reddit.com/r/GME/comments/mk3gcd/call_memaybe_why_the_massive_volume_of_deep_itm/](https://www.reddit.com/r/GME/comments/mk3gcd/call_memaybe_why_the_massive_volume_of_deep_itm/)


[There](https://www.reddit.com/r/GME/comments/m05jed/mystery_solved_the_deep_itm_calls_are_coming_from/) [has](https://www.reddit.com/r/GME/comments/m7n0rm/hiding_ftds_in_dark_pool_calls/) [been](https://www.reddit.com/r/GME/comments/mhv22h/the_si_is_fake_i_found_44000000_million_shorts/) [a](https://www.reddit.com/r/GME/comments/m0pvlc/update_38_84_million_in_calls_in_last_hour_2465m/) [lot](https://www.reddit.com/r/GME/comments/mjzx9w/full_analysis_of_current_gme_si_proof_from_the/) of thoughtful DD regarding the strange volume of deep ITM calls. 

None of it I feel has dived into the unusualness of the actual order flow, which I hope to do in this post. 
This is post is not intended to draw a definitive conclusion rather it is to reiterate how unusual this volume has been and spark a discussion, especially revolving on these double transactions we are seeing.

&nbsp;

*Brief terminology for the smooth brains:*
>[Overview of Options](https://optionalpha.com/handbook/options )
>
Volume = Number of options contracts transacted in a day

>Open Interest (OI) = Number of contracts still open at the end of day. A contract can either be removed by exercising it (for example getting the shares if the call is in-the-money) or closing your contract by selling it back (or buying it back if you are the seller) thereby closing the loop.

>Deep ITM Call = A call option whose strike is ~~very far away~~ far below the current the trading price. Depending on its expiration date its value will almost completely be made up of its intrinsic value, meaning that 4/16 12C will effectively be fairly valued at the current share price - $12. 
*Edit*

&nbsp;

#Let's Dive

[Take a look at this chart comparing the 4/16 11, 12 and 15 Call Volume and OI since the beginning of this year.](https://i.imgur.com/IfqxbeD.png) 

[Here is the same chart but with FTDs displayed (data for FTDs is only available up to 3/12\).](https://i.imgur.com/nWZdHGE.png)

You notice relatively normal activity through most of January. Open interest (the dotted lines on the graph) was relatively stable and volume was not especially high but that is not unusual for a contract that still had 100+ days to expiry.  I would not try to draw conclusions between the share price or FTDs on the graphs – that is just to give some perspective.

We see the run up in share price in late January, a big volume surge in these contracts and a decrease in OI as people closed or exercised these contracts for profit. 

&nbsp;

What is more interesting is what comes next:

&nbsp;

OI remains stable (no one is closing or exercising these contracts) and volume almost nonexistent up until 2/25. The day beforehand, 2/24, GME unexpectedly jumps up 104% to close at 91.71 and continued surging into afterhours. We see the big volume spike for these calls the following day and throughout early March – however OI does not change. Things quiet down for a bit up until the past few days when we again saw huge volume spikes for these calls, especially at the 12 and 15 strike price. Despite this, OI is grossly unchanged since beginning of February. 

I included the 11C to illustrate just how unusual this activity is. The 11C is fundamentally identical to a 12C in terms of its characteristics in relation of its premium to share price but it gets no love and you can barely see it in the graphs. *In retrospect I should have included the 10C as that would be more popular to retail/swing traders due to its nice, even number - [but I assure you that after January it does not see nearly as much volume like the 12 and 15 Calls](https://i.imgur.com/E6VVqWm.png).*

So why are the 12c and 15c so popular? I have no idea but what is especially interesting is the order flow themselves.

#The Double Orders
[Take a look at largest option trades on 4/1. Notice anything?](https://i.imgur.com/2rgZEGt.jpg) 

At 1:22 PM we see large 12 and 20 calls orders. Two seconds later we see another set contracts for the same quantity and strike. 

That’s an initial set of trades is at a cost of $17,470,00. Based on this it seems like it is immediately sold-to-close two seconds later at a slightly higher price ($5,050 difference). Keep in mind the Bid/Ask strikes (and underlying share price) for this contract are unchanged but the mid-price (aka the transaction price) increased slightly in these two seconds.

That’s – um – weird. 

We see a run up in GME share price immediately after that to 196 before it pulls back to 192. These trades otherwise occur on a day when volume is near recent all-time lows, price action has been uneventful, and not much seems to be going on the surface. 

And then it happens again – but on a larger scale. Big orders for 12, 15, 18, 19 Calls are seen at 1:58 PM. On the GME chart we see a small pullback about 10 minutes later. Repeat orders for the same strikes and quantity are seen again at 3:29 PM. There is some increase volume of GME and price dip about ten minutes later.

These large “double” contracts are not a new phenomenon. It is hard to track them with the smooth brain tools I have at my disposal but [here is another example from 3/8](https://i.imgur.com/STxMILr.jpg). We see [similar activity on 3/1](https://i.imgur.com/H9IkLjR.jpg) but also orders that do not seem to have a “double” counterpart (regardless these orders have no net effect on OI). 

Theses are not double prints showing up on the orderbook of a single trade as we see the price for the two sets of contracts vary between the first set and the second set. 

Additionally, in [u/dejf2 DD](https://www.reddit.com/r/GME/comments/mhv22h/the_si_is_fake_i_found_44000000_million_short/ ) he has screen caps of the various large deep ITM options play on 4/1. [I particularly like this one.](https://preview.redd.it/74jgvko2hmq61.png?width=634&format=png&auto=webp&s=17745e15f7f32f2354c357dba338ec1f3f7c2ff7) It shows that despite the different quantities between the two sets of orders due to the different prices the total quantities are perfectly aligned after the second transaction. 

You may be thinking: “Hey the only reason you are noticing these are because they are expensive!”


Well no. Lets look at the 4/16 200c and 250c which are cheaper and considered normal, reasonably bullish plays: [834 and 1,122 vol respectively versus the 4,045 vol for the 12c on 4/1.](https://i.imgur.com/bRoBrWP.png)  

So what can we draw from this? Well as far as I have can tell all these contracts are routed through PHLX, are priced at the midpoint price (indicating an arrangement between two parties), involve select deep ITM calls (predominantly the 12 and 15 strike point but all deep ITM), and the contracts exist from anywhere from a few seconds to few hours in the day.

#A Brief Aside
A key fact is that all of these options contracts are at the mid-point price. This is an arranged transaction between two parties. Lets say I decide I’m going to buy 30 million dollars’ worth of GME shares tomorrow on the open market. A MM has to give me those shares at the best bid – but I’m buying them at the BID and that bid will go up as I buy more shares. But lets say they don’t have enough shares in their inventory to cover that? Well they are allowed to naked short me briefly while they go out and look to acquire the shares – usually from their own internal pool and then from another MM. When MMs swap shares between each other they do it at the mid-price. Their goal isn’t to take a position but to maintain liquidity and to profit off the transactions themselves. The fact that these call options are all at the mid-price indicate it is not some lone long whale or small hedge fund (Melvin) buying up these contracts to make a swing play – it is two MMs or broker-dealer doing the transaction in an organized fashion.

&nbsp;

Why the PHLX? 


Well these “SingLegFlr” trades mean they are Single Leg Floor Trades. 

Definition:

> Transaction represents a non-electronic trade executed on a trading floor. Execution of Paired and Non-Paired Auctions and Cross orders on an exchange floor are also included in this category.

So these trades are occurring via brokers who are physically present at the Philadelphia Exchange. 

#The Buy-Write
I’ve read a lot of DD referencing [this SEC risk alert](https://www.sec.gov/about/offices/ocie/options-trading-risk-alert.pdf) and while it sounds suspiciously like this might be a buy-write style transaction –I am not convinced that is the case…otherwise why do we see the “double” contract transactions?

A buy-write in essence is Group A buying 100 shares from Group B while selling a contract at the same time to Group B – Group B exercises and they get the 100 shares back that they had sold to Group A. That is a one-way options transaction in which the call is created/sold and exercised thereby removing it from OI. It does not explain these double orders. They may do this while at the same time buying Calls/Selling Puts that are At-The-Money to generate a synthetic long position. 

There are three possible explanations why we are seeing this huge volume, double orders, and no net change in open interest:

1. These contracts are being bought-to-open with immense capital and then later sold-to-close – sometimes within seconds but always that same day - with minimal return of on capital. 

2. These contracts are bought, executed, and then bought again at the same quantity and strikes and executed again – thereby keeping OI unchanged but with two sets of orders for the same strike and quantity appearing on the order book.

3. These contracts are being written by Group A and sold to Group B who immediately executes them and gets Group A’s shares. Group B then writes an identical contract for the same strike and sells it back to Group A who then executes them. The net effect is shares move from Group A to Group B and then back to Group A. The volume of contracts is doubled reflecting these two transactions and open interest remains unchanged at end of the day as both sets of contracts were executed. One party receives a small net premium for this transaction. 

I’ve speculated on different reasons this may be going on [in this comment](https://www.reddit.com/r/GME/comments/mi31m6/deep_itm_calls_activity_pt2_april_1st_708000_ftds/gt38jtj/). Keep in mind this is pure speculation but written in a way I hope will create a dialog.

#The Trade

Let’s go deeper and just look at[ this one large order for 12C that began at 1:58 PM on 4/1](https://i.imgur.com/2rgZEGt.jpg): 

* At 1:58 PM 1,470 contracts were transacted for a total cost of $26.4 million.
* At 3:29 PM - 90 minutes later - another 1,470 contracts were transacted for $26.6 million.
* Net difference was $227,850.

**So by explanation 1**, a buyer of that contract would have spent $26.4 million – not exercised it - and later sold it back to make $228k, or less than 1% return on capital. Keep in mind if the original seller of the contract sold this contact naked – ie did not own the 147k shares agreed upon for this contract – and the buyer had executed, they would potentially lose far more than they gained in premium. 

**By explanation 2**, a buyer would have spent $53 million dollars total on two separate transactions for contracts and then executed to get 294k shares in total. The buyer may have done this if their intention was to obtain shares with minimal effect on share price and the pass the onus on acquiring the shares to the other party. If the writer/seller of these contracts is a MM their ultimate goal is to be delta neutral and provide liquidity. If they agreed to sell these contracts to the buyer it means that they were in a far delta positive and overweight position that they needed to offload nearly 300,000 shares via this one set of contracts alone to lower their exposure. This is a position they should not be in to begin with especially with relatively low volume lately (MM’s move shares between themselves all of the time to maintain liquidity but I’m not aware of a reason they would use derivatives for this than simply block share transactions between dark pools). Keep in mind when you buy a call you may be buying it from another trader or a MM who takes the other side of the trade. With large volume, deep ITM calls like this it is exclusively a contract between one party and the counter party who is willing to take the trade – it’s not just clicking a button on the screen and having it filled. 

**By explanation 3**, two parties prearrange agree upon a particular strike/date (“12c sounds good”) and bounce contracts – and thereby shares – back and forth in a single day with one side taking a small premium. As they are the only ones actively trading these contracts bystanders are unlikely to get caught in the midst and interfere. 

&nbsp;

Overall I think explanation 3 logically makes the most sense although the reality is a little bit of explanation 1 and 2 do also occur. Explanation 3 is the only scenario where both the buyer and seller of the contracts have potential for benefit.

Why? Well lets just speculate for a minute and both Group A and Group B are poorly positioned and short:

* Group A is net short but they are good pals with Group B who is a Broker-Dealer and they do a lot of trades together.
* Group B has been lending shares to Group A to short, but is also starting to rack up FTDs.
* Float is so tight they know if they try to buy shares on the market the price will skyrocket. 
* Both parties know that if Group B cannot source their shares for their FTDs its game over. 
* Group A also has long shares. They coordinate with Group B and sell them deep ITM calls.
* Group B executes to get the fresh shares which they use to close their FTDs or for other use. Lets speculate they are broker dealer/bona-fide MM and they can also generate new naked short shares as needed.
* Group B then sells the same call contract back to Group A, who executes them and gets these “naked shares”.
* The net effect is Broker B has seemed to obtain “fresh shares” via a call contract while Group A’s shares went out for a walk but ended up back home at the end of the day. Group A has the same number of shares they started with and Group B still needs the shares in the future – they just kicked the can. Both remain net short.

*Please note that is speculation on my part and not necessarily what is going on here. It is just my way of trying to make sense and simplify these transactions. It may be the mechanics of this theory are wrong but the underlying transactions still remain bizarre.*

#Unicorn

GME is a unicorn in many ways. Given its rapid rise you will not find many other tickers with contract strikes so far in (and out of) the money. If you look at any other “normal” security you will not see crazy volume on these expensive deep ITM calls. Microsoft, for example, only goes as low as 110 a strike for 4/16 because it is not as volatile although it trades in a similar price range to GME as of late. 

&nbsp;

But for fun, lets glance at A More Comparable ticker:

&nbsp;

This stock closed at 9.36 on 4/1. It has calls starting at $1 strikes on 4/16. A GME call at $12 is actually deeper  in-the-money than the $1 calls for this stock at this time, but lets look at some of the volume for these strikes over the past three months:

*4/16 1.00 Call Highest Daily Volume: 46, OI: 13 on 3/15


*4/16 2.00 Call Highest Daily Volume: 62, OI: 47 on 2/19


*4/16 3.00 Call Highest Daily Volume:  226, OI: 110 on 2/16

I glanced at other dates for this stock at these strikes and lets just say the volume of these deep calls is basically nonexistent. 

&nbsp;

So yes, the volume of these deep ITM calls is HIGHLY unusual and there are no contemporary similarities on the market for this activity. It reiterates that GME remains a market outlier with HIGHLY unusual options activity and large sums of money are being used to conceivably move shares back-and-forth for seconds to a few hours at a time. 


#TLDR:

GME has highly unusual option activity – most noticeably in expensive, deep ITM calls. The order book of these calls seems to often point to “double” contracts indicating that the contracts – and thereby the shares – are being flipped between at least two parties and traded physically on the PHLX floor for dubious reasons. Despite relatively flat price action and low volume the past week, these contracts are again appearing in large quantities, and may indicate large, temporary movement of shares between parties. There are no comparative securities with similar activity as far as I am aware. 

###TLDR 2:

Fun fact: the reason the 4/16 12c always have a flat OI of ~500 is because DFV has not sold 😊

&nbsp;

*This is not financial advice and if you think I have described something fundamentally wrong please message me to discuss so I can correct it*


#Edit: 

[Here is data straight from CBOE showing all of the deep ITM calls from 4/1](https://imgur.com/r7XGvFU). The screen cap data is filtered to just trades on the PHLX and sorted by volume in descending order. Ignore the time stamps as it doesn't display correctly in excel. Trade condition 118 = Single Leg Floor Trade. NOTICE ANYTHING? [Each deep ITM call has a corresponding duplicate trade.](https://i.kym-cdn.com/entries/icons/original/000/027/257/perfectly-balanced-as-all-things-should-be.jpg). These contracts and shares are just being flipped back and forth.