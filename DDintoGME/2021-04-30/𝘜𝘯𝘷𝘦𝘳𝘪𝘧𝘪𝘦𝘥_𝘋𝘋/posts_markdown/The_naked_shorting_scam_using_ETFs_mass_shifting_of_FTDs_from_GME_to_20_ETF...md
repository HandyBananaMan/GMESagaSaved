# Author: broccaaa
# Post URL: [https://www.reddit.com/r/DDintoGME/comments/n1x75w/the_naked_shorting_scam_using_etfs_mass_shifting/](https://www.reddit.com/r/DDintoGME/comments/n1x75w/the_naked_shorting_scam_using_etfs_mass_shifting/)


[.](https://preview.redd.it/yeq3jm7tqbw61.png?width=4500&format=png&auto=webp&s=d28e4cac7cdb395aa6e758d4b79dafe9847dfc20)

In my recent post [The naked shorting scam in numbers](https://www.reddit.com/r/Superstonk/comments/mvdgf5/the_naked_shorting_scam_in_numbers_ai_detection/) I looked at options activity that could be used for mass naked short selling (Deep ITM calls and married put trades) and weird OTC trade data for GME in 2021. Since then I've taken another look at the ETF data to help complete the picture.

**TLDR**: Short positions were shifted from GME to related ETFs after the Jan mini-squeeze. XRT and IWM were the ETFs of choice in Feb, in march dozens of ETFs have been used. As reported SI decreased in GME the ETF IWM had simultaneous increases in reported SI. Total value of reported SI (GME + ETFs) remains as high as ever at 27+ billion dollars owed. Hiding FTDs and SI in ETFs must be massive ball ache and does nothing to solve the short problem.

*Note: this is not financial advice. I am not a cat. I gathered some data, made some figures and tried to understand them. Any number of my interpretations could be flawed and wrong. Do your own research, make your own mind up.*

# Introduction

Back in Feb the apes felt cheated. Robinhood and other brokers blocked retail buy orders at the end of Jan 2021 and GME price crashed back down. The media claimed GME was over. Other subs and paper hands laughed at the 'bag holders' and I can't have been the only one to think maybe I was crazy to be hanging on. That was until the DD started to flow and we found shorts shifting their positions to ETFs.

DD apes like u/ahh_soy started to find [massive short interest in GME containing ETFs](https://www.reddit.com/r/GME/comments/ljwo3v/serious_researchers_needed_now_i_think_i_know/). XRT was a main EFT of interest back in Feb. Here is a [Baron's article describing how ETFs can be used to short specific stocks](https://www.barrons.com/articles/synthetic-shorting-with-etfs-1488206009) and another [academic paper for further reading if interested](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2836518).

With all the great DD work since then we now know that GME short positions are almost certainly being hidden in ETFs and using different types of options fuckery. I left out analysis of ETFs in the past because it can get complicated but a [recent post](https://www.reddit.com/r/Superstonk/comments/mvvmvp/time_to_expose_the_shell_game_ftds_can_be_reset/) by u/augrr inspired me to take another look.

# ETF Fail to Delivers

I selected GME and 19 ETFs containing GME. I chose to only look at the ETFs that contain the most GME shares and had large numbers of FTDs in 2021.

&#x200B;

[Total FTDs for GME and selected ETFs in 2021 with GME close price overlaid.](https://preview.redd.it/g392vdc74cw61.png?width=4500&format=png&auto=webp&s=3063cb1822e05c741c4a39fbf408444ba501e396)

Notice in this plot that GME made up most of the total fails throughout Jan 2021. As price spiked during the Jan mini-squeeze GME FTDs decreased but FTDs in all ETFs spiked.

Interestingly XRT and IWM had the most fails throughout Feb. After the apes learnt about XRT and IWM fails at the end of Feb FTD fails started to be spread across a multitude of other ETFs. If managing FTDs in GME was a pain in Jan imagine the poor fuckers who now need to keep a lid on FTDs across 20+ GME containing ETFs.

&#x200B;

[Total Value of FTD fails for GME and selected ETFs in 2021 with GME close price overlaid.](https://preview.redd.it/4jihm7t84cw61.png?width=4500&format=png&auto=webp&s=95a9d8b592cabf005fbe0d693e33224e06bfcc60)

This plot is similar to the previous one but now looks at the total value of FTD fails in dollars. Here we see that even though GME FTDs were very low in March the total value of ETF fails was comparable with the total fails seen in early Jan.

Could the massive spike in IWM fails at the end of Feb be what led to the price run up in early March??

&#x200B;

[Total FTDs for GME and selected ETFs since Jan 2020 with GME close price overlaid.](https://preview.redd.it/uni2sz4b4cw61.png?width=4500&format=png&auto=webp&s=ea4081e6bb153db5ec35e6fb67ed85511245c0c1)

Here we see the GME and ETF FTDs since Jan 2020. Because there has been such an exponential change in GME share price over the last year I'm using a log scale here.

&#x200B;

[Total FTDs for GME since Jan 2020 with GME close price overlaid.](https://preview.redd.it/c4kt5yad4cw61.png?width=4500&format=png&auto=webp&s=3a230e156f5d601070f88188608d7ad81bf489b0)

This plot is the same as before but just focuses on GME to make some of the observations clearer.

A few things of note:

1. GME FTDs (light blue) emerge in 'clumps' with many fails over successive days
2. The time between GME FTD clumps can range from a few weeks to even a few months before exploding again (relatively few fails between May and Sept 2020)
3. Of the ETFs IWM has the most fails, occasionally reaching 8 million+ shares failed to deliver
4. IWM FTD spikes appear to follow spikes in GME FTDs. The exception being huge IWM FTD clumps in June 2020 despite there being not so many GME FTDs.
5. Fails across all GME containing ETFs have been consistently large throughout March even if GME FTDs were reported to be low.

# ETF Reported Short Interest (SI)

W can also look at reported short interest for the GME containing ETFs. The shorts are completely fucked if they let the true short position in GME be know. This is why they've gone to such lengths to make the GME short position appear so low. However they're unlikely to be able to manipulate the reported SI across all the GME containing ETFs as well.

These plots take a look at reported SI for GME and the selected GME containing ETFs.

&#x200B;

[Reported SI as number of shares sold short for GME and selected ETFs.](https://preview.redd.it/dgld9ngf4cw61.png?width=4500&format=png&auto=webp&s=6e061ca3f8014692653e35059e5dff9d8251eca8)

The total number of shares reported to be sold short for GME and ETFs remained fairly consistent throughout 2020. At the end of Jan 2021 GME SI was reported to drop significantly but at the exact same time we see an increase in the number of IWM shares sold short.

&#x200B;

[Total value of reported SI for GME and selected ETFs.](https://preview.redd.it/ntm48ohh4cw61.png?width=4500&format=png&auto=webp&s=9f1e2518e23657f2cea955bc9a2a10a1dfe67de1)

With the shift of SI in GME to IWM the actual value of reported SI has not decreased in any meaningful way. Approx 27 billion dollars worth of shares are reported to be sold short for GME and the selected ETFs.

# Bonus: Exponential price increases since RC declared his GME position on Aug 18th 2020

[Exponential price increases in GME since Ryan Cohen revealed his GME position.](https://preview.redd.it/j4ktocel4cw61.png?width=3343&format=png&auto=webp&s=618d42bbfa4b9114a63787cf7185dbba0bfb06ee)

This plot isn't related to ETFs but I thought it was interesting enough to include.

In the first half of 2020 GME share price remained pretty flat, even slowly decreasing in value. On Aug 18th 2020 Ryan Cohen revealed his GME share purchase. Since then GME share price has increased exponentially. Even with current prices and sideways trading we remain on this exponential trajectory. If this were to continue then prices would naturally reach the realm of a margin call.

# ETFs with GME in April 2021

[ETFs containing GME. Total dollar value of GME and &#37; allocated to GME.](https://preview.redd.it/jesl8blo4cw61.png?width=5400&format=png&auto=webp&s=53b5121963aa38703a1cffed055df395fd77ac32)

Not much to say about this plot but it contains info on all GME containing ETFs as of April 2021. Could be useful for other people to use when starting a DD.

# Conclusion

This data appears to show a shift of short positions from GME to related ETFs after the Jan mini-squeeze. XRT and IWM were used the most in Feb before the apes caught on. Did the shorts then switch to 20+ other ETFs to hide their fuckery again? This is definitely possible as the ETF FTDs seen in March were much larger than typical values in 2020.

As well as FTDs being shifted we see evidence of SI being shifted from GME to ETFs. The main ETF used here appears to be IWM. Total remains as high as ever at 27+ billion dollars owed.

The short fuckery being done with ETFs as well as [what we've seen using options trades](https://www.reddit.com/r/Superstonk/comments/mvdgf5/the_naked_shorting_scam_in_numbers_ai_detection/) paints a clear picture of manipulation on the short side. All of these efforts reek of desperation from the shorts as their only hope of escape is making apes scared or bored. But I ain't going anywhere. ***I like the stonk***.

🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