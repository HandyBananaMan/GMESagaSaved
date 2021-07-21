# Title: I think I know what the OTM puts are for
# Author: theyellowfromtheegg
# Post URL: [https://www.reddit.com/r/DDintoGME/comments/oo2lrk/i_think_i_know_what_the_otm_puts_are_for/](https://www.reddit.com/r/DDintoGME/comments/oo2lrk/i_think_i_know_what_the_otm_puts_are_for/)



**[edit 5: u/sweatysuits seems to have independently come up with something very similar - they even made illustrations visualizing the scheme. Go visit their post: https://www.reddit.com/r/Superstonk/comments/onn69e/gutof_connecting_the_dots/]**

**[edit 4: Fully Revised Post - I might have gotten cause and effect for the synthetic long wrong. And in practice, this thing might be a bit more complicated than initially thought. But this theory fits well with some of the observations.]**

Premise: You're anything but a market maker. Let's call you S. A long time ago, S borrowed x stonk from Lender L. The price of stonk was 1$. S went short on stonk by selling x of it for 1$ (in the following: *the initial short sale*).

The original problem: Stonk is now at 10$. S is margin called by lender L. S needs to post collateral. S is fucked. S has not enough money to meet the margin call. S needs at least one of the following: (1) The stonk price to go down. (2) Enough money to meet the margin call. Both would be even nicer. S still would like to make money on the *initial short sale*. 

The obvious solution: Just short x stonk at 10$ now, driving down the price and getting you enough money to meet the margin call.

The other problem - the locate requirement: 17 CFR § 242.203(b)(i) requires broker-dealers

>prior to accepting a short sale order in an equity security from another person, or effecting a short sale in an equity security for their own account, to borrow the security, enter into a bona-fide arrangement to borrow the security, or have reasonable grounds to believe that the security can be borrowed so that it can be delivered on the date delivery is due.

S's broker dealer can't borrow any of that precious stonk. S is also not a market maker. S does not profit from the excemption from the locate requirement for bona-fide market making pursuant to 17 CFR § 242.203(b)(iii). S thinks they're fucked.

The not so obvious solution - the exception under 17 CFR § 242.203(b)(ii): The locate requirement does not apply

> to any sale of a security that a person is deemed to own pursuant to § 242.200, provided that the broker or dealer has been reasonably informed that the person intends to deliver such security as soon as all restrictions on delivery have been removed. If the person has not delivered such security within 35 days after the trade date, the broker-dealer that effected the sale must borrow securities or close out the short position by purchasing securities of like kind and quantity.

One way to "own" a security, even if you're not net long, is defined in 17 CFR § 242.203(d):


>A broker or dealer shall be deemed to own a security, even if it is not net long, if:

>(1) The broker or dealer acquired that security while acting in the capacity of a block positioner; and

>(2) If and to the extent that the broker or dealer's short position in the security is the subject of offsetting positions created in the course of bona fide arbitrage, risk arbitrage, or bona fide hedge activities.

Here things get a bit tricky and I might not understand correctly. But S needs a broker or dealer willing to take on their position. Let's call them B-D. [Investopedia](https://www.investopedia.com/terms/b/block-positioner.asp) defines a block-positioner. Interesting how they talk about dark-pools...

Anyway, assume B-D in the capacity of a block positioner has taken on S's *initial short-position*, probably because they also risk defaulting when the stonk rises even further, cause they're in on the shorting. Remember when most of these GME OTM puts were opened? Jan 27... So B-D has fulfilled requirement (1) of 17 CFR § 242.203(d), but they also need to fulfill requirement (2) - the bona fide hedging activities. How does one hedge a short opened at 1$, when the stock is at 10$? Enter the synthetic long at 1$ - which involves the purchase of a call at 1$ (now deep ITM) and the sale of a 1$ put (now deep OTM). And now B-D is free to sell short x stonk at 10$, roughly offsetting their initial cost for the deep ITM calls. They may have the money to just outright buy those ITM calls - but they also need the stonk to go down. They also still need to cover the margin call of the *initial short position* they just took on. Again, B-D may have the money for the margin call, but B-D was in on the shorting and also needs the stonk to go down. So they excercise those deep ITM calls and immediately sell the stock. Voilà - the deep ITM call OI disappeared. B-D also has collateral to cover the margin call. Plus, B-D just added selling pressure of twice the *intial short position*.

The T+35 comes in: B-D has sold x stonk short at 10$ that they were deemed to own, thus not requiring to locate it in the first place. 17 CFR § 242.204(a)(2) now gives B-D 35 days to close the FTD. Sound familiar?

The buy-writes come in: B-D either doesn't want those FTDs to show up in the first place or needs to close them in time. They call their market maker friend MM and agree to perform a buy-write, where MM sells x stonk to B-D and B-D sells a deep ITM call for x stonk, which after pretending to have closed out the FTD gets immediately excercised so that MM gets back the stonk.

We now have a theory that explains:

- the high OI of deep OTM puts, with no equivalent OI of deep ITM calls
- the date when the OI of those deep OTM puts skyrocketed
- the buy-writes we've been seeing pop up
- the smaller SHFs testifying to have closed out their short positions (S's *initial short position* has been taken on by B-D)
- something with dark pools (the part where B-D is acting as a block-positioner which I don't fully understand and probably is the weak link in all of this)
- some juicy T+35

Now go ahead and poke holes in all of this, my head hurts. Cheers. I'm no longer sure if this week will be a wild ride, but I see green crayons which is nice.

_______________________________________________________________________________________
Original Post:
_______________________________________________________________________________________


[edit 1: corrections regarding delivery - cancelled parts marked with ~~striketrough~~ - added parts marked with *italics*]

[edit 2: clarification regarding motivation]

**[edit 3: major revision incoming - stay put]**


These OTM puts had me thinking all weekend, but I think I have found a solution.

**IMPORTANT EDIT** *The solution starts with the premise that you have a short position that you opened with borrowed stock at a price a fraction of the current share price, for which you are now being margin called. Else, opening a synthetic long with deep ~~ITM~~ OTM puts makes no sense.* [edit 2]


A synthetic short involves the purchase of a put and the sale of a call, both at the same strike and expiration. Now, why are all examples you can find on the internet using ATM puts and calls? Because it assumes that your going short **at the current price**. Which also means that the premiums for those options are roughly equal, i.e. it doesn't cost much to go synthetic short.

A synthetic long is the opposite of this strategy, you buy the call and you sell the put. Same strike, same expiration, both ATM.

But why would you enter a synthetic long or short position with a combination of deep ITM calls and deep OTM puts? **Because you're trying to offset a short position that was opened at much lower prices!**

Imagine you've borrowed x stonk at 1$ to short it. Now stonk is at 10$, highly illiquid and your lender has marge call you. What are do you do? **You pretend to be net balanced**. You open a synthetic long of x stonk at 1$, i.e. buy enough 1$ calls and sell an equal amount of 1$ puts. So you can now call your lender and tell them all is fine, your borrowing of the stock was just a hedge for your synthetic long! No matter what the price of the stonk, there's always the possibility to get it back for 1$. If the call stays ITM, just exercise it. If the put goes ITM, someone else is gonna exercise it. Either way, x stonk at 1$. Lender is happy.

But how come those 1$ calls are nowhere to be seen? Well... How much is a 1$ call per share if the stonk is at 10$? Well roughly 9$ per share. If you had that much money, why not just post that as collateral? You're a hedgefund, so what do you do when you need money? **Short the fucking stonk**. So you naked short x stonk at 10$, which is like hitting two birds with one stone. It gives you money for the ITM calls **and** helps drive the price down, lowering your margin requirements.

But wait... What about the T+2 settlements date? You don't intend to deliver those shares, do you? Of course you don't. ~~Guess what, you don't have to.~~ *Guess what, you just bought yourself 35 days* [edit1]! 17 CFR § 242.200(d)(2) to the rescue. ~~You're original short with the borrowed stock isn't a short sale under Reg SHO.~~[edit1] And your new naked short position is a legitimate hedge against your synthetic long. Mark it as short exempt! *And enjoy that sweet, sweet T+35 pursuant to 17 CFR § 242.204(a)(2).* [edit1]

So that still leaves the ITM call in existence... What do you do with it? Exercise it of course. And then you sell x stonk at 10$ to further push the price down. Leaving you with a lot of cash on hand, which you can post as collateral for your initial short, or shove it up your butt, whatever. Or maybe it goes into RRP...

*But what about the T+35, when you have to deliver those x stonk sold at 10$? Enter the well-known buy-write using more deep ITM calls to kick the can another T+35* [edit1] 

So. That's why we see all those OTM puts but no ITM calls and tons of money in RRP. When does the whole thing come crashing down? When the puts expire... Leaving you net short on x stonk you sold naked at 10$ in addition to the x stonk you shorted at 1$ ~~and need to return to the lender~~ *your lender now wants new collateral for* [edit1].

We're in for a wild ride this week.