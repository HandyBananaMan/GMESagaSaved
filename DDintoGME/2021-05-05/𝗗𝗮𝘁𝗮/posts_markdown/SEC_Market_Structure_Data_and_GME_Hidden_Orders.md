# Title: SEC Market Structure Data and GME Hidden Orders
# Author: CruxHub
# Post URL: [https://www.reddit.com/r/DDintoGME/comments/n582tm/sec_market_structure_data_and_gme_hidden_orders/](https://www.reddit.com/r/DDintoGME/comments/n582tm/sec_market_structure_data_and_gme_hidden_orders/)


Fellow apes, I wanted to present a source of market data related to the trading of GME which I have not seen previously analyzed here. I am an infant ape when it comes to the complexities of market structures and specific trade types (I only know buy and hodl), however I thought this information - with a focus on "hidden" orders - would be of interest even in a basic form. This is not financial advice, I prefer the taste of green crayons over red and have typed this with my toes.

**TLDR at the bottom**

**Background**

The U.S. Securities and Exchange Commission (“SEC”) comprises several divisions and offices, one of which is the [Division of Trading and Markets](https://www.sec.gov/divisions/trading-markets). What is the Division of Trading and Markets *supposed* to do?

>The Division of Trading and Markets establishes and maintains standards for fair, orderly, and efficient markets. The Division regulates the major securities market participants, including broker-dealers, self-regulatory organizations (such as stock exchanges, FINRA, and clearing agencies), and transfer agents.

Setting aside the question of how effective the Division of Trading and Markets are accomplishing these tasks, they also perform [market structure research](https://www.sec.gov/marketstructure/research-and-analysis), which includes the compilation of market data and performing [Market Structure Analytics](https://www.sec.gov/marketstructure/market-structure-analytics). They do this through the [Market Information Data Analytics System](https://www.sec.gov/marketstructure/midas-system) (“MIDAS”).

MIDAS sounds pretty cool (if you’re an 8 year old), but what does it actually do?

Apparently MIDAS compiles a shit-load of data:

>Every day MIDAS collects about 1 billion records from the proprietary feeds of each of the 13 national equity exchanges time-stamped to the microsecond.. . .Specifically, MIDAS collects:Posted orders and quotes on national exchangesModifications/cancellations of those ordersTrade executions against those ordersOff-exchange trade executions

So the SEC collects a bunch of data. What do they do with it? The SEC touts the qualities and applications of MIDAS:

>...It can help us **monitor and understand mini-flash crashes**, **reconstruct market events**, and develop a better understanding of long-term trends.

Great, the SEC claims they have data which could show the chicanery going on with a stock, maybe even GME.

**So what does this have to do with GME?**

The SEC actually makes some of this MIDAS data available. No shit? Yep, your tax dollars at work. We can’t see the full order book and billion data points collected per day, but they do provide aggregated metrics on exchanges and, pertinent to this post, some metrics by security.

The SEC provides quarterly downloads of metrics for over 4,800 securities [here](https://www.sec.gov/opa/data/market-structure/marketstructuredownloadshtml-by_security.html). This is daily data by security compiled from various exchanges:

>Order-based exchanges: Arca, Bats-Y, Bats-Z, Boston, CHX, Edga-A, Edge-X, Nasdaq, NSX, PHLXLevel-book exchanges: Amex, NYSE

They also provide downloads of [daily data for each security by exchange](https://www.sec.gov/opa/data/market-structure/market-structure-data-security-and-exchange.html). There are other notes on the website and in the README.txt that accompany this data; for brevity I will skip covering that here.

What kind of metrics does the SEC provide?

* McapRank
* TurnRank
* VolatilityRank
* PriceRank
* Cancels
* Trades
* LitTrades
* OddLots
* **Hidden**
* **TradesForHidden**
* OrderVol
* TradeVol
* LitVol
* OddLotVol
* **HiddenVol**
* **TradeVolForHidden**

Hidden trades... interesting. Haven’t we seen some DD on these before? Yes, ape-with-many-wrinkles [u/jsmar18](https://www.reddit.com/u/jsmar18/) has done a deep dive on order types including these Hidden trades, his most recent post is [here](https://www.reddit.com/r/Superstonk/comments/n1w89c/how_hfts_are_creating_the_180_sell_wall_questions/). I encourage you to read his work, and I’m not going to cover it here. **The key takeaway is that hidden orders allow HFTs to “jump the line” ahead of visible orders.** AKA HFT fuk retail.

[Here](https://www.sec.gov/marketstructure/market-activity-report-methodology) is how the SEC describes these hidden trades (emphasis added):

>We use the term “Hidden Trades” to mean trade executions on an exchange that are t**he result of a marketable order matching an undisplayed, or hidden, resting order**. The exchange feeds do not generally provide messages related to the addition of undisplayed orders. But many provide an indicator or other method for identifying when trade executions (which are not themselves hidden) involved a resting undisplayed order.

If we examine this data will we find confirmation of HFT fuckery? I’m guessing we will. Let’s dig in.

**Examining the MIDAS data**

I compiled a subset of the daily security and daily security/exchange data, which ends Q1 2021.

First, let’s start at a high level. Here is a chart from Jan 2020 - Mar 2021 of GME’s daily closing price and volume per Yahoo Finance, and the “HiddenVol” from MIDAS. I decided to use Yahoo Finance reported volume because the “OrderVol” from MIDAS appears to include volume for all orders and that appeared high, because it isn’t limited to executed trades. The SEC defines “HiddenVol” as the “\[s\]um of trade volume for trades against hidden orders from exchanges that report trades against hidden orders.” So hopefully I’m comparing apples-to-apples.

![GME - Daily Volume, Hidden Volume and Closing Price; 1\/2\/2020 - 3\/31\/2021](https://preview.redd.it/9g5j1szxj8x61.jpg?width=684&format=pjpg&auto=webp&s=4cee745e5adc2b823c92b899859650e29fe9be26)

Tough to tell much at this scale, but you can see when there are major spikes in volume (blue line) there is also a spike in the “HiddenVol” (orange line).

What does a “regular” stock look like?

![AAPL - Daily Volume, Hidden Volume and Closing Price; 1\/2\/2020 - 3\/31\/2021](https://preview.redd.it/l2omdtgzj8x61.jpg?width=684&format=pjpg&auto=webp&s=ce42f0927ffb8e38bbdd748f1eb5616f96ea2a8a)

Some pretty big swings in volume, and a couple periods where the “HiddenVol” stand out, but not nearly as prominent of spikes as GME.

![WMT - Daily Volume, Hidden Volume and Closing Price; 1\/2\/2020 - 3\/31\/2021](https://preview.redd.it/n4prxd71k8x61.jpg?width=684&format=pjpg&auto=webp&s=bb3d8a58170c58f5f828f71a17b747fee554c16b)

Not terribly exciting, but visually the small spikes in “HiddenVol” appear to correlate to spikes in volume.

Let’s not forget our favorite ETF, XRT!

![XRT - Daily Volume, Hidden Volume and Closing Price; 1\/2\/2020 - 3\/31\/2021](https://preview.redd.it/lbfcyyr2k8x61.jpg?width=684&format=pjpg&auto=webp&s=86423ee15db036905f3c30458b5f2ca10dc18a2b)

Hmmm what stands out here?

Let’s move back to GME and focus on Q1 2021.

![GME - Daily Volume, Hidden Volume and Closing Price; 1\/4\/2021 - 3\/31\/2021](https://preview.redd.it/j6mrzz74k8x61.jpg?width=684&format=pjpg&auto=webp&s=8b44b6b8ddd684f42628f6cc714c705d87242e9a)

Gee, lots of hidden order volume on the dates major fuckery occurred. No way!

What does the XRT Q1 2021 chart look like?

![XRT - Daily Volume, Hidden Volume and Closing Price; 1\/4\/2021 - 3\/31\/2021](https://preview.redd.it/afakeh86k8x61.jpg?width=684&format=pjpg&auto=webp&s=c918b97211f639be5a902ade91986bbad87dfb5f)

Definitely hidden order volume on the dates major fuckery occurred as well. Not as prominent on the other days compared to GME.

Back to GME - what percent of the daily volume is from these hidden orders?

![GME - Daily Volume and Hidden Volume; 1\/4\/2021 - 3\/31\/2021](https://preview.redd.it/e3ow0ej7k8x61.jpg?width=684&format=pjpg&auto=webp&s=3f58bb8e30cd2abd613f4f1822db824a8af227ab)

Never more than 20%, but it spiked in the late January run-up and has stayed at or over 10% since late February. Still, that's a shitload of shares. Sometimes millions per day.

Now let’s look at Q1 2021 Hidden Volume by exchange for GME.

![GME - Daily Hidden Volume by Exchange; 1\/4\/2021 - 3\/31\/2021](https://preview.redd.it/eiraxug9k8x61.jpg?width=684&format=pjpg&auto=webp&s=a4e53e9b9dfa103c1196f2dd85635e0c24623ea0)

Who are the winners? Arca (dark orange), Edge-X (brown), Nasdaq (dark green) and NYSE (light orange).

What I found particularly interesting is that IEX reports 0 hidden volume for all of Q1 2021. Maybe it’s a data issue or maybe they just don’t have that order type? I know they’re seen as the best exchange to route orders so perhaps this makes sense.

Let’s drill into the top 4 I called out above.

![GME - Daily Hidden Volume for Arca, Edge-X, Nasdaq and NYSE Exchanges; 1\/4\/2021 - 3\/31\/2021](https://preview.redd.it/v4r6wwqak8x61.jpg?width=684&format=pjpg&auto=webp&s=771d9dd5d6b593de020b6c1601b63d0ce5e7891c)

Most of the hidden volume is running through Nasdaq, with a tie for second place between Arca and NYSE.

I could go on with many more charts, but at this point **it is clear that HFTs have used and continue to use hidden orders when trading GME.** **~~This is a special type of order not available to retail investors.~~** 

**EDIT 1 (May 6)**:  u/Musaran2 pointed out that hidden order types actually **are** available to some retail investors, at least those who use Interactive Brokers.  I confirmed it [here](https://www.interactivebrokers.com/en/index.php?f=596).  IB says this about hidden orders (emphasis added):

>Investors wishing to hide large-size orders can do use by applying the "Hidden" attribute to a large volume order to completely hide the submitted quantity from the market. **The Hidden order type is a simple solution to maintaining anonymity in the market when trying to buy or sell large amounts of stocks**, options, bonds, warrants, futures or futures options. The Hidden order type is simple to add to the main trading window within TWS and requires a simple check-mark in the box in order to activate. Display the Hidden field from the Layout Manager, and check the Hidden attribute in the order line. Your order is submitted but evidence of the order is hidden from the market.

So if someone hypothetically used hidden orders to hide a large volume of buys but left the sells. on the "lit" market would this influence the price?   Hmm....

**End EDIT 1** 

**TLDR:**

* **The SEC claims to collect order execution data sufficient to reconstruct market events like flash crashes.**
* **The SEC makes some of this data publicly available, including volume from “Hidden” orders - an order type HFTs use to “jump the line” and fuk retail.**
* **The SEC’s own data confirms “Hidden” orders are consistently used when trading GME - nearly 20% of all volume on some days! This is millions of shares!**

Is this level of hidden orders manipulation or something else? I don’t know I’m not a market expert, but we’ve got some data on it.

I welcome your comments, questions and corrections. If apes find this line of investigation interesting I can continue digging, there is a lot of data left to explore.

💎🙌🦍🚀🚀🚀🚀