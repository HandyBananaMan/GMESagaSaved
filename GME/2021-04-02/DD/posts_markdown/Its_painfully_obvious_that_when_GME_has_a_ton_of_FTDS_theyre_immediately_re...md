# Author: canhazreddit
# Post URL: [https://www.reddit.com/r/GME/comments/mijfq9/its_painfully_obvious_that_when_gme_has_a_ton_of/](https://www.reddit.com/r/GME/comments/mijfq9/its_painfully_obvious_that_when_gme_has_a_ton_of/)


tl;dr:
Maybe 100 million FTD's that need to be covered


So I scrapped all the data from [https://www.sec.gov/data/foiadocsfailsdatahtm](https://www.sec.gov/data/foiadocsfailsdatahtm) in to a sql database to make it easy to mess with charting in Excel. (I don't do charting/reporting, I'm a software developer, scraping the data was the easy part. I know there's probably much better ways to chart stuff with R Shiny or some shit). 

I used a sql function called 'lag' to add the gain/loss of the ftd quantity over time and charted it.

[https://i.imgur.com/2KYDw1c.png](https://i.imgur.com/2KYDw1c.png)

I know there's a shit ton of lines on this pic, but bear with me. Just look at the pattern. Up then Down in practically identical numbers. Look at the numbers on the left. They go positive/negative pretty regularly. 

Here's zoomed into February to the latest date:

![https://i.imgur.com/1cUJrKQ.png](https://i.imgur.com/1cUJrKQ.png)

Okay, so here's my thought, sum up the gains and the losses, see what comes out.

Total value of FTDs that were reset (loss): (closing cost (at the time) \* qty (66109899)): $1,704,359,023.94. 

Total value of FTDs accumulated (gains): (closing cost (at the time) \* qty (165019925))? $3,315,577,254.39.

So a net loss of ftds (they "covered" or whatever you call it) since the beginning of time: \*66,109,899\*

Net FTD gains: \*165,019,925\*.

Since FTD's in this SEC data is aggregate, and they say themselves you can't know how old they are based on this data, I say that doesn't really matter. They're all reset anyways. 

However, since it's pretty clear when the FTD's go up, they very quickly go back down, it seems reasonable enough to sum and subtract all those ups and downs. So what if we do just that? How many FTD's are left over after subtracting between the qty all the times it went up (165019925) and down (66109899)? 

98,910,026 FTD's. Might be a major flaw in that logic, but it makes sense to my smooth brain. 

Again... 98,910,026 FTD's. At current share price that's $18,936,324,477 (billion)

On the SEC they say the source of the FTD data can suck and vary, so grab that salt and throw it over your shoulder and hit Seabass.

Not financial advice. I barely comprehend this stuff, and my logic could be completely wrong.  I just like the stock.