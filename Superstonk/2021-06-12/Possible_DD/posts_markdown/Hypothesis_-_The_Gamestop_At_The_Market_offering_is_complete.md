# Author: Roasterson
# Post URL: [https://www.reddit.com/r/Superstonk/comments/ny9l3t/hypothesis_the_gamestop_at_the_market_offering_is/](https://www.reddit.com/r/Superstonk/comments/ny9l3t/hypothesis_the_gamestop_at_the_market_offering_is/)


Hey all, I want to be very clear that all credit for this work goes to u/jebjoya. Posting requirements did not allow him to post this, and I've been working with him in discord to get this out. This past week we've seen some weird movements with gme, and this data focuses on patterns. Specifically, a pattern that seems to show that it's possible that the 5m share offering could be completed as of Friday. None of this is financial advice, and it is meant for open discussion. 

# TL;DR
Through some simple analysis of AMC and GME stocks over the last 60 days, I have attempted to show some “natural” relationship between the two.  With this relationship assumed to be true based on the evidence found, I have shown there to be some level of excess volume for GME in the morning of the 11th June (prior to 12:30pm).  This excess volume equates to a very similar number to the number of shares that GME are releasing to the market through their ATM offering.  As such, I am hypothesising that the sale of the 5m shares in an ATM offering is now complete, and that Gamestop will announce this to be the case in T+2, or AH Tuesday / PM Wednesday of next week.
# Introduction
## About the Author
Hi there, I’m /u/jebjoya and first of all, I have exceptionally limited knowledge of the financial sector outside of the past few months.  I’m in my mid-30s, have a wife and kid, work in technology consulting, and have a Masters degree in Maths from a Russell Group University in the UK (admittedly, only got a 2:2 - was too much of a fan of the pub!).  I can throw together some code, but as you’ll see, I’m assuredly not a developer!
Although I’m something of a lurker on Reddit (which is why I’ve been unable to post this myself), I’m a relative regular in the Discord VC rooms.
## Where this began
So, in the after hours of the market on the 11th June, I was chatting with /u/ClearlyPopcornSucks and /u/Bootheskies and an article came up “How AMC Is Breaking a Meme-Stock Pattern”, which I’m not going to bother linking here (screw their ad revenue for writing that crap) but it got me thinking about what “pattern” might be shared between GME and AMC.
# The Impetus
So, we can start with doing a simple visual comparison of GME and AMC - at the time, I did this with the small Yahoo Finance graphs, but let’s go up a notch and code it out (since we’ll be using some of this same code later).
First of all, you can play along at home if you like - I’m using Python 3.9 (although any 3.x version will probably work), and have pip installed yfinance, plotly, pandas and scipy - that’ll probably do you.  The code for this first graph can be found here: [ATMOffering01-AMCvsGME.py](https://github.com/jebjoya/jebstonks/blob/main/ATMOffering01-AMCvsGME.py)
(NB: Please feel free to do whatever you like with code from the jebstonks repository, it’s up there with the unlicense on it - have fun, go wild.)
[Imgur](https://imgur.com/AXmRPxn)
Just from a rudimentary eye over this, we can see some fairly similar price action between GME and AMC from something like 12:00-13:00 until the end of the day, but the mornings look quite different - GME is moving downwards and AMC is trading pretty sideways.
This is all very well and good doing this by eye, but let’s take it up it a notch and code it out.  We’ll be using the [Pearson Correlation Coefficient](https://en.wikipedia.org/wiki/Pearson_correlation_coefficient) for this, which should give us a guideline as to how related these two stocks are in their movement.  I’m also going to split the day in two - the “morning” or “am” is prior to 12:30pm, and the “afternoon” or “pm” is after 12:30pm.
Our code is here: [ATMOffering02-Correlation.py](https://github.com/jebjoya/jebstonks/blob/main/ATMOffering02-Correlation.py) and we get a result of:
`Morning Pearson: -0.18081255928248074`  
`Afternoon Pearson: 0.8771973125353307`
This shows a clear difference in morning and afternoon - the afternoon being much more closely correlated (positively) and the morning being pretty disconnected.
# A brief diversion into a hypothesis or two
## AMC and GME Diverge only when there is big news
It was at this point that a hypothesis came to me - that the natural state of being of AMC and GME is to broadly track one another (for whatever reason), and any time that this tracking does not happen suggests some change in activity on one side or other (whether that be a squeeze, SHF fuckery or interesting company news, for instance).
So, let’s turn this into something - I hypothesise that the days that AMC and GME track each other the *least* (per a Pearson that is closest to 0) will be days where something major has happened for one or other stock.  So, to start with, let’s find the 5 most and 5 least tracking days since the 14th April (Yahoo Finance’s API only provides 5m candle data for the last 60 days, and this is the earliest data possible at time of coding).  Code, as usual is available from [ATMOffering03-MostTrackingDays.py](https://github.com/jebjoya/jebstonks/blob/main/ATMOffering03-MostTrackingDays.py)
`Least Correlated:`  
`Date   Pearson`  
`28  2021-05-24  0.087472`  
`36  2021-06-09  0.108484`  
`11  2021-04-29  0.169620`  
`23  2021-05-17  0.174076`  
`16  2021-05-06  0.198065`
`Most Correlated:`  
`Date   Pearson`  
`22  2021-05-14  0.905453`  
`31  2021-05-28  0.919137`  
`13  2021-05-03  0.919917`  
`29  2021-05-25  0.925267`  
`33  2021-06-02  0.930533`
So our hypothesis says that the least correlated days should be ones with major events of some description.  Let’s use [gmetimeline.com](https://gmetimeline.com/) and take a look - 24th May was RC’s erection tweet and Lucy Komisar’s AMA, 9th June was 6/9, go figure, 29th April was RC’s Mr Hankey tweet and the AMA with Dr T, 17th May was RC’s tweet of his Grandma and Melvin’s 13F with no $GME holdings, and 6th May was the day after both dlauer’s AMA and the “disappearing” volume on the lowest volume day of 2021 at the time, along with it being the 3rd hearing of the House Committee on Gamestop.
What do we see here?  Well, I’m going to admit - this one is a bit shaky - I’m going to go with this being unproven for now.  I like the fact that 6/9 was in the least correlated days, and we’re seeing a lot of RC tweets on low-correlation days.  On the other hand, 6/2 was the day after DFV came back to Twitter, which perhaps feels like a “big” day for GME.  I don’t feel like we have *enough* at this point to prove the link, but I leave this hypothesis in here for discussion and potential extension (I’ve only been looking at GME news, and not AMC news - should we look at direction, etc etc)
## Minor Aside
I have more recently run this again using a variant of the code above that does *not* include the absolute value of the Pearson Coefficient - this means that we’re looking at the *most negative* correlation (that they’re not tracking).  Most correlated remain the same, but least correlated change to:
`Least Correlated:`  
`Date   Pearson`  
`10  2021-04-28 -0.640546`  
`5   2021-04-21 -0.473214`  
`27  2021-05-21 -0.439651`  
`17  2021-05-07 -0.351925`  
`3   2021-04-19 -0.225512`
These dates don’t exactly scream bigger news days to me than the previous set, but I add this purely to aid discussion.
[ATMOffering03-MostTrackingDays-NONABS.py](https://github.com/jebjoya/jebstonks/blob/main/ATMOffering03-MostTrackingDays-NONABS.py)
## Correlation in Price Action drives Correlation in Volume Spread across the Day
The second hypothesis, and arguably the most important one, is that I believe that the most correlated days will have correlated volume across the day as well.  In particular, I’m going to be looking at pre-12:30 vs post-12:30 volume for each of the 5 most correlated days to see whether they look similar.  Code is here [ATMOffering04-VolumeCorrelationTest.py](https://github.com/jebjoya/jebstonks/blob/main/ATMOffering04-VolumeCorrelationTest.py) and output is:
`Date: 2021-05-14 GME: 0.6969832013569681 AMC: 0.7186096861005629`  
`Date: 2021-05-28 GME: 0.701353007190714 AMC: 0.717350901193812`  
`Date: 2021-05-03 GME: 0.6604088618964389 AMC: 0.6767881287420806`  
`Date: 2021-05-25 GME: 0.3190856955418446 AMC: 0.4060525168801743`  
`Date: 2021-06-02 GME: 0.5112048987969748 AMC: 0.5640133520495791`
The numbers here are showing the ratio of volume that happens before 12:30 to the whole day.  As we can see, when the two stocks are highly correlated (which I hypothesise to be the “natural state” of them, but was unable to fully demonstrate above), the volume pre- and post-12:30 broadly correlate as well.
# Back to Friday
So, I’ve shown to a limited extent that volume appears to track where the stock price tracks, and I am *suggesting* (but, again, have not been able to fully demonstrate) that this is the natural state of GME and AMC.
So, what do I suggest we do with that information?  Well, let’s go back to Friday’s data.  We can see that the afternoon has a high level of correlation (0.87, almost on a par with the 0.90 of the 5th most correlated day), and the morning a crap correlation (0.18 - worse than the 0.19 on the 5th least correlated day).  I’ve also suggested that when correlated, the stock has similar volume.  What I am suggesting is that the lack of correlation on Friday morning was caused by excess shares being loaded into the market, causing a deviation from the AMC baseline and downward trend.
How do we work out what the excess is?  Easy really - check the percentage of AMC volume that happened in the morning vs afternoon, assume the afternoons should broadly match, and work out what the morning *should* have been for GME if tracking.
Code is here [ATMOffering05-ExcessVolumeCalculation.py](https://github.com/jebjoya/jebstonks/blob/main/ATMOffering05-ExcessVolumeCalculation.py)
And the results:
`AMC Ratio: 0.37143463487609085`  
`GME PM Volume: 5574831`  
`AMC Implied Total Volume for GME: 8869134.873349302`  
`Excess Volume for GME: 6420225.1266506985`
We can see an implied excess volume in the morning for GME of 6.42 million shares.  Obviously higher volatility breeds higher volume due to HFTs, but this 6.42m is surprisingly close to the 5m share ATM offering that Gamestop announced earlier this week.