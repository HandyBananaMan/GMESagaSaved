# Author: jsmar18
# Post URL: [https://www.reddit.com/r/Superstonk/comments/n1w89c/how_hfts_are_creating_the_180_sell_wall_questions/](https://www.reddit.com/r/Superstonk/comments/n1w89c/how_hfts_are_creating_the_180_sell_wall_questions/)


If you don't know me, I tend to write about HFT manipulation. I came across a post that my fellow ape u/SmithEchoes tagged me[ in here](https://www.reddit.com/r/Superstonk/comments/n0ks3g/important_this_is_an_illustration_about_the/). It's a beautiful visual of how HFTs use the shit show of a fragmented exchange market and order types to manipulate stock prices.

# Why should you care?

The "$180 Wall", which is all the rage at the moment is in large part due to what the picture below describes. So educate yourself, and when you write or read your next post about "$x wall" - you can go:

"Hey!! I know WTF your game is HFs, my tits were already jacked and they are now even more jacked!"

As I stickied in a comment[ here](https://www.reddit.com/r/Superstonk/comments/myftqz/david_lauer_former_citadel_employee_is_up_for_an/?utm_source=share&utm_medium=web2x&context=3), fingers crossed we'll get **Dave Lauer** onboard for an AMA who will be able to further highlight and explain manipulative practices that HFTs employ. Personally, I've followed the guy for a while as I work in the same industry as him, so I'm keen to get his valuable thoughts.

# What'll we cover?

**1.** You're gonna read the comic below, a MINIMUM of 2 times, if I see any questions relating to how locked markets work I'm gonna YEET you so far you'll hit the ground harder than GMEs price did in late January (I'll forgive you if you have questions about hide and slide though)

**2.** *Hidden Orders*, this is the specific order type that the comic below describes - let's make sure we drive the point home on its abusive power

