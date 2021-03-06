# Title: When Kenny Sneezes the Market Seizes, Part IV: Lock, Stock, & Two Crossing Markets — Taking an X-ray of GME's price data to reveal HFT and algo-trading activity
# Author: G_KG
# Post URL: [https://www.reddit.com/r/DDintoGME/comments/opb59e/when_kenny_sneezes_the_market_seizes_part_iv_lock/](https://www.reddit.com/r/DDintoGME/comments/opb59e/when_kenny_sneezes_the_market_seizes_part_iv_lock/)


Previous Chapters in this book:

1. [11 Red Flags of Gaslighting](https://www.psychologytoday.com/us/blog/here-there-and-everywhere/201701/11-red-flags-gaslighting-in-relationship)  (hi hedgies and Gabe's data scientists 💕😘)
2. [Intermarket Sweeps](https://www.reddit.com/r/Superstonk/comments/ok1bta/the_intermarket_sweep_aka_the_straight_upanddown/?utm_source=share&utm_medium=web2x&context=3), the **COMMON** trade type causing ~~vertical lines~~ glitches
3. [The Glitchening](https://www.reddit.com/r/Superstonk/comments/omegu8/when_kenny_g_sneezes_the_market_has_a_seizure/?utm_source=share&utm_medium=web2x&context=3), WHY we can believe the data- **what you see with your eyes is REAL**!
4. [Going Cross-eyed with Crossed Markets](https://www.reddit.com/r/DDintoGME/comments/onka1q/when_kenny_sneezes_the_market_has_a_seizure_part/), when the **BID** is **HIGHER** than the **ASK**

Hello ~~ladies~~ ape-ettes and apes, I'm back from safari!!  That wild glitch hunt was .... WILD!  Ya know how when you're on safari, scanning the horizon for rare and exotic beasts...  then suddenly your field of vision goes dark, you pull down your binoc's to curse at your husband (or boyfriend) for blocking your view, and.......     you realize *you're staring right into the asshole of a motherfucking unicorn???*

Okay full disclosure I don't know what that's like either, but I IMAGINE it would feel something like watching last night's $$$ battle at GME's closing and seeing ***everything*** **you were looking for** ***happen all at once***\*\*.\*\*  My tits are still sore from being so jacked 😮

*But first!!* Let's use a price analysis from 4/12 (when GME's price shat all over everywhere and dropped from $165 to $140 between 9:30 and 10:00) to explain the fancy new visuals.  Here's a quick refresher on what 4/12 looked like-

![I can still taste the dimension of pissed off I visited that day](https://preview.redd.it/h7eit1eszlc71.png?width=827&format=png&auto=webp&s=7656a67b48d2b7f36a78215a5325478e579b32ba)

***Here's what ACTUALLY happened from 9:30 to 10:00 that day-***

![Try to let the \\"oooo pretty\\" soothe away the \\"wtf\\"](https://preview.redd.it/na1tsem68pc71.png?width=1773&format=png&auto=webp&s=61c4177c0be8a0686c8d1481ce557254259f0356)

try to let the "ooooo pretty" soothe away the "wtf"

What's the lock?  I didn't talk about [locked markets](https://www.investopedia.com/terms/l/lockedmarket.asp) in my [last post about crossed markets](https://www.reddit.com/r/DDintoGME/comments/onka1q/when_kenny_sneezes_the_market_has_a_seizure_part/), but they're the same concept as a crossed market (bid $ HIGHER than ask $) except it's when the bid EQUALS the ask.  (Fun fact: the order protection rule is [supposed to protect against crossed and locked markets](https://www.finra.org/rules-guidance/rulebooks/finra-rules/6240). There are exceptions, but I don't know anything more about this.)  Volume is shown at the bottom of the graph; odd-lot volume is overlaid on top of total volume so you can see just how much of the overall volume is from odd-lot trades.  **EACH** one of those crayon-dot-lines is a moment in trading-time where the price of the trade landed ***outside*** the bid:ask range, aka [the national best bid/offer (NBBO](https://www.investopedia.com/terms/n/nbbo.asp)), by over 1% of the average spread.  (If, like me, you're noticing how many of them seem to line up with steep price drops, .....   yeeeaaaaa.)  (The data used is from a level 1 feed that [we know to be an accurate](https://www.reddit.com/r/Superstonk/comments/omegu8/when_kenny_g_sneezes_the_market_has_a_seizure/?utm_source=share&utm_medium=web2x&context=3)\- accuracy of data source has been verified vs Bloomberg terminal data.)  [**Most of these instances are due to trades called intermarket sweeps**](https://www.reddit.com/r/Superstonk/comments/ok1bta/the_intermarket_sweep_aka_the_straight_upanddown/?utm_source=share&utm_medium=web2x&context=3)**,** a very common type of institutional trade.  The green and red crayon-dots have trade volumes of over 100.  The blue and purple crayon-dots are **odd-lot trades** outside the NBBO are only *probably* market sweeps because without a better data sub I can't see for certain if they have the "*IS/trade-through exempt/611 exempt"* trade condition which would confirm that these are sweeps (I'm a poor).  These data points could *also* be trades with prices drifting outside of the NBBO due to some [completely random and definitely unintentional instance of the NBBO calculator getting overloaded with too many trades](https://www.investopedia.com/terms/q/quote-stuffing.asp).

Here's why it's super fun to differentiate the two:  *Unlike large trade orders, odd lot trades don't enter into the NBBO calculation.* They're not technically protected under the order protection rule, either (though as a retail trader if you've got a decent broker they will execute your trade at best prices).  Why?  Because.... um.... reasons.  u/incandescent-leaf is the brain here, I just wield the crayons.

So let's show the graph again, but this time with only HIGH volume sweeps that DID affect the price calculation:

![Yup, looks like they affected the price](https://preview.redd.it/tn5bparm8pc71.png?width=1769&format=png&auto=webp&s=9b0c1c3ec16eb11cf18eb4ef70ed2e072ee9c521)

Here's the sweeps+ that were ODD LOTS and did NOT affect the price calculation:

![Selling peaks and buying dips? I see you, trading algos :D](https://preview.redd.it/rtf59mv59pc71.png?width=1765&format=png&auto=webp&s=58a49173a80845354fe9ee414ffd0a6caa98ee91)

Here's sweeps+ that landed outside the NBBO that were **1-share trades**:

![if you're giggling because there's barely any difference, me too](https://preview.redd.it/s5q6mppibpc71.png?width=1761&format=png&auto=webp&s=13af4304d696f6783839f8126f046c88ce8745ed)

Let's zoom in on that *especially* spicy shit-show around 9:44-

https://preview.redd.it/tpkjr1whgpc71.png?width=1729&format=png&auto=webp&s=f6c485e3f3a197bef22a1e0effe46a791bda005d

Looks like a game of "push the price with big volume and then scalp with odd-lot sweeps" if you ask me.  (I can haz this video game??)

High volume sweeps which DID affect the price-

![definitely affected the price](https://preview.redd.it/5zcg6ulpgpc71.png?width=1734&format=png&auto=webp&s=4268dc2ef5f1ec255d02fea86a528c109d7ead2f)

Sweeps+ which were ODD LOTS and did **not** affect the price-

![algos go nom nom nom](https://preview.redd.it/9h6mdw8vgpc71.png?width=1734&format=png&auto=webp&s=1f9410d1cc283f5e2f9fb247ab8f60c20f2b3529)

And the 1-share trades only-

![TF are with these little bands\/packets of 1-share trades?](https://preview.redd.it/w5trhtjzgpc71.png?width=1730&format=png&auto=webp&s=8724238317599e58dbd587309bb494ef973da69d)

Now that the appetizer round is finished, on to the main course- taking a peek behind the surface at what in the HELL happened during the last 20 minutes of trading on Tuesday (7/20).

![that middle part makes me giggle](https://preview.redd.it/2tot6111xpc71.png?width=1732&format=png&auto=webp&s=c881d697e7323c99996372039d5cd1ef1e9ae95d)

Now THIS tells a story.  GME had just broken out of the boring-ass price channel it was trading in and was headed on up (to $200 is what I thought, its last major resistance/support).  Trading algos and HFTs were loving life and gobbling it all up, sweep-to-buys during the dips (and whenever the stock needed a little "boost" in the right direction), sweep-to-sells during the peaks, and scalping with odd-lot sweeps along the way (to make the moneys but not disturb the price in any way).  Everything was great all the way up until exactly 15:48:24 ET, when trading got *weird* and then- [the market locked](https://www.investopedia.com/terms/l/lockedmarket.asp).  😮

What ensued afterwards can only be described as pure chaos.  At first, the trading algos and HFTs thought this was a VERY good sign, and two large-volume sweeps came through.  Then....   a wave of pure shit-fest. Sweep-to-sells like **crazy** with HUGE volumes that visually dragged the price down.  Followed by rapid-fire sweep-to-buy ODD LOT trades that wouldn't affect the price.  Followed by more HUGE volume sweep-to-buy orders that tugged the price down each time.  Let's zoom in on the shit-storm, shall we?

![holy sweep-to-sells, batman](https://preview.redd.it/uk1octk6cqc71.png?width=1714&format=png&auto=webp&s=592a1a40584cd84482814a75a4d7a1eda7f1e6c2)

So....  either **a)** trading algos and HFTs decided to break up a perfectly predictable and delicious upward price movement that they were VERY clearly making money on for ...magical.... reasons, or **b)** some entity was using massive sweep-to-sell orders to stifle the upward movement of the stock.  *Hmmmm.*

**It gets better!!**  Look at the volume-per-price distribution of these four ETFs, the IWM (rus 2000), IWN (russ 2000), IWF (russ 1000) and XRT (a SPDR retail ETF known to be used for GME stock).

![They're samsies!](https://preview.redd.it/5im3fyghfqc71.png?width=627&format=png&auto=webp&s=ba32f1184cf4c056fdc798d264c8b9a6675849d6)

Remind you of anyone??

![GME's shit-storm](https://preview.redd.it/uki9d1m8gqc71.png?width=323&format=png&auto=webp&s=23b1823b37ee8c342c0f0a51c3fc681fa22fa129)

X-ray Time!!  GME for reference once more:

https://preview.redd.it/uk1octk6cqc71.png?width=1714&format=png&auto=webp&s=592a1a40584cd84482814a75a4d7a1eda7f1e6c2

Let's start with the tiniest ETF first, the IWN, mid-storm:

https://preview.redd.it/fhz91h5omqc71.png?width=1727&format=png&auto=webp&s=99c7ba2820f74a716376d8117e15f2c862a40c40

Lots of locked market there- and one REALLY significant sweep to sell around 15:53.

IWF mid-shit-storm:

https://preview.redd.it/03crh0gllqc71.png?width=1752&format=png&auto=webp&s=18dc8a7f5610ffab08202129fec927b700df0eca

Looks like the action here really picked up in the latter portion of the storm, holy crap. TONS of market locking and high-volume sweeps.

Here we have XRT:

https://preview.redd.it/ps088znpnqc71.png?width=1722&format=png&auto=webp&s=c717506ea044131485e945b49f1ced4c81361b5c

*Oh lookie who had a market crossing around the time that GME locked??*  🤣  Sweep to BUYS like CRAAAAZY.  I wonder if someone was snatching up ETF baskets for some tasty GME??

Finally, IWM during the time of the shit-storm:

https://preview.redd.it/qepbrejjkqc71.png?width=1733&format=png&auto=webp&s=a35f1779c2f10a7bca68cceec14f697a4c92bca8

Uhh.   Uhh?  Holy crap.  And I thought GME was having a shit-storm.  HOLY crap.

*ANYWAY*, if more clever wrinkles had ideas of what ETFs might be REALLY interesting to also inspect for this time frame, let me know!!  I'm no expert here- just with crayons 😁 I can make a follow-up post with all the requested ETFs since this post is just about at image limit.

# TA-DR: Straight-line thingies (aka "glitches") are actually the result of market sweeps done by HFTs and algo-trading. Plotting the sweeps shows what a big effect they have on price movement...  but ONLY when hedgies want to, because we can ALSO see sweeps made of odd lots used to NOT change the stock's price.  Sweeps can also be used to judge what ETFs are being bought and dismantled/shorted to smush GME's price.  hi kenny ❤💕

&#x200B;

![DEFINITELY SUPER KIDDING ABOUT ANY \\"ILLEGAL\\" ACTIVITIES.  It's probably just these quality extracts talking- I've processed a magenta crayon into sugar wax and have been DABBIN THAT SHIT ALL NIGHT](https://preview.redd.it/7fmlbzkrllc71.png?width=1177&format=png&auto=webp&s=0dd04eea59a50f89489a3bb1142bddb89c1d7f3b)

**Acknowledgements:**

I've been busy taking the suggestions of people smarter than me.  u/incandescent-leaf and u/pubertus had both been looking into odd lots and 1-share trades outside the NBBO- ***This shit looks so much better now, thanks you two!!!***  It's important to state here that **yes, intermarket sweeps CAN happen in odd lots, and do all the time.**  Because I am working with free data, I can't indicate which trades were officially marked as sweeps.

Also, big shout-out to u/AlarisMystique , u/No-Fox-1400 , and u/incandescent-leaf for suggesting this sweeps activity was related to ETF destruction/reconstitution and could be crucial to the method Kenny uses to short stocks with ETFs.  ❤  I'll keep making pictures, you guys keep having great ideas! Additionally, u/2Girls1Fidelstix taught me that the market-wide sweeps that occur around 4:42pm may be due to futures market hedging.  Sweeps are ***apparently*** part of normal trading patterns ***every day***.  *(I'm still tickled by the fact that so many of us are learning for the* ***first time*** *that sweeps even exist, they're still being called "****glitches****" by hedgies, yet they're a* ***totally normal part of trading flow every day***\*.  lmfao.)\*  There is a BIG sweep every morning around 8am (also 4am, 4:40-ish pm, and 7:30pm) which I *also* expect to be related to some totally normal thing- will edit with info when I get it!

Full disclosure, the only things I do well are 1) learn from criticism + mistakes, 2) repeat what other people teach me and, and 3) draw pretty patterns with crayons.  Thanks to the following wrinkle-brains whose posts/critiques/willingness to share knowledge provided the smarts behind everything. First: **SECRET FRIENDS** (I 💕 you all, ask and you will be immediately un-tagged ❤)  u/pubertus , u/incandescent-leaf , u/AlarisMystique , u/No-Fox-1400 , u/2Girls1Fidelstix , u/Sgt-GiggleFarts (helping me look towards max-pain price theory), u/Defeat3r (pointed out the bizarre behavior of the CFD of the rus-1000, still mushing my brain around this wrinkle), u/Leenixus (ETF story!) , u/BuzzMonkey (price correlations!), u/VoxUmbra (ETF arbitrage!), u/Criand ,  u/Doom_Douche , u/broccaaa , u/valso34 , u/apegoneinsane (i need your brains to see if these pics support any of your theories!)  u/PWNWTFBBQ (do you see algos at work in the pics above??)  u/Blanderson_Snooper (any chance this helps you track ETF arbitrage?) u/HomeDepotHank69 (can your quant army make use of these visuals??)   ❤💕❤💕🦍🦧🐱‍👤💎🙌