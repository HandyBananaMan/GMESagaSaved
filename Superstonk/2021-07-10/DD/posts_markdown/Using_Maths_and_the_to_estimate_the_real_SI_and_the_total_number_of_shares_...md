# Author: ThrilHouse83
# Post URL: [https://www.reddit.com/r/Superstonk/comments/ohqka0/using_maths_and_the_to_estimate_the_real_si_and/](https://www.reddit.com/r/Superstonk/comments/ohqka0/using_maths_and_the_to_estimate_the_real_si_and/)


Hi all, I wanted to repost this fantastic DD from yesterday that seems to have gotten completely lost in the avalanche of karma farming lego meme's. All credit goes to [u/nydus\_erdos](https://www.reddit.com/user/nydus_erdos/). This is part two of his series, both posts are top tier IMO and deserve more love. You can find them here:

[The Chronicles of Short & Shorter, Ep. 1: Before the January Sneeze](https://www.reddit.com/r/Superstonk/comments/ogi75b/the_chronicles_of_short_shorter_ep_1_before_the/)

[The Chronicles Of Short & Shorter, Ep. 2: During the January Sneeze](https://www.reddit.com/r/Superstonk/comments/oh8fcz/the_chronicles_of_short_shorter_ep_2_during_the/)

&#x200B;

The TLDR is that u/nydus_erdos is using the Finnerty formula to estimate the total number of cumulative shorted shares and the total SI up to the Jan "sneeze". SPOILER ALLERT: the number of shares will jack your tits into the thermosphere.

Again, all credit for this amazing DD goes to OP and anyone that enjoys the content should show his posts some love. Anyway onto the content:

(EDIT: to fix formatting and add the TLDR meme from original post. Im honestly so happy that people are looking at this and discussing it. Please show the love to OP u/nydus_erdos as he deserves all the credit!!) 

(EDIT 2: Just noticed my brain fart in the title lol. Clearly my brain is much smoother than OP’s. Hopefully the content makes up for it)

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

&#x200B;

&#x200B;

Disclaimer: Not financial advice. I've put a disproportionate amount of time into this for free, I clearly do not make good decisions. Though I continually strive to improve this model it is, at best, just fancier napkin math.

\--------------------------------------------------------------------------------------------------------------------------------------------------------

Quick Descriptions of my Previous Posts, if something doesn't make sense its probably in here:

[Math Black Magic, Vol. 1: Why It Is Mathematically Impossible for Hedgies To Unfuk Themselves](https://www.reddit.com/r/Superstonk/comments/nw8281/math_black_magic_vol_1_why_it_is_mathematically/)

* If you only read one post, read this one
* **TL;DR => Finance professor John Finnerty mathematically proves that it's impossible to short a stock to zero without naked shorting at least as many shares as there are outstanding, doubling the float in the process.**

[Math Black Magic, Vol 2: The Limit Does Not Exist!](https://www.reddit.com/r/Superstonk/comments/nwy0oz/math_black_magic_vol_2_the_limit_does_not_exist/)

* This one touches on the price pattern of the short attacks
* **TL;DR => At this point, the number of shares needed to short $GME to zero does not mathematically exist.**

[Math Black Magic, Vol. 3: Trillion Short Share Seance](https://www.reddit.com/r/Superstonk/comments/nya5ps/math_black_magic_vol_3_trillion_short_share_seance/)

* **TL;DR => I try to make estimates of shares shorted based on the known equations and data at that time. I stand by the methods, but they needed more refinement. Which leads to the following volume...**

[Math Black Magic, Final Vol: Epilogue](https://www.reddit.com/r/Superstonk/comments/odrnbv/math_black_magic_final_vol_epilogue/)

* **TL;DR => I made this post as a sort of correction. I went through the model again and tightened it up and got an answer I feel much more confident in**

[Malleus Oeconomica: A Compressed Primer](https://www.reddit.com/r/Superstonk/comments/of1lz2/malleus_oeconomica_a_compressed_primer/)

* In Short & Shorter, I use several economic concepts and equations that need a little explaining first.
* **TL;DR => This is already a compressed post. I can't really put it any simpler than I do in the post.**

[The Chronicles of Short & Shorter, Ep. 1: During the January Sneeze](https://www.reddit.com/r/Superstonk/comments/ogi75b/the_chronicles_of_short_shorter_ep_1_before_the/)

* This is the first step of the process from which I got my revised shares shorted count. I try to dissect their shorting strategy and quantity shorted from 2015 to before the January Sneeze.
* **This post could really use some love as it got downvoted to oblivion by shills.**
* **TL;DR => scroll to bottom of this post**

\-----------------------------------------------------------------------------------------------

# A. Intro

This is still stuck in my head from the last post. Once again very sorry:

([Begin drum loop](https://www.youtube.com/watch?v=JgLcJFad90I))

Absolutely nobody: Hey Nydus, can you tell us a bedtime story?

Ok, heeerrre we go:

Once upon a time not long ago

When people went long and invested slow

When laws were stern and justice stood

And people were investin' like they ought to: good

There was little Gabe who broke his bread

With another Kenny boy and this is what he said:

"Me, you and Steve are gonna make some G's

Shorting inelastic curves and makin' FTDs"

&#x200B;

I DID NOT MAKE THIS! IT WAS ORIGINALLY POSTED BY u/MisterFinishLine.! [https://www.reddit.com/r/Superstonk/comments/nii1s6/short\_shorter/](https://www.reddit.com/r/Superstonk/comments/nii1s6/short_shorter/)

\-----------------------------------------------------------------------------------------------

# B. Timeframe

* (Magenta circles denote time points)
* Time 0 - Squeeze peaked Jan. 27; P(0) = $357.51
* Buy Button turned off Jan. 28
* Time 1 - Feb 1 (3 trading days from time 0); P(1) = $214.51
* Time 2 - Feb 3 (5 trading days from time 0); P(2) = $85.80
* Time 3 - Feb 4 (6 trading days from time 0); P(3) = $51.48
* On approximately Feb. 10 (10 days from time 0) price settled out at \~$45

&#x200B;

[Time Frame](https://preview.redd.it/8pzd9plt4ga71.png?width=1085&format=png&auto=webp&s=86a0ec858c26316fb0add3ca0df57313fab5a6dd)

\-----------------------------------------------------------------------------------------------

# C. Additional Assumptions

The full list of my assumptions can be found in Ep. 1. See links at top of post.

*SHORT ATTACK MAGNITUDE IS ALWAYS MAXIMUM*

In the last post, I mentioned an excerpt from Finnerty's paper, which should sound familiar:

>"...suppose the manipulator realizes at time 2 that the firm’s share price the next period will be *H*, rather than *L* as originally expected, say, due to favorable developments in the firm’s business. Suppose further that the securities regulators or the clearing house require all securities dealers to clear up all fails to deliver. The manipulator would face potentially large losses on his short sales. By short selling an additional *2A/(3B)* shares at time 2, he can drive the share price close to zero." (Pg. 56, par. 3)

The quantity *2A/3B* is double the amount the manipulator usually sells at time 2, which indicates to me that they have to increase the magnitude of their short attacks to compensate for the change to a higher value. I will not be using the quantity strategy described above as its mathematical parameters are different, but the I feel the circumstantial similarity provides reasonable basis to assume that during and after the Sneeze, they were always shorting the maximum amount of shares.

With all this in mind, and the fact that GME is a *H* company, I will no longer calculate/use variable *L*.

*ELASTIC DEMAND CURVE*

This assumptions ONLY applies to during the Sneeze as a result of them turning off the buy button. Using the elastic coefficient resulted in the lowest reasonable estimates as well. This makes sense as they can manipulate an elastic demand curve with less shares.

\-----------------------------------------------------------------------------------------------

# D. Price Pattern

With buy pressure pretty much neutralized. Its hard for me to judge the how much each contributed to price drop. I tried to identify if there were any clear trends. **The first attack dropped price by 40 percent (normally it drops 33 percent), the second by 60 percent (normally it drops 50 percent) and the third by 40 percent (normally takes price close to zero)**. Not too much deviation, in fact, I expected more, but I assume that letting us buy limited amounts of shares on the way down stiffened out demand curve a little to maximize their profit.

\-----------------------------------------------------------------------------------------------

# E. Equations & Variables

FINNERTY FORMULAS

[Quantity Shorted](https://preview.redd.it/xax47cpu4ga71.png?width=919&format=png&auto=webp&s=ae6de0da936ab3191b25da1f014a733d7c288d51)

VARIABLE *B*

[Elasticity](https://preview.redd.it/al41sdvv4ga71.png?width=977&format=png&auto=webp&s=de833e2bca03a4b97528fb651e94fc85e5bfff22)

&#x200B;

[Variable B](https://preview.redd.it/2bx6yj6x4ga71.png?width=851&format=png&auto=webp&s=3525b0733c687395d3d919a577478837c17290e4)

&#x200B;

VARIABLE *A*

&#x200B;

[Variable A](https://preview.redd.it/rhkmakma5ga71.png?width=980&format=png&auto=webp&s=33ece2edace98830a32933bdaae3cd52946f6196)

&#x200B;

VARIABLE *H*

&#x200B;

[Variable H](https://preview.redd.it/du6kmnfc5ga71.png?width=949&format=png&auto=webp&s=02b0223ad8d9f7de69ac1c96c0a53071a753a5bd)

&#x200B;

\-----------------------------------------------------------------------------------------------

# F. Results

(Share counts in millions)

Chart 1: Shares Shorted During Sneeze

|Time (t)|Quantity Shorted|
|:-|:-|
|Time 1|62.642|
|Time 2|62.648|
|Time 3|133.35|

Chart 2: Totals from During Sneeze ONLY

|Total Shorted Shares at Time 2|125.29|
|:-|:-|
|SI at Time 2|177%|
|Total Shorted Shares at Time 3|258.64|
|SI at Time 3|366%|

&#x200B;

Chart 3: Cumulative Counts (Pre-Sneeze + During Sneeze)

&#x200B;

|Shares Shorted from Pre-Sneeze|155.37|
|:-|:-|
|Pre-Sneeze SI|220%|
|Cumulative Shorted Shares at this Point|414.01|
|Cumulative SI at this Point|586%|

&#x200B;

\-----------------------------------------------------------------------------------------------

# G. Conclusions

Notice how that by time 2, when the price halves they had shorted more shares than shares outstanding and by the end of time 3 they have shorted about the same amount of shares they had shorted Pre-Sneeze.

The more I extrapolate I assume my margin of error grows, but I still feel confident in these answers. I believe this is where reached a point that they were no longer able to drop us back down to $40. I feel like my hypotheses don't fully explain why though. Input is appreciated.

\-----------------------------------------------------------------------------------------------

# H. Next Post

We'll look at the time period after the January Sneeze to approximately mid-April 2021

\-----------------------------------------------------------------------------------------------

# I. TL;DR

&#x200B;

[I DID NOT MAKE THIS! ORIGINAL MEME POSTED BY u\/Archisaurus, https:\/\/www.reddit.com\/r\/Superstonk\/comments\/oev08e\/this\_is\_my\_brain\_going\_through\_the\_due\_diligence\/](https://preview.redd.it/lmundof7pga71.png?width=942&format=png&auto=webp&s=0e77d79ba2b5bc4739a4372513080174f9a3efc3)