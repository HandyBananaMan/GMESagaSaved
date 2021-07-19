# Title: UPDATE ON: "The Hidden Shorts: The Correlation of FTDs and Open Interest for EXTREMELY OTM Put Options"
# Author: Jonathan_McFall
# Post URL: [https://www.reddit.com/r/Superstonk/comments/o28bbd/update_on_the_hidden_shorts_the_correlation_of/](https://www.reddit.com/r/Superstonk/comments/o28bbd/update_on_the_hidden_shorts_the_correlation_of/)


Hey guys,

I posted this DD earlier this morning: [https://www.reddit.com/r/Superstonk/comments/o1sggl/the\_hidden\_shorts\_the\_correlation\_of\_ftds\_and/](https://www.reddit.com/r/Superstonk/comments/o1sggl/the_hidden_shorts_the_correlation_of_ftds_and/)

If you haven't read that, read it and then come back.

Many of you asked for more strike prices and to also explore the 1/21/22 options chain as it is seeing similar activity. Originally, I didn't think I'd have time to go through and manually pull and correct the data from their respective sources. However, I made a python script to get this information a lot more quickly.

I have run some correlation tests on the wider sets of data, and it looks promising. I have found that the correlation in open interest for these OTM puts are really strong (like **0.997 correlation coefficient strong**). However, the FTD correlation actually decreased. The correlation is still negative, its just less strong. I can think of a few reasons that this could be happening, but the one I suspect the most is:

* The techniques used to reset FTDs **weren't used until the share price reached a point that was actually uncomfortable for SHFs**.

However, I think with a **0.997 correlation coefficient** between the open interests of various OTM put positions proves beyond reasonable doubt that these were purchased and/or sold by one entity or were purchased and/or sold by colluding entities/algorithms.

Clearly something **fucky** is going on here, so that's where I'm going to ask for help from you apes. I am going to make my datasets public. It contains all of the FTDs of $GME from Sep. 6, 2019 to May 28, 2021. It also contains the OI data for strikes in the 7/16 and 1/21/22 chains that have a high OI (>10,000). Hopefully this easy-to-access data will inspire the wrinkle-brains of this sub to search for correlations. Personally, here are a few things I'd like to know that I just don't have the wits to analyze on my own:

1. **If the correlation between OI and FTDs is stronger in the time period that ranges from the January to run-up to present day than the time period that ranges from 2019 to present day, is it safe to say that SHFs haven't used options techniques to "reset" FTDs until recently?**
2. **Is it completely safe to say that these contracts are definitively purchased/sold by one entity/algorithm?**

If you apes can think of any other questions, that would be great. I am going to start researching my own questions right now, so let me know. Here is the data set used:

[https://docs.google.com/spreadsheets/d/1FslEBxiy4Tkfc5ZAzA8o937R4oPPt6EOIwr0xVZO80o/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1FslEBxiy4Tkfc5ZAzA8o937R4oPPt6EOIwr0xVZO80o/edit?usp=sharing).

It contains very valuable information and I'd absolutely love for other apes to take a look at it and see what they come up with.

That's all for now.

&#x200B;

**TL;DR: Negative correlation between FTDs and OTM put open interest is less when looking as far back as 2019, but its stronger when looking at 1/15 or later. Could be because SHFs haven't used FTD "reset" techniques until recently due to the price being low enough in 2019/2020. Now that the price is higher, the high negative correlation suggests they could be using the very tricks they've been suspected of to "reset" FTDs with options contracts.**

&#x200B;

Edit 1: QA/QC of the Data: Description of the methods used to obtain data and full list of sources found below. Was originally a reply to u/Training_Molasses_51 comment, but auto-mod removed because it was too long. 

&#x200B;

 

It is accurate and slightly altered in that some days have 0 FTDs. Those dates aren't listen the files. I had to manually go into all 41 files, check if the days that are missing were 0 FTD days, holidays, or weekends. I did that by cross-referencing the dates of the publicly available and verifiable put option open interest data for various strike prices (ie. some options were available for purchase/sale earlier than others, so you have to look at various strikes to put the puzzle pieces together). That was most of the hard work.

The second nightmare is that the data from the SEC is in such horrible format. The FTD data is stored in bi-monthly CSV files. And it's not just the data for $GME, its the data for literally every stock on the NYSE that had FTDs. So there was 41 14,000+ line files with $GME FTD data hidden throughout. So, I created a python script to search for $GME within each file, get the necessary data (date, volume of FTDs, notional value). Once I had all the data in a spreadsheet, I did the calendar checking process that I described above. You're more than welcome to cross-reference my spreadsheet data with the actual files released from the SEC.

I got the put open interest data straight from [Barchart.com](https://barchart.com/), but I made sure to double check it with my broker, TD Ameritrade. All of their numbers lined up, you can also cross-reference this with another source if you'd like to.

Also it would be extremely hard to enter incorrect data for two completely different options strikes with different expiries and get such a high Pearson Correlation Coefficient, so I trust that I made no mistakes in "doing the grunt work."

Here are my sources if you'd like to check for yourself:

[https://www.sec.gov/data/foiadocsfailsdatahtm](https://www.sec.gov/data/foiadocsfailsdatahtm)

[https://www.barchart.com/stocks/quotes/GME%7C20210716%7C0.50P/interactive-chart](https://www.barchart.com/stocks/quotes/GME%7C20210716%7C0.50P/interactive-chart)

[https://www.barchart.com/stocks/quotes/GME%7C20210716%7C1.00P/interactive-chart](https://www.barchart.com/stocks/quotes/GME%7C20210716%7C1.00P/interactive-chart)

[https://www.barchart.com/stocks/quotes/GME%7C20210716%7C5.00P/interactive-chart](https://www.barchart.com/stocks/quotes/GME%7C20210716%7C5.00P/interactive-chart)

[https://www.barchart.com/stocks/quotes/GME%7C20210716%7C20.00P/interactive-chart](https://www.barchart.com/stocks/quotes/GME%7C20210716%7C20.00P/interactive-chart)

[https://www.barchart.com/stocks/quotes/GME%7C20210716%7C50.00P/interactive-chart](https://www.barchart.com/stocks/quotes/GME%7C20210716%7C50.00P/interactive-chart)

[https://www.barchart.com/stocks/quotes/GME%7C20210716%7C30.00P/interactive-chart](https://www.barchart.com/stocks/quotes/GME%7C20210716%7C30.00P/interactive-chart)

[https://www.barchart.com/stocks/quotes/GME%7C20210716%7C10.00P/interactive-chart](https://www.barchart.com/stocks/quotes/GME%7C20210716%7C10.00P/interactive-chart)

[https://www.barchart.com/stocks/quotes/GME%7C20210716%7C12.00P/interactive-chart](https://www.barchart.com/stocks/quotes/GME%7C20210716%7C12.00P/interactive-chart)

[https://www.barchart.com/stocks/quotes/GME%7C20210716%7C15.00P/interactive-chart](https://www.barchart.com/stocks/quotes/GME%7C20210716%7C15.00P/interactive-chart)

[https://www.barchart.com/stocks/quotes/GME%7C20220121%7C0.50P/interactive-chart](https://www.barchart.com/stocks/quotes/GME%7C20220121%7C0.50P/interactive-chart)

[https://www.barchart.com/stocks/quotes/GME%7C20220121%7C1.00P/interactive-chart](https://www.barchart.com/stocks/quotes/GME%7C20220121%7C1.00P/interactive-chart)

[https://www.barchart.com/stocks/quotes/GME%7C20220121%7C2.00P/interactive-chart](https://www.barchart.com/stocks/quotes/GME%7C20220121%7C2.00P/interactive-chart)

[https://www.barchart.com/stocks/quotes/GME%7C20220121%7C5.00P/interactive-chart](https://www.barchart.com/stocks/quotes/GME%7C20220121%7C5.00P/interactive-chart)

Edit: Forgot to mention that I got the price data from Yahoo Historical Data linked here: [https://finance.yahoo.com/quote/GME/history?period1=1568592000&period2=1622160000&interval=1d&filter=history&frequency=1d&includeAdjustedClose=true](https://finance.yahoo.com/quote/GME/history?period1=1568592000&period2=1622160000&interval=1d&filter=history&frequency=1d&includeAdjustedClose=true)