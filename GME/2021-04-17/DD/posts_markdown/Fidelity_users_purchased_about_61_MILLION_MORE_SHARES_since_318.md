#Title: Fidelity users purchased about 6.1 MILLION MORE SHARES since 3/18
#Author: 33a
#Post URL: [https://www.reddit.com/r/GME/comments/msyhlq/fidelity_users_purchased_about_61_million_more/](https://www.reddit.com/r/GME/comments/msyhlq/fidelity_users_purchased_about_61_million_more/)


The [Fidelity customer orders](https://eresearch.fidelity.com/eresearch/gotoBL/fidelityTopOrders.jhtml) suggest retail is buying GME *hard*.  But it's an incomplete picture because:

1. It only gives the data for the last trading day.  We need historical data to find trends.
2. It only gives the number of orders.  We need order sizes to compute volume.

My brother and I set out to find the missing data and compute how many shares of GME are in Fidelity's retail accounts.  Here's what we've figured out:

## Mining historical data

Starting 3/18 we scraped Fidelity every day:

https://imgur.com/a/Zi0Xoo4

Which we then painstakingly transcribed into a table:

| Date | Buy Orders | Sell Orders |
|:-----|-----------:|------------:|
| 03/18/2021 | 14449 | 5350 |
| 03/19/2021 | 22209 | 9984 |
| 03/22/2021 | 15082 | 11976 |
| 03/23/2021 | 14518 | 4998 |
| 03/24/2021 | 32371 | 11628 |
| 03/25/2021 | 21425 | 12581 |
| 03/28/2021 | 18302 | 13861 |
| 03/29/2021 | 8441 | 4621 |
| 03/30/2021 | 8315 | 6791 |
| 03/31/2021 | 6079 | 3724 |
| 04/01/2021 | 7216 | 3579 |
| 04/05/2021 | 15251 | 4545 |
| 04/06/2021 | 4727 | 2568 |
| 04/07/2021 | 7247 | 2396 |
| 04/08/2021 | 12715 | 3144 |
| 04/09/2021 | 15034 | 3639 |
| 04/12/2021 | 15704 | 3593 |
| 04/13/2021 | 10039 | 2664 |
| 04/14/2021 | 12202 | 5466 |
| 04/15/2021 | 8127 | 2192 |
| 04/16/2021 | 7246 | 1992 |

[Since 3/18, every day there are more buy orders than sells](https://docs.google.com/spreadsheets/d/e/2PACX-1vRjpGn7c6iozFnAs_nQFQUYNxTbS-Etkha5GUCVa5Br0y2Kv-sZ_tBKtc_tPhDYbPbps92jC3tSXLqH/pubchart?oid=124323433&format=interactive).

https://imgur.com/a/FfspgvW

You can check our work using the [wayback machine](https://web.archive.org/web/*/https://eresearch.fidelity.com/eresearch/gotoBL/fidelityTopOrders.jhtml) or [archive.is](https://archive.is/eresearch.fidelity.com).

## Estimated order sizes

Neither of us have direct access to level 2 historical order flow data, so we improvised by scraping ["Stocks Big Plays"](https://www.youtube.com/channel/UCdwwRjEyseTOUYxUWZn2Uqw)'s YouTube channel.
We were able to find archived streams for all of the days in our data set except March 23 and March 28.
We then transcribed the top bid and ask orders at 9:30, 10:30, 12:00, 13:30 and 15:55, giving 5 data points per day. 
[The distribution of order sizes looks roughly Pareto (not surprising)](https://docs.google.com/spreadsheets/d/e/2PACX-1vRjpGn7c6iozFnAs_nQFQUYNxTbS-Etkha5GUCVa5Br0y2Kv-sZ_tBKtc_tPhDYbPbps92jC3tSXLqH/pubchart?oid=442492841&format=interactive):

https://imgur.com/a/pSZt6YW

This gives us something to work with, but there are some issues:

1.  *Noise*:  We can try to compensate for this with more samples and also biasing our estimates to be more conservative.
2.  *Algo trades*: We observed weirdly regular blocks of bid/asks would sometimes flood the books on both sides (eg. 33, 33, 33...).  Fortunately these seem to be wash sales and so their net effect on purchased shares should be close to 0.
3.  *Whales*: Some buy orders are waaaay too larget and not likely retail.  These are usually in blocks of of 500 or more shares.  We exclude outliers by discarding order sizes greater than 1 std deviation above the mean.

With these adjustments we get the following stats

|    | Average | Std. Dev. | Average (Excl. Outliers) |
|:--:|--------:|----------:|-------------------------:|
| **Bid** | 112.46 | 270.71 | 51 |
| **Ask** | 109.54 | 232.66 | 65.66 |

## Putting it together

We propose the following simple formula to estimate the shares purchased each day:

```
Net shares = (Avg. buy) * (# Buy orders) - (Avg. sell) * (# Sell orders)
```

Based on the above analysis, we can plausibly assume the average buy is 51 shares and the average sell is 66.
[Plugging in the numbers from Fidelity, we get the following cumulative share purchases:](https://docs.google.com/spreadsheets/d/e/2PACX-1vRjpGn7c6iozFnAs_nQFQUYNxTbS-Etkha5GUCVa5Br0y2Kv-sZ_tBKtc_tPhDYbPbps92jC3tSXLqH/pubchart?oid=1738592533&format=interactive)

https://imgur.com/a/eX8ZleU

Or in other words, **FIDELITY CUSTOMERS PURCHASED 6.1 MILLION SHARES OF GME SINCE 3/18**

If we include whales as retail, the number goes up to 17 million.
Since Fidelity represents at most 15% of all retail buyers, *I extrapolate that more than 40 million shares were purchased last month alone*.

------

**EDIT** To account for these numbers maybe being too high, I used only 1 std for removing outliers instead of 2 std.  If we use a range of 2 stddev, we get an average buy price of 56 and sell price of 77 and a higher total purchased share count of 6.3 million.  

Also for those who still think these numbers are unrealistic, FT has reported that retail trading continues to grow and is now the 2nd largest volume of all trading, after HFT/algo trades.  We are bigger than the ETFs, mutual funds and hedge funds:

https://archive.is/drLS7

**EDIT 2**  To be clear these numbers are for customer *orders* not transfers.  This is 6.1 million new shares net purchased during the last month, not including any transfers.

**EDIT 3** The median buy order size in this data is 34 and sell order is 56.  If you use these for order sizes, you would get 2.6 million purchased.