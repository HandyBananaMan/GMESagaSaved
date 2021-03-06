# Title: GME's Average Net FTD $ Amount is 30.5x higher than all FTD $ Amounts across all tickers in 2021
# Author: TheStickyToaster
# Post URL: [https://www.reddit.com/r/GMEJungle/comments/oq8zpo/gmes_average_net_ftd_amount_is_305x_higher_than/](https://www.reddit.com/r/GMEJungle/comments/oq8zpo/gmes_average_net_ftd_amount_is_305x_higher_than/)


I'm a crayola junkie. My drink of choice is pink bubblegum amoxicillin out of a turkey baster.

I (somehow) write code professionally, got baked the other night and decided to monkey around with some numbers. If anybody actually reads this, and wants to see the source code, I'll gladly clean it up and post it on GitHub. Or wants me look at the data through a different lens, I'd be glad to do that too.  Otherwise, this is my first attempt at a DD so I'll find out if I'm destined to just continue being a recluse lurktard.

I compiled the FTD data from [https://www.sec.gov/data/foiadocsfailsdatahtm](https://www.sec.gov/data/foiadocsfailsdatahtm) for the entire year of 2021, *so far*. Combining each file and then viewing the results was quite lackluster; because IMO the quantity of fails doesn't really matter when you don't know the float. Failing 1M shares on a 10B float is a lot different than failing 100K on 500K float.

So I writ some code to scrape the web and attempt to obtain the float for every ticker that had appeared in my compilation of the FTDs. That shit ran all night while I dreamt of being Assistant Trailer Park Supervisor at Sunnyvale.

Once that was done, I joined the FTD data with the Float data by ticker.

At the start, I was really just attempting to gain some inside into the T + N theories regarding FTD's, but this snippet on the same link I posted above squashed that idea:

>Fails to deliver on a given day are a **cumulative number of all fails outstanding until that day**, plus new fails that occur that day, less fails that settle that day. The figure is not a daily amount of fails, but a combined figure that includes both new fails on the reporting day as well as existing fails. In other words, **these numbers reflect aggregate fails as of a specific point in time**, and may have little or no relationship to yesterday's aggregate fails. Thus, it is important to note that the age of fails cannot be determined by looking at these numbers. In addition, **the underlying source(s) of the fails-to-deliver shares is not necessarily the same as the underlying source(s) of the fails-to-deliver shares reported the day prior or the day after**.

I'm sure this has been posted before, but I think it's important to understand.

So to my ape brain I concluded the following:

1. FTD's are cumulative
2. There's no way to know if tomorrows fails are the same as todays
3. If day 69 FTDs are 420,000 and day 70 has 1000, AT LEAST (420,000 - 1000) = 419,000 FTD's were satisfied SOMEHOW. (This is where I want to head next, finding a correlation between FTD satisfaction/option volume but I can't find publicly available option data)
4. Due to above points, I disqualified any T + N theory because the disgraceful SEC publishes data in a way that makes it impossible to distinguish FTDs.

So the only data I was able to gather was a little bit of confirmation bias juice.

From January through June, there were 10,987 unique tickers that had FTDs. This dataset included 124 trading days. GME appeared **122 out of those 124 dates**.

The average Percentage of Float (Quantity of Fails / Float) across every instance was 0.0009883%.

GME's average Percentage of Float is 0.003461%, making GME's average **3.87x** normal. Ok, cool. whatever.

Note: the data uses the Float from Yahoo as of 7/22/2021 - we know GME has done share offerings. If anything, this builds a stronger case for the above result, as we are dividing by a larger float, giving a smaller number here.

But, more interestingly..

The average Net Amount (Quantity of Fails \* Share price that day) was $522,891.38.

GME's average Net Amount is **$15,970,901.33, making GME's Net FTD position 29.62x higher than average.**

So on a given day where GME has FTD's (98% of trading days this year), some brain dead SHF's are failing to deliver a position worth nearly $16 million, on average.

No jail, no sale.

&#x200B;

Edit: 

\- Tickers with respective float data (list includes all tickers that were both listed in SEC FTD data & had a float value on Yahoo... could be used for many other analyses): [https://pastebin.com/2JYaGQmU](https://pastebin.com/2JYaGQmU)

\- Aggregate data: [https://thoughtcrime.s3.amazonaws.com/aggregate\_ftds.csv](https://thoughtcrime.s3.amazonaws.com/aggregate_ftds.csv)

\- Script (download data alongside as 'aggregate\_ftds.csv', must have python3.7>): [https://pastebin.com/nvwp58NA](https://pastebin.com/nvwp58NA)

\- Changed 3.5x to 3.87x after slight adjustment. Changed 30.5x to 29.62x.

&#x200B;

&#x200B;