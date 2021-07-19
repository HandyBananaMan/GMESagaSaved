# Author: nydus_erdos
# Post URL: [https://www.reddit.com/r/Superstonk/comments/ol4gv0/short_shorter_ep_3_post_sneeze_and_final_shares/](https://www.reddit.com/r/Superstonk/comments/ol4gv0/short_shorter_ep_3_post_sneeze_and_final_shares/)


&#x200B;

[ALL CREDIT TO u\/ljgillzl https:\/\/www.reddit.com\/r\/Superstonk\/comments\/oeke7u\/short\_shorter\/](https://preview.redd.it/8sz085nc7gb71.png?width=1008&format=png&auto=webp&s=cbc5fdbaf36e1ead99f82badcedaa7fcb4341429)

&#x200B;

# 0. What This Model Can/Can't Tell You

* **What it can tell you:**
   * **An estimate of the cumulative amount of shares ever shorted since 2015 to near present.**
   * **An estimate of the equivalent cumulative SI.**
* **What it can't tell you:**
   * **How many (if any) shares were covered?**
   * **Where are the shares now?**
   * **Wen moon?**

Disclaimer: Not financial advice. I've put a disproportionate amount of time into this for free, I clearly do not make good decisions. Though I continually strive to improve this model it is, at best, just fancier napkin math. I am not an economist, and have no qualifications other than a long time math background. I just like the stock.

# TL; DR => Low: 1.2 billion shares (1,665% SI); High: 2.3 billion (3,322% SI)

\----------------------------------------------------------------------------------------------------------------------------------------------------

# PREVIOUS POSTS, if something doesn't make sense its probably in here:

[Math Black Magic, Vol. 1: Why It Is Mathematically Impossible for Hedgies To Unfuk Themselves](https://www.reddit.com/r/Superstonk/comments/nw8281/math_black_magic_vol_1_why_it_is_mathematically/)

* GENESIS POST
* **TL;DR => Finance professor John Finnerty mathematically proves that it's impossible to short a stock to zero without naked shorting at least as many shares as there are outstanding, doubling the float in the process.**

[Math Black Magic, Vol 2: The Limit Does Not Exist!](https://www.reddit.com/r/Superstonk/comments/nwy0oz/math_black_magic_vol_2_the_limit_does_not_exist/)

* **TL;DR => Naked selling leaves a distinct price pattern and, at this point, the number of shares needed to short $GME to zero does not mathematically exist.**
* 50% conjecture/50% Speculation

[Math Black Magic, Vol. 3: Trillion Short Share Seance](https://www.reddit.com/r/Superstonk/comments/nya5ps/math_black_magic_vol_3_trillion_short_share_seance/)

* **TL;DR => I speculate on how apes fucked up hedgies' algos and make estimates of shares shorted**
* **EDIT: the estimates in this volume are out of date. Check next volume for corrections.**
* 75% speculation/25% conjecture

[Math Black Magic, Final Vol: Epilogue](https://www.reddit.com/r/Superstonk/comments/odrnbv/math_black_magic_final_vol_epilogue/)

* **Short correction for previous volume**
* **TL;DR => I stand by the methods, but they needed more refinement.** **I tightened up the model and got an answer I feel much more confident in.**
* Weak Conjecture

[Malleus Oeconomica: A Compressed Primer](https://www.reddit.com/r/Superstonk/comments/of1lz2/malleus_oeconomica_a_compressed_primer/)

* In Short & Shorter, I use several economic concepts and equations that need a little explaining first.
* **TL;DR => This a short post, but on a wide range of topics. I can't really break it down quickly.**

[The Chronicles of Short & Shorter, Ep. 1: Before the January Sneeze](https://www.reddit.com/r/Superstonk/comments/ogi75b/the_chronicles_of_short_shorter_ep_1_before_the/)

* First step of how I got my revised shares shorted count. I try to recreate their shorting strategy from 2015 to before the January Sneeze.
* **TL;DR => check the bottom of this\^ post itself (its a picture)**
* Conjecture

[The Chronicles of Short & Shorter, Ep. 2: During January Sneeze](https://www.reddit.com/r/Superstonk/comments/oh8fcz/the_chronicles_of_short_shorter_ep_2_during_the/)

* Second step of process. I try to recreate shares shorted during the January Sneeze.
* **TL;DR => check the bottom of this\^ post itself (its a picture)**
* Weak Conjecture

[Short & Shorter, Interlude: Why I Still Think Exponential Floor Guy Is On To Something](https://www.reddit.com/r/Superstonk/comments/oji000/short_shorter_interlude_why_i_still_think/)

* Here I justify my use of the exponential floor equation for price trend data, and give instances from economics that can begin to explain it.
* **TL;DR => SHF broke the law of supply, so apes broke the law of demand, cause fuck 'em thats why!**

# -----------------------------------------------------------------------------------------------

# Uncharted Territory

I feel like I've managed to stay in the conjecture zone up till now, barely at some points, but still in the zone. In this part we're going to probably start violating the speculation zone. Reasons things might get a little weird:

1. This will be our third and fourth iteration. Its very likely that my margin of error grows with each iteration of this process (one wrinkle brained ape estimated that I'm probably at about 10-15% error as of the end of last post).
2. I will stick to Finnerty's equations and theories, but use my own conjecture to apply them.
3. I will be using the exponential trend as price data (justifications in previous post)
4. Past a certain date, ATM offerings would have to be factored in. It adds complexity so I try to cut off the timeframe before it starts happening. I want to integrate these into the model into the future but not now.
5. Price drops get smaller and smaller, making it harder to identify the price drop pattern.

# --------------------------------------------------------------------------------------------------

# Time Frame

The layout for this time frame will be slightly different. Originally, I had planned to identify the price drop pattern, do a normal 3 event shorting cycle, then move on to the next pattern.

As I tried to identify the next full price pattern, no obvious one presented itself. The only substantial price drop consisted of just two points. On top of this, they may overlap with the first ATM offering. However, I am at a woeful lack of data points so I figured a way to include them.

The full 3 event shorting cycle will be called "Leg A", and the 2 event shorting cycle will be called "Leg B".

In earlier posts, I point out what I call a "scramble strategy" in Finnerty's paper. This is when the manipulator is hit by an unexpected positive catalyst and must increase the magnitude of their short attack at time 2 in an effort to compensate. Originally, I said I was not going to use this scenario, but it seems to fit our exact situation.

**LEG A**

* Time 0 - March 12; P(0) = $264.50
* Time 1 - March 15; P(1) = $220.14
* Time 2 - March 23; P(2) = $181.75
* Time 3 - March 24; P(3) = $120.34

&#x200B;

**LEG B**

* Time 0 - March 30; P(0) = $194.46
* Time 1 - April 12; P(1) = $141.09
* THIS LEG ENTERS THE SPECULATION ZONE

# --------------------------------------------------------------------------------------------------

# Multiplicative Demand Shock

>"In economics, a demand shock is a sudden event that increases or decreases demand for goods or services temporarily." ([source](https://en.wikipedia.org/wiki/Demand_shock))  
>  
>"...even if the linear demand is defined in a restrict production range so that the price is positive, with a negative stochastic variation of Y the positive price could become negative (a problem of economic consistency). In order to prevent this, **one alternative is to consider a multiplicative demand shock...**  
>  
>"**A good feature of multiplicative demand shocks, that is, P = Y \* k, where k can be a deterministic demand function**, that is: if Y follow a GBM then the price P also follows a GBM and with the same parameters like drift and volatility! The vice-versa is also valid." ([source](http://marcoagd.usuarios.rdc.puc-rio.br/dema-unc.html))

I will be using this property in the last part of my calculations. My point in mentioning it is there exists a precedent for a multiplying a scalar or another function times your demand curve to simulate a demand shock.

# --------------------------------------------------------------------------------------------------

# Variables & Equations

https://preview.redd.it/mk013zdzfgb71.png?width=947&format=png&auto=webp&s=efd6c42d13394273dff9b5cb019498ddd078031b

[Variables A and H](https://preview.redd.it/5rs7wuxjbgb71.png?width=970&format=png&auto=webp&s=3c0ea973a7a272dd579a2ff6853b7d2560d8705c)

[Elasticity](https://preview.redd.it/3k4jpaotbgb71.png?width=981&format=png&auto=webp&s=74f8f4a627ef5f32f45ea54afa4a5d96acec479f)

# -------------------------------------------------------------------------------------------------

# Growth Rate

>"Exponential functions are unique in that the growth rate of such a function(the derivative) is directly proportional to the value of that function. The constant of proportionality is natural log of the base of the exponential function, ln(b)"

https://preview.redd.it/eb03qpgrcgb71.png?width=966&format=png&auto=webp&s=91ccf2e87b7eb44c0ba35fc9d8d7789a54f1fc8a

![Growth Rates](https://preview.redd.it/yfdqqqyxhgb71.png?width=953&format=png&auto=webp&s=88488ea69e4f3ecd9a1dcf7767b5e4f24ceaf6fd)

# Results

(Share counts in millions)

**Chart 1: Shares Shorted Post Sneeze LEG A**

|Time (t)|Quantity shorted (Q)|
|:-|:-|
|1|230.75|
|2|230.77|
|3|301.42|

&#x200B;

**Chart 2: Totals from Post Sneeze LEG A ONLY**

|Total Shorted Shares by Time 2|461.51|
|:-|:-|
|Total shorted Shares by Time 3|762.94|
|SI within LEG A|1,080%|

&#x200B;

**Chart 3: Cumulative SI After LEG A**

|Cumulative Shares Shorted|1176.9 (1.2 billion)|
|:-|:-|
|Cumulative SI|1,665%|

&#x200B;

**Chart 4: Shares Shorted Post Sneeze LEG B**

|Time (t)|Quantity shorted (Q)|
|:-|:-|
|1|390.62|
|2|781.32|

&#x200B;

**Chart 5: Totals from Post Sneeze LEG B ONLY**

|Total shorted Shares by Time 2|1171.9 (1.2 billion)|
|:-|:-|
|SI within LEG B|1,658%|

&#x200B;

**Chart 6: Cumulative Counts (Pre-Sneeze + During Sneeze + Post Sneeze)**

|Shares Shorted Pre + During|414.01|
|:-|:-|
|Shares Shorted Leg A|762.94|
|Shares Shorted Leg B|1171.9 (1.2 billion)|
|Cumulative Shorted Shares|2348.9 (2.3 billion)|
|Cumulative SI|3,322%|

&#x200B;

**Chart 7: Theoretical Time to Cover High Estimate**

(Got volume assumptions from Barchart)

|Daily Volume Assumption (million)|7.6|
|:-|:-|
|Trading Days to Cover|310|
|Trading Years to Cover|1.2|

&#x200B;

**Chart 8: Theoretical Time to Cover Low Estimate**

|Daily Volume Assumption (million)|7.6|
|:-|:-|
|Trading Days to Cover|155|
|Trading Years to Cover|0.6|

&#x200B;

# Conclusion

This began as a mathematical ritual, so I feel I should end on that note with a bit of mathematical symbolism I found to be prophetic about the ominous doom hanging over Kenny's head.

So, I know I've mapped out several time 3's, but think of those as 'dummy' time 3's I used to help me divide the time frames up in order to make the math easier (think of mini-waves within a bigger wave for the Elliot apes). The REAL Time 3 has yet to come.

In the paper, time 3 is the reckoning. This is when the true value of the stock is revealed and the whole market demand curve shifts. At this point, the manipulator must bankrupt the company or cover and close. That's it.

All the manipulators in Finnerty's model, no matter what the strategy they devise, they ultimately can't keep time 3 from coming. It always arrives. In this model, it is a mathematical certainty.