**3.** *Add Liquidity Only Orders,* not mentioned in the comic below, and is affected by both[ crossed](https://www.investopedia.com/terms/c/crossedmarket.asp) and locked markets - this is more relevant to the $180 walls we are seeing

&#x200B;

[Read it Twice.](https://preview.redd.it/1vo63u7pvbw61.jpg?width=637&format=pjpg&auto=webp&s=eb3bf4dee8ad50a60022b474b2c12264e26376a0)

# Hidden Orders

&#x200B;

[NYSE Order Type Data](https://preview.redd.it/rc1cwt4svbw61.png?width=688&format=png&auto=webp&s=3d01f3b2bf4a974450b84f157279d33cbf73453a)

This is a chart from one of my older posts that delves into NYSE order type data. Handily enough they provide data on hidden orders. Yep, the order that is described in the comic above!

We already have a base understanding thanks to the comic, but let’s recap.

HFTs can effectively jump the line by posting [“hide not slide”](https://docs.google.com/document/d/1QmoFpdq9HeGJ-cdPP7y808uWxVufJNr2b69J0GY_-SQ/edit?usp=sharing) orders instead of visible orders. This is because a hidden order will not be slidden, resetting the timestamp. So if I placed an order at $120.01 for GME, they then place a hidden order for $120.01 as well from another exchange, I get my timestamp reset due to the market now being locked, but the hidden order does not get their timestamp reset therefore essentially skipping the fucking line. Slightly different wording to the above as I’m introducing timestamps, which is the actual function and how it works.

**Let’s get back to the chart**

These orders haven't just been increasing on the NYSE Chicago (What I define as Shitadel’s stomping ground, will touch on this later) but on every single other NYSE exchange since October-20. To me, I interpret this as some pretty solid evidence of an increase in HFT activity since GME started to gain attention in November-2020.

Especially for the NYSE Chicago. This regional exchange is notably much smaller in volume than the others, as a by-product is much easier to pick up signals of changes in order type behavior.

# Add Liquidity Only (ALO)

To start off, let’s observe the insane increase in ALO order usage within NYSE Chicago… Since…. October 2020. Yep, pretty suss, and it’s been growing ever since ([Check my other post](https://www.reddit.com/r/GME/comments/mf1f6n/i_was_missing_a_key_piece_of_the_puzzel_this_is/?utm_source=share&utm_medium=web2x&context=3) for the IOC ISO order).

&#x200B;

[NYSE Chicago, Shitadel is based there, low volume makes it easy to pick up patterns...](https://preview.redd.it/9g8ro1ucwbw61.png?width=700&format=png&auto=webp&s=5c0d4127a3c2c1672bd8c4d5ba5d6b24f9b0ba2f)

&#x200B;

This is the order I want to focus on and again raise attention to. As it’s relevant to the past week where we’ve seen a pretty obvious wall we keep hitting at the \~$180 mark.

Now, this order type is a doozy and is currently being used for nefarious purposes.

ALO follows a strict “If,then” rule set based on if it **locks** [(7.31(e)(2)(b)iii-iv)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37) OR **crosses** [(7.31(e)(2)(b)ii)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37). This ruleset forces the ALO to perform these trades until it is fully consumed, or the order is canceled. Rule [7.31(e)(2)(C)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37), once ALO is resting on the exchange AND it was forced to change its price in accordance with [7.31(e)(2)(b)i-iv](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37) THEN it now gets to be priced in accordance with [7.31(e)(1)(A)iii and iv](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37). This is the equivalent of HFT when ALO “activates” BUT it comes with a built-in safety feature that IF the price goes UP(Sell ALO) or DOWN (buy ALO) the ALO limit price is no longer locking or crossing at the values it was getting moved to, it REVERTS back to its original limit order price.

**Monke speak translator:** These orders create sell/buy walls (thanks to cross/locked markets and the fragmented exchange market) that have a nifty function that essentially “flips the safety switch” back to the original limit order price if too much buy/sell pressure is applied.

Funnily enough, the NYSE has tried to [amend how ALO orders work](https://www.federalregister.gov/documents/2014/10/16/2014-24547/self-regulatory-organizations-new-york-stock-exchange-llc-nyse-mkt-inc-order-approving-proposed-rule), because of how they can be used for nefarious purposes…. \*cough\* Shitadel \*cough\* The amendment would force to cancel the ALO once it crosses or locked, and not perform how it currently does in accordance with [7.31(e)(2)(b)i-v](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37). Which means no buy/sell wall capability for them to use and abuse.

# How to Fight Back?

# IF YOU ARE HASTILY SCROLLING, SLOW DOWN HERE.

So HFTs can be associated with positives for retail through reduced spreads thanks to the increase in liquidity (arguments exist..). How to fight back?

Don’t buy the liquidity they are selling.

WHAT!? THAT’S AN OPTION? Yeah. 

Imagine the GME bid/ask spread is $180.10/180.20, just say fuck it and don’t pay $180.20 for the shares. Chuck in a limit order for x shares at $180.10 instead. Then whenever someone does come along who wants to sell at $180.10 they will sell to the HFT and then sell to you. (Or set the order at $180.11 to get ahead of the line and you’ll also get a rebate for adding liquidity)

Errrrrrr - but the market moves fast, I’m not gonna be able to keep up with the continuously moving B/A spread!

Fair deuce. I agree. 

Here's where it becomes ironic, what’s the answer? ALO. Yep. The same order HFTs use. By using ALO orders (and I believe a few retail brokers over there in the US allow for this) you can make sure you are not buying what the HFT is selling. 

# 🤯

Defined as part of the ALO, is that they add liquidity only. As such, if you place an ALO buy order at $180.10 and the market does end up moving to sell at $180.10, your order gets rejected (because you ain’t adding liquidity). As a by-product, you will not end up buying from the HFT and just get told, try again - your order got rejected. Rinse and repeat until you purchase your shares.

It cuts the HFT out of the loop. The negative? Surely there is a catch, right?

Execution risk. But it’s not exactly relevant to us lowly retail traders, especially as we’re buying GME. Buy and HODL (not financial advice).

# Summary

These are only two order types, there are also a few more I go into that you can check out in my post history. ALO specifically is relevant to putting a stop to buy pressure which essentially creates these sell walls until we see a reversal. Hidden orders fit into the mix from a… well… angel that I’m not entirely sure of, it’s one cog in a larger machine (algorithm) that we don’t have the full picture on how it functions...

So the *fuck* what? Well, yeah, something we have to live with until it’s properly regulated.

Much like the outcome from u/atobitt and Dr T’s AMA, this helped us get an even better understanding of the shady illegal stuff that goes on. So I’m looking forward to hearing further from Dave Lauer to get the full picture when it comes to HFT.

Lastly, **pitchforks**. We don’t have many ways to poke our pitchforks at HFs outside of HODL. ALO orders are one way we can start to fight back, so if you can - i encourage you to use them. Also, stop placing market orders at the least and start using limit orders (NOT CROSSING THE SPREAD).

# Questions

Now, these are some of the things I'm really keen on understanding Dave’s opinion on: 

* I want to know in which context HFTs use hidden orders
* ALO is one order type, how does it fit into the wider setting of suppressing buy or sell pressure
* Chuck in dark pools, we know how they function, and that HFTs are active within them, how does this fit into the wider strategy? ….. Assuming every piece has its purpose
* IEX combats HFTs to an extent via a delay thanks to a neat spool of fiber optic cable, are there any caveats to this where it can be abused?
* How can we further combat HFTs, given GME is heavily manipulated and is highly volatile due to the diminishing trade volume/liquidity
* And many more…..

# TL;DR

HFTs fuck with GME, causing the $180 price wall as we know. Keen AF for Dave to help provide further context into the issue. ALO orders can be used against HFTs, so if you can, use them (knowing they can get rejected easily due to the B/A moving, so you may have to try multiple times).

Again, shoutout to u/SmithEchoes on collaboration regarding posts delving into order types.