# Author: Jonathan_McFall
# Post URL: [https://www.reddit.com/r/Superstonk/comments/o1sggl/the_hidden_shorts_the_correlation_of_ftds_and/](https://www.reddit.com/r/Superstonk/comments/o1sggl/the_hidden_shorts_the_correlation_of_ftds_and/)


**My dearest apes,**

&#x200B;

This something that has been weighing on my mind for quite a while. **Where are the short positions?** Well, we all have heard the rumors of **resetting FTDs with the use of the options chain**. Being the ~~wrinkle brain~~ retard that I am \*wink wink\*, I've decided to do a little digging. Most of the solid theories people have about hiding short positions comes from this SEC paper: [https://www.sec.gov/about/offices/ocie/options-trading-risk-alert.pdf](https://www.sec.gov/about/offices/ocie/options-trading-risk-alert.pdf)

&#x200B;

Coincidentally \*wink wink\*, there just so happens to be some really insane stuff going on in the options chain of $GME. And a lot of it started... \*gasp\*... when the price jumped to $483 and the short interest suddenly dropped from \~140% to \~30%. So, what do you say we look a little deeper into the options chain, Kenny?

&#x200B;

&#x200B;

[from: https:\/\/www.barchart.com\/stocks\/quotes\/GME\/put-call-ratios](https://preview.redd.it/bsxz0n0f9s571.png?width=1157&format=png&auto=webp&s=00894296b776243a7257e58a317e226c85700409)

&#x200B;

This is the options data for all of the currently existing $GME options. There are a few things that strike me as odd. The main thing is: what is up with the huge amount of put open interest for the 7/16 expiration date and 1/21 expiration date? Let's take a closer look at the 7/16 options chain specifically.

&#x200B;

&#x200B;

[from: https:\/\/www.barchart.com\/stocks\/quotes\/GME\/options?moneyness=allRows&view=stacked&expiration=2021-07-16-m](https://preview.redd.it/85976zk0as571.png?width=1157&format=png&auto=webp&s=7d7071a130a47b22977aad47d2dd8b6d835c4102)

&#x200B;

**WOAH THERE, KENNY!** You're almost making it too easy. As you can see, an **ENORMOUS** amount of the open interest comes from way, way, way, way, way OTM put options. In case I wasn't clear, these puts are stupidly out of the money at a price point that will never be reached again. Find me another stock that has this sort of bizarre options activity and I'll trade you one $GME share. "Okay, well so what?" you ask. "These options have been purchasable since June of 2020. They could've been bought by bears back then who were still convinced $GME was going to zero." Oh really? Let's take a look at a graph of the open interest, then.

&#x200B;

&#x200B;

[from: ThinkOrSwim platform](https://preview.redd.it/4vmae7syas571.png?width=1546&format=png&auto=webp&s=2cdd8cf91984923c4a2c5000acc7dbf7c60ee1e0)

&#x200B;

As you can clearly see (or maybe not so clearly, it's kind of shit quality), the open interest doesn't enter significant numbers until 1/25. From 1/25 to about 2/3, the open interest spikes from near zero levels to 80,000. This coincides with $GME's initial gamma squeeze. The second spike from 80,000 to 140,000 occurred from 2/23 to 3/23. This coincides with $GME catching it's second breath, the run-up that followed the 2/24 spike, and the eventual fall from near-peak levels.

Ok, so it's obvious someone really needs these worthless put options for something. Now, let's start to do some statistical testing. I'll try to keep this simple for all of you smooth-brains out there.

&#x200B;

So, the working theory for a long time is that SHFs reset their FTDs using tricky options trades outlined in the SEC paper I linked above. It basically involves a bunch of synthetic positions that make the balance sheet look like you've covered your shorts. (NEWS FLASH: THEY HAVEN'T). So, if we are looking at FTDs and the use of these worthless put options (If I haven't emphasized enough how weird it is for these stupidly OTM put options to have this kind of activity, here it is: THIS IS FUCKY SHIT GOING ON HERE THAT IS COMPLETELY ABNORMAL) and FTDs, what can we expect to see? Well, we would expect to see a negative correlation meaning: as the FTDs are hidden away, the open interest in these puts (used to reset these FTDs) should go up. So how do you test for something like this. \*ENTER EXCEL\* (or Google Sheets because I spent all my money on $GME).

&#x200B;

So here was my process. I am going to get FTD data from pre-January-run-up to April 28. I'm then going to get the open interest of this specific put option for the same dates and run a Pearson Correlation Coefficient these two data points to check for a correlation.

&#x200B;

Here is what I am working with:

[from: my brain](https://preview.redd.it/2jl7v64gds571.png?width=1064&format=png&auto=webp&s=f74833a9d05ba9b1c67249cf20d1849fa644eef4)

&#x200B;

You can't really see in the screenshot, but there are a lot more rows of this FTD and open interest data. Now, this **DOESN'T EVEN INCLUDE ETF FTDs AND IS ONLY ONE OF THE OPTIONS CONTRACTS FOR THE ENTIRE CHAIN** and still there **IS A STRONGLY NEGATIVE CORRELATION**, exactly what we hypothesized from earlier.

&#x200B;

**Unfortunately**, I don't have the time to sit down and look at every contract's data, all the ETF FTDs, and the other chains from 01/22/22. But I have glanced at the open interest charts for a lot of them, and they all look EXTREMELY SIMILAR to the contract I showed you today. I suspect if I did sit down and do the grunt work for every single chain and contract, the correlation coefficient would probably increase.

**Fortunately**, though, a -0.67 correlation is considered to be strongly, negatively correlated (anything of +/- 0.5 is considered to be a strong correlation).

**So let's wrap this thing up shall we.**

1. SHFs "reset" their FTDs using nifty options tricks.
2. As FTDs go down, nifty options should go up. (Negative Correlation)
3. After running a Pearson Correlation Coefficient, I have found a STRONGLY, NEGATIVE correlation, exactly what was hypothesized.

&#x200B;

**So questions after reading this DD:**

1. **Should my tits be jacked?**If this doesn't confirm your bias I don't know what will.
2. **What are your qualifications?**I eat crayons for breakfast, lunch, and dinner. Seriously, though, I don't do this for a living. This has just been an interesting side project to confirm my own bias, and I thought I should share the results with all of you.
3. **What mean?**Statistically, it's highly likely the SHFs are using the techniques we've been suspecting them of to reset FTDs.

&#x200B;

So that's it apes. If I've fucked something up majorly, please let me know so I can make the necessary corrections.

**TL;DR**: See question #3

&#x200B;

**Edit 1**: I now realize I should have went more in depth to the SEC paper to explain how they are using options to reset the clock. The idea is that you use a married put trade with a synthetic long rather than buying shares. This would look like: 

buy put + sell put + buy call = married put

Note the put/call ratio of these transactions would be 2. So, as long as the put call ratio for each particular option chain is above 2, it would be valid to say that it is possible that these techniques could be being used. My post aims to prove statistically that these techniques are being used. So with the put/call ratio of the 7/16 options being above 2, I am aiming to correlate the FTDs with the opening of these contracts. 

Here is the section of the SEC paper that talks about the married put trades being used to reset the clock.  [https://imgur.com/a/dWKtvF0](https://imgur.com/a/dWKtvF0). The full paper is linked at the beginning of this post if you are interested in reading. 