#Title: Where and how Citadel/other hedge funds have been hiding their short positions, and a true estimate of how many short shares are currently being hidden.
#Author: AcedVector
#Post URL: [https://www.reddit.com/r/Superstonk/comments/o7fsqc/where_and_how_citadelother_hedge_funds_have_been/](https://www.reddit.com/r/Superstonk/comments/o7fsqc/where_and_how_citadelother_hedge_funds_have_been/)


Hello there fellow apes! I have an interesting theory to share with you today, that if plausible, would be able to explain how Citadel (and maybe even other hedge funds with massively overleveraged positions against GME) have been hiding the true extent of their short position, as well as give a good estimate of how many shorts they have truly been hiding.

In order to properly explain this, we need to look at another entity that was in a similarly overleveraged position (suffering heavy losses as a result), and who other to perfectly fit the bill than **Archegos Capital Management**.

# The Archegos Capital Management Fiasco:

Archegos, just like Citadel, suffered massive exposure in their positions in the stock market and ended up collapsing with *billions in dollars of losses*. But what exactly were they doing that lead them on this path to utter destruction? Well, according to a [WSJ article](https://www.wsj.com/articles/what-is-a-total-return-swap-and-how-did-archegos-capital-use-it-11617125839), *total return swaps played a large role in how overleverged they were in their positions*.

So what in the goddamn is a [total return swap](https://smartasset.com/financial-advisor/total-return-swap)? I'm glad you asked. A total return swap is basically a contract between two parties (such as a hedgefund and a bank) , where one party makes a series of payments to the other, and in exchange they are receiving the full return of the assets being held by the other party. In essence, one party is paying another to hold assets for them in exchange for the returns the asset would give them, *as if they had owned it themselves*. WSJ has a nice graphic of the process behind it here, given that this is happening between a hedgefund and a bank:

![In this demographic, the hedgefund pays fees to the bank to buy assets for them and gets returns based on the returns of the assets. If the position is highly leveraged, the bank can margin call them and sell their positions if they fail the call.](https://preview.redd.it/kgxpxkz30b771.png?width=666&format=png&auto=webp&s=df8d9cca2d57301e9dcd617c7e7d84f2e875f7e5)

In Archegos' case, they were EXTREMELY overleveraged (as a lot of their positions were concentrated on certain stocks like blue chip stocks), and when they got margin called and couldn't put up the collateral the banks they paid to hold their assets for them sold them into the market, causing *market wide sell offs* in the positions that they held billions of dollars in. This lead to their downfall, and shows why so many people are against total return swaps, especially if you *don't even have to disclose you have them like Citadel and other hedge funds can*.

# How does this connect with Citadel and friends?

It doesn't make sense to say that Citadel or Melvin Capital or any other hedge fund that shorted GameStop had *total return swaps*, because they actually *were* in ownership of their short positions. However, as I was scouring the sub, I came across a [post](https://www.reddit.com/r/Superstonk/comments/o776lz/i_know_exactly_who_is_holding_the_05_puts/h2x1333/?context=3) (its worth checking out) that had a nice comment by u/taimpeng that goes into detail on how there could be the exact EQUIVALENT of a short position using *synthetic return swaps*: return swaps between a synthetic prime brokerage and a hedge fund that hedge funds can use to gain massive leverage (similar to Archegos using total return swaps to gain massive leverage on their positions) , that would effectively allow them to have a short position without *actually* owning the short position.

![Seriously, give this man an award! This is gold.](https://preview.redd.it/vaq7xmm88b771.png?width=890&format=png&auto=webp&s=7b2fb7cba925f9d0f82743af182556378aba09af)

Taimpeng here basically states that through netting by novation, its possible that hedge funds like Citadel, Melvin Capital, and other hedge funds can essentially say that they have "closed their short positions", but effectively just create an equivalent of the short position by entering into a contract with a synthetic prime broker to say, "hey, we want you to *swap* our short shares with OTM put contracts. We'll hold the OTM puts and we'll pay you to keep hold of our short shares." This would, in effect explain how those 0.5$ strike July 16th puts appear in the options chain, and why it looks like GME isn't as shorted as it **actually** is. It helps to explain the FTDs to some extent too as a lot of these shares could have been nakedly shorted, but put under the veil of these put contracts that makes it look like the shares actually exist. If this is the case, then we can go down the options chain to all OTM puts of the like and find an estimate of the equivalent accumulation of short shares that the hedge funds have worked together to hide through these OTM put contracts (at least the ones in the option chain that haven't expired) , so l took the liberty of finding where most of these are (this is using [yahoo finance options data](https://finance.yahoo.com/quote/GME/options?p=GME)):

![This is for July 16th. Basically what I'm doing is sorting by open interest and adding up the highest ones \(as in thousands of open interest\) on expirations that have suspicious  OTM low strikes like there are here.](https://preview.redd.it/ff7un4tohb771.png?width=816&format=png&auto=webp&s=9d387eac1f293050e32b20f222d50a936f144c69)

For reference, here is what the puts on a options expiration date is *supposed* to look like:

![Here, the open interest shows up low overall on strikes OTM like 10$ and 50$ which don't signify much suspicious activity at play.](https://preview.redd.it/nyn2273gnb771.png?width=812&format=png&auto=webp&s=d9353baa9c0735eaca9cc12e0ca83eb5a97e7cce)

I will now show you the rest of the dates that these suspicious OTM put open interest appears:

![October 15th, 2021](https://preview.redd.it/hcigmh0skb771.png?width=829&format=png&auto=webp&s=d7cd0bff9bed635400694fad7d8053a9888aa9c2)

![November 19th, 2021](https://preview.redd.it/hqkcs5hclb771.png?width=823&format=png&auto=webp&s=3c0ebe3528cf42b396209dd3de6a8d07612239b1)

![BIG one for January 21, 2022](https://preview.redd.it/a7mguofbmb771.png?width=830&format=png&auto=webp&s=fb2711873a2e93b658ee41976308ba9a8b4f2169)

![January 20, 2023](https://preview.redd.it/r5uoay4vmb771.png?width=816&format=png&auto=webp&s=7e6246ee344e1c4b73a66cf41b32d06038ba62dd)

After crunching the numbers, here is a table of what I found:

&#x200B;

|Options Expiration|Approximate Suspicious OTM Put Open Interest Total|
|:-|:-|
|July 16th, 2021|408,746 put contracts|
|October 15th, 2021|27,433 put contracts|
|November 19th, 2021|35,689 put contracts|
|January 21, 2022|267,336 put contracts|
|January 20, 2023|56,776 put contracts|
|Total:|795,980 put contracts|

HOLY SMACKEROOS that's a lot of put contracts, and that's just the ones that I could find! There could be a lot more put contracts they spread out that I couldn't find over other expiration dates, these are *just the put contracts where the put open interest stands out suspiciously on low strikes*. For the grand total number suspicious put contracts being at approximately 795,980 put contracts, in terms of shares that would be... **79,598,000** shares short. Not as high as you would think, but also keep in mind that this does NOT include the shorts they have covered already through FTD buy ins in the FTD cycle, as well as shares short they could be hiding through other means that we don't know about. If we were to calculate the short interest based on current data, we would have:

79,598,000 shares short / 70,800,000 [shares outstanding](https://finance.yahoo.com/quote/GME/key-statistics/)  ≈  **112% short interest**

Quick edit: This is the short interest based on OTM Put data ALONE. If you were to add the short shares currently reported ([9.67M](https://finra-markets.morningstar.com/MarketData/EquityOptions/detail.jsp?query=14%3A0P000002CH&sdkVersion=2.59.1) according to Finra data) on top of this, the *revised calculation* would be:

89,268,000 shares short / 70,800,000 [shares outstanding](https://finance.yahoo.com/quote/GME/key-statistics/) **≈ 126% short interest**

**AND THIS IS STILL EXCLUDING GOD KNOWS HOW MANY SYNTHETICALLY CREATED SHORTS EXIST.**

# QUICK EDIT AGAIN: I've recently just read u/criand 's  [post](https://www.reddit.com/r/Superstonk/comments/o7klxj/looks_like_the_recent_robinhood_class_action_si/?utm_source=share&utm_medium=web2x&context=3) that goes into depth on the deep ITM CALL side of options (Side Note: I find it weird that these contracts were around the same strike prices too for both puts and calls, makes me think we can get an idea of the strike prices of their short position based off that, just some food for thought), and I think everyone should take a look at THAT as well as it is most definitely a good read. Just for shits and giggles, I've decided to include the call side of the shares shorted based on his post to grab a good estimate of the synthetic shares overall.

According to his post, approximately 1,100,000 calls in open interest were present (this is during January) , or **≈ 110,000,000 shares overall on the call side regarding suspicious deep ITM calls.** SO, to add that on top of the already existing shares short we have:

# 199,268,000 shares short / 70,800,000 [shares outstanding](https://finance.yahoo.com/quote/GME/key-statistics/)  ≈ 281% Short Interest

# Edit: saw some comments asking to do short % of float so here it is

79,598,000 shares short / 55,480,000 [float](https://finance.yahoo.com/quote/GME/key-statistics/)  **≈ 143% of float shorted**

Revised calculation:

89,268,000 shares short / 55,480,000 [float](https://finance.yahoo.com/quote/GME/key-statistics/)  **≈ 160% of float shorted**

# Calculation including the deep ITM CALL side from criand's [post](https://www.reddit.com/r/Superstonk/comments/o7klxj/looks_like_the_recent_robinhood_class_action_si/?utm_source=share&utm_medium=web2x&context=3):

# 199,268,000 shares short/ 55,480,000 [float](https://finance.yahoo.com/quote/GME/key-statistics/) ≈ 359% of float shorted

That is a MASSIVE amount of short interest, and shows that **GME is still very much being manipulated even if we can't see it on the surface**. If they have to buy all of these shares at once  when we quite possibly own the float MULTIPLE times over, they would have to buy approximately 199,268,000 shares ***MULTIPLE TIMES.*** The share price would *definitely* go into the millions in that circumstance (at least in my opinion), and we KNOW the hedgies can pay it too. ***BUY AND HODL.***

# Post DD Message:

Thank you guys again for reading my DD! :) On this DD I felt motivated to find out what the hedgies were hiding in terms of short shares, as I felt left in the dark as to what was happening overall and there was a lack of explanation for *a lot* of things in my mind. This theory only manages to explain a little, but I hope what I found was helpful to you guys and maybe give you a little confirmation bias going forward. It's hard going against the grain, where there are so many people around you that think "oh GameStop is done" and "the squeeze has been over for months now", so I truly applaud each and every one of you that have been hodling with those diamond fucking hands of yours. Anyways, it's getting pretty late right about now, so I think that's gonna be about it for this DD. I'll try to hang in the comments before going to bed but I hope you guys have a nice rest of your day!

&#x200B;

EDIT: ~~WTF? THE OPTIONS CHAIN IS BEING HIDDEN NOW..? I have no clue. This could just be because its late and the computers are resetting or something but its suspicious to me.~~

EDIT 2: I've been seeing in the comments that yahoo finance seems to regularly have this phenomenon with their data at night (open interest data resetting). I've removed the images just so the post is a little cleaner now and doesn't stir confusion regarding the data.