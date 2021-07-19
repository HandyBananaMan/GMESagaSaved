# Title: Retail is the whale
# Author: 33a
# Post URL: [https://www.reddit.com/r/Superstonk/comments/mwn95o/retail_is_the_whale/](https://www.reddit.com/r/Superstonk/comments/mwn95o/retail_is_the_whale/)


Here's a really simple method to estimate the amount of shares that retail owns in GME, in the [spirit of a Fermi estimate](https://www.lesswrong.com/posts/PsEppdvgRisz5xAHG/fermi-estimates).  Summed with [the 13f/g filings](http://finra-markets.morningstar.com/MarketData/EquityOptions/detail.jsp?query=14%3A0P000002CH&sdkVersion=2.59.0), this gives a lower bound on the total number of shares currently in circulation as well as the short interest.  Therefore, figuring this out would be great to help convince skeptics and shut down shills/FUD.

The general approach I take in this document is to try to estimate the fraction of all shares held by retail from a few different sources.  From this we can then divide the known institutional holdings to get some estimate of how big retail is.

# Retail market share according to FT

[According to the Financial Times](https://archive.is/drLS7), retail market share has been growing significantly in the last 2 years and is now the second largest source of all trading volume after high-frequency trading (HFT).  Based on their chart, I got the following numbers

| | Market Share % |
|--:|:---|
| HFT | 45 |
| Retail | 23 |
| Quants | 13 |
| Hedge funds | 8 |
| Banks | 5 | 
| Mutual Funds | 6 |

[Here's the same data in a pie chart:](https://docs.google.com/spreadsheets/d/e/2PACX-1vSKfRL8EeXpZoCIe3ITFCsuHga-0AEAnPajpc6W8HqHMye7-INtn1MLDv5RShMr3HpIDCNAA34LeZ7I/pubchart?oid=1076768830&format=interactive)

https://imgur.com/a/nkSdlG6

But the market share with HFTs is misleading; while they make a large volume of trades HFTs don't hold their positions very long.  [According to Deustche Bank,](https://web.archive.org/web/20170529002243/http://www.dbresearch.com/PROD/DBR_INTERNET_EN-PROD/PROD0000000000269468.pdf)

> Typically, a high frequency trader would not hold a position open for more than a few seconds. Empirical evidence reveals that the average U.S. stock is held for 22 seconds.

When we exclude HFTs, **retail is the biggest whale in the stock market**

| | Market Share % (Excl HFT) |
|--:|:--|
| Retail | 41.8 |
| Quants | 23.6 |
| Hedge funds | 14.5 |
| Banks | 9.1 |
| Mutual Funds | 10.9 |

[Again, in a pie chart:](https://docs.google.com/spreadsheets/d/e/2PACX-1vSKfRL8EeXpZoCIe3ITFCsuHga-0AEAnPajpc6W8HqHMye7-INtn1MLDv5RShMr3HpIDCNAA34LeZ7I/pubchart?oid=1176366613&format=interactive)

https://imgur.com/a/2MujZuS

This suggests that a typical security has **40% retail ownership on average**.

# Retail market share according to Fidelity

Since I don't have a Bloomberg terminal, we can check the 40% estimate using Fidelity's ownership data.  [Here's AAPL](https://eresearch.fidelity.com/eresearch/evaluate/fundamentals/ownership.jhtml?stockspage=ownership&symbols=AAPL):

https://imgur.com/a/NOgksLG

My assumption is that "Other" is mostly retail implying AAPL has about 38.2% retail ownership. 
 I collated this data for a bunch of other types tickers of tickers below;

## Mainstream stocks

First, I looked at some boring mainstream stocks to get a baseline estimate.  These are generally safe investments that slowly go up-and-to-the-right over time:

| Ticker  | Other % |
|--------:|:--------|
| [AAPL](https://eresearch.fidelity.com/eresearch/evaluate/fundamentals/ownership.jhtml?stockspage=ownership&symbols=AAPL) | 38.2 |
| [WMT](https://eresearch.fidelity.com/eresearch/evaluate/fundamentals/ownership.jhtml?stockspage=ownership&symbols=WMT) | 31.6 |
| [SPY](https://eresearch.fidelity.com/eresearch/evaluate/fundamentals/ownership.jhtml?stockspage=ownership&symbols=SPY) | 36.5 |

To me around 1/3 retail ownership seems consistent with FT's numbers.

## Cult "Meme" stocks

These are companies with solid fundamentals and a great story that have lots of traction on social media and tons of retail buying.  [They hit the top of Fidelity's top orders every day](https://eresearch.fidelity.com/eresearch/gotoBL/fidelityTopOrders.jhtml) and are popular on WSB:

| Ticker  | Other % |
|--------:|:--------|
| [TSLA](https://eresearch.fidelity.com/eresearch/evaluate/fundamentals/ownership.jhtml?stockspage=ownership&symbols=TSLA) | 52.1 |
| [PLTR](https://eresearch.fidelity.com/eresearch/evaluate/fundamentals/ownership.jhtml?stockspage=ownership&symbols=PLTR) | 73.9 |
| [BB](https://eresearch.fidelity.com/eresearch/evaluate/fundamentals/ownership.jhtml?stockspage=ownership&symbols=BB) | 54.7 |


Again we see numbers between 50-75%, which suggests above average levels of retail buy in.

## Pump and dumps

And then there's the pump&dumps.  We've seen lots of these hit WSB rapid fire since the rise of GME in some futile effort to break retail.  You know what they are: weed, silver, ...  All of them pumped to high hell by the Motley Shill and summarily dumped on the poor fools greedy and dumb enough to buy in:


| Ticker  | Other % |
|--------:|:--------|
| [SNDL](https://eresearch.fidelity.com/eresearch/evaluate/fundamentals/ownership.jhtml?stockspage=ownership&symbols=SNDL) | 99.9 |
| [PSLV](https://eresearch.fidelity.com/eresearch/evaluate/fundamentals/ownership.jhtml?stockspage=ownership&symbols=PSLV) | 89.7 |
| [NOK](https://eresearch.fidelity.com/eresearch/evaluate/fundamentals/ownership.jhtml?stockspage=ownership&symbols=SNDL) | 95.7 |

*GUH!* those are some heavy bags.  SNDL doesn't even have a board any more!  At 99% retail ownership, it's just worthless paper with no insiders or institutions or connection to a real company.  Fuck the WSB mods, the Motley Shill and Robinhood for pushing this garbage on people.

## AMC, KOSS and GME

Finally there's the big 3.  I grouped all of these together because they are the same 3 securities [implicated in the Apex Cartel price fixing conspiracy](https://old.reddit.com/r/Superstonk/comments/mq4gfi/sec_filing_merger_with_brokarage_detailing/).  They've all traded more-or-less the same since January, though AMC has recently begun to break out of the pattern:

https://imgur.com/a/q96E6Wr

Isn't it strange that our beloved GME trades exactly the same dip-for-dip, peak-for-peak as [a company that makes mediocre headphones](https://www.koss.com/)?


| Ticker  | Other % |
|--------:|:--------|
| [AMC](https://eresearch.fidelity.com/eresearch/evaluate/fundamentals/ownership.jhtml?stockspage=ownership&symbols=AMC) | 79.2 |
| [KOSS](https://eresearch.fidelity.com/eresearch/evaluate/fundamentals/ownership.jhtml?stockspage=ownership&symbols=KOSS) | 68.3 |
| [**GME**](https://eresearch.fidelity.com/eresearch/evaluate/fundamentals/ownership.jhtml?stockspage=ownership&symbols=GME) | **0.1** |

Given the extreme interest, no surprise AMC is at 79% and KOSS around 68%.  **BUT WHAT THE FUCK IS GOING ON WITH GME**?!  0.1% of GME is only 70000 shares.  **DFV ALONE HAS MORE THAN TWICE THAT MUCH**.  Clearly this number is totally wrong.

# Estimate of the REAL retail ownership

Given the fraction of all shares owned by retail and the size of all institutional holdings we can compute the number of synthetic shares as a % of the total shares outstanding.  Here's a quick table I put together for reference:

https://imgur.com/a/wNMYBHf

According to the [latest Bloomberg terminal drop](https://old.reddit.com/r/Superstonk/comments/mwdqyh/22042021_gme_bloomberg_terminal_information/), institutions have at least 110% of all shares outstanding. So:

* If retail has 40% (like AAPL), then 83% of outstanding shares are short. **58.1 million shorts in total**
* If retail has 50% (like TSLA), then 120% of outstanding shares are short. **84 million shorts in total**
* If retail has 70% (like AMC), then 267% of outstanding shares are short. **186.9 million shorts in total**
* ...and if retail has 80%, then *450% of outstanding shares are short*.  **315 million shorts will need to cover**

Conclusion: **Retail is leviathan**.  And shorts r fuk

----

**EDIT**  Fixed some typos.  For clarification the calculation in that table is purely mathematical.  We have two independent variables:

* I_o = % of *outstanding* shares held by institutions
* R_c = % of *circulating* shares held by retail

Note that circulating and outstanding shares are not the same thing due to shorts or "synthetic longs".  We want to compute the number of these shorts, which is (circulating shares) - (outstanding shares).  I assume retail ownership is linearly proportional to institutional ownership.  We can solve for the size of retail holdings in outstanding shares, R_o, starting from the definition of R_c

R_c = R_o / ( R_o + I_o )

Giving

R_o = R_c * I_o / ( 1 - R_c )

To get the amount of shorts as a % of shares outstanding we can sum R_o and I_o then subtract 100%.