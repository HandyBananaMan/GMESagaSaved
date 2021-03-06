# Author: Theceilingis_theroof
# Post URL: [https://www.reddit.com/r/Superstonk/comments/n5go8a/massive_jump_in_vix_is_a_sign_of_things_to_come/](https://www.reddit.com/r/Superstonk/comments/n5go8a/massive_jump_in_vix_is_a_sign_of_things_to_come/)


I want to start off this post by saying that I am not a financial advisor.  All of this should be taken with a grain of salt.  Do your own research to back up beliefs you may have about the stock that you like.  I will site sources I used at the end with links.

I heard a couple of people, including Pixel, mention a few things about VIX, which is a volatility index that was created back in 1993 with the goal of giving real time analysis to market expectations of possible near-term price movements of the market.  Pixel was the first person I heard personally that mentioned it as something to look at for a guideline of market sentiment.  So occasionally I would sneak a peek of what was happening based of sentiment I could feel from r/GME and r/Superstonk.

Then yesterday, 5/4, I decided to check it again.  Needless to say, my tits were jacked.

Open up a banana and crack open a cold Fresca, cause it's about to get deep MF.

Before I get into all that though, I want to give you a little background on VIX and why we can view it as reliable for predicting short term price movement based off historical data and major historical events.  Then we will see if VIX has any correlation to price movement in GME and see if we can predict any possible events that may be coming (aka when moon).

So first some background.

Vix was created back in 1993 by Cboe (originally known as the Chicago Board Options Exchange (CBOE) which changed its name back in 2017.  The Cboe was founded in 1973 and is the world's largest options exchange.  Really what VIX calculates is not volatility but instead the expectation of possible future volatility or implied volatility.  Originally when it started it took into consideration the implied volatility of 8 separate S&amp;amp;amp;amp;P 100 put and call options but then expanded in 2002 to the S&amp;amp;amp;amp;P 500 for more accuracy.

So how does this whole thing work ?????  I'm glad you asked.

Two methods are used.

1. They perform calculations based on historical prices over a specific period of time.  Basically they find things like an average, mean, variance, and historical deviation on the data sets.  This allows them to calculate the risk.  Any time you want to know the future of a stock, you can go off the baseline of what it's done in let's say the last couple months and go off of that.  So they do that and take past data to find future implied volatility.
2. They infer that value of the stock based off of option prices.  Option prices are made according to the probability of it reaching it's strike price before it expires.  So to calculate the price of these options in most cases, the possibility of it reaching that set price is represented by a volatility factor and dictates the price of such options.  Since option prices are available to the open market, they are able to be used for data.  Boom, more data to show movement in pricing or implied volatility.

Okay so you grew a few wrinkles right?  Now how accurate is this fancy thing?  Get ready to look at some data with me.

I poured over some historical data correlating to historical events.  [Here is a link to the raw data.](https://cdn.cboe.com/api/global/us_indices/daily_prices/VIX_History.csv)

Here's some examples.

2001 WTC Attack in NYC

DATE,OPEN,HIGH,LOW,CLOSE

08/31/2001,25.310000,25.470000,24.410000,24.920000 09/04/2001,26.110000,26.170000,24.190000,25.850000 09/05/2001,26.220000,27.370000,26.220000,26.350000 09/06/2001,27.230000,28.730000,27.230000,28.610000 09/07/2001,29.890000,31.300000,28.920000,30.990000 09/10/2001,33.110000,33.340000,31.840000,31.840000 09/17/2001,43.200000,44.330000,39.770000,41.760000 09/18/2001,41.070000,42.170000,38.870000,38.870000 09/19/2001,37.880000,44.260000,37.500000,40.560000

Literally before 9-11-2001, they were showing implied volatility and then there was a massive jump on recorded date, 9-17-2001.  The stock market was closed until 9-17 due to the worry for panic selling. On 9-17-2001, the Nasdaq Composite index fell by 6.8%.

The Stock Market Crash of 2002

DATE,OPEN,HIGH,LOW,CLOSE

07/01/2002,25.710000,27.160000,25.630000,27.110000 07/02/2002,27.560000,29.780000,27.560000,28.960000 07/03/2002,28.880000,31.030000,28.760000,29.420000 07/05/2002,27.300000,27.300000,25.680000,27.110000 07/08/2002,28.540000,28.780000,27.880000,28.250000 07/09/2002,27.960000,30.340000,27.790000,30.220000 07/10/2002,31.400000,34.170000,30.770000,34.100000 07/11/2002,34.420000,36.350000,33.850000,33.850000 07/12/2002,34.300000,34.300000,32.410000,32.940000 07/15/2002,35.070000,38.380000,34.860000,35.030000 07/16/2002,35.970000,36.820000,35.200000,36.650000 07/17/2002,34.250000,36.730000,33.620000,35.450000 07/18/2002,35.200000,35.420000,33.450000,35.120000 07/19/2002,36.420000,38.170000,35.980000,38.170000 07/22/2002,39.130000,42.580000,38.570000,41.870000 07/23/2002,42.270000,46.130000,42.050000,44.920000 07/24/2002,48.170000,48.460000,39.830000,39.860000 07/25/2002,40.650000,42.050000,38.890000,39.270000 07/26/2002,38.610000,38.800000,35.510000,35.510000 07/29/2002,33.890000,33.890000,31.190000,31.330000 07/30/2002,32.040000,32.770000,30.600000,31.920000 07/31/2002,32.780000,33.680000,32.030000,32.030000

Again, showing steady and then increasing in implied volatility.  Well that July, The Dow Jones fell from it's March high of 10632.40 to 7702.30.

2008 Recession

Yet again, the VIX for almost the whole year went back and forth in the 18-22 range and then...

DATE,OPEN,HIGH,LOW,CLOSE

09/05/2008,24.540000,24.710000,22.970000,23.060000 09/08/2008,22.220000,24.060000,22.120000,22.640000 09/09/2008,22.690000,25.680000,22.580000,25.470000 09/10/2008,25.470000,25.480000,23.800000,24.520000 09/11/2008,25.380000,26.250000,24.390000,24.390000 09/12/2008,24.800000,26.670000,24.800000,25.660000 09/15/2008,25.660000,31.870000,25.660000,31.700000 09/16/2008,31.700000,33.700000,30.240000,31.540000 09/17/2008,30.250000,36.400000,30.250000,36.220000 09/18/2008,36.100000,42.160000,33.100000,33.100000

UH OH.  Looks ominous.  \*insert Billy Mays' voice\* BUT WAIT, THERE'S MORE!!

DATE,OPEN,HIGH,LOW,CLOSE

09/26/2008,34.760000,36.400000,34.440000,34.740000 09/29/2008,36.920000,48.400000,36.920000,46.720000 09/30/2008,43.770000,43.800000,38.860000,39.390000 10/01/2008,39.390000,42.380000,39.390000,39.810000 10/02/2008,39.820000,46.480000,39.820000,45.260000 10/03/2008,45.220000,45.520000,41.510000,45.140000 10/06/2008,45.120000,58.240000,45.120000,52.050000 10/07/2008,52.050000,54.190000,47.030000,53.680000 10/08/2008,53.680000,59.060000,51.900000,57.530000 10/09/2008,57.570000,64.920000,52.540000,63.920000 10/10/2008,65.850000,76.940000,65.630000,69.950000 10/13/2008,69.950000,71.420000,54.690000,54.990000 10/14/2008,55.100000,59.810000,46.350000,55.130000 10/15/2008,55.690000,69.470000,55.690000,69.250000 10/16/2008,69.210000,81.170000,66.510000,67.610000

Yeah, we all know what happened there.  Look at 9-29-2008.  The Dow Jones fell 777.68 in one day.

Let's just look at one more shall we?  Something more recent.

2020 Stock Market Crash

DATE,OPEN,HIGH,LOW,CLOSE

02/21/2020,17.330000,18.210000,16.190000,17.080000 02/24/2020,22.250000,26.350000,22.000000,25.030000 02/25/2020,22.190000,30.250000,22.190000,27.850000 02/26/2020,26.630000,29.570000,24.760000,27.560000 02/27/2020,28.950000,39.310000,27.790000,39.160000 02/28/2020,42.020000,49.480000,39.370000,40.110000 03/02/2020,34.860000,43.770000,31.500000,33.420000 03/03/2020,33.640000,41.060000,24.930000,36.820000 03/04/2020,34.440000,35.580000,30.300000,31.990000 03/05/2020,33.610000,42.840000,33.540000,39.620000 03/06/2020,41.460000,54.390000,40.840000,41.940000 03/09/2020,41.940000,62.120000,41.940000,54.460000 03/10/2020,49.680000,55.660000,43.560000,47.300000 03/11/2020,52.240000,55.820000,49.980000,53.900000 03/12/2020,61.460000,76.830000,59.910000,75.470000 03/13/2020,71.310000,77.570000,55.170000,57.830000 03/16/2020,57.830000,83.560000,57.830000,82.690000 03/17/2020,82.690000,84.830000,70.370000,75.910000 03/18/2020,69.370000,85.470000,69.370000,76.450000

Guess what happened on 2-28-2020?  The Dow Jones and S&amp;amp;amp;amp;P 500 each lost 4.4%.

Okay you got the picture now.  VIX is almost scarily accurate with predicting implied volatility.  Which led me to investigate, what is it doing with this entire GME situation.

Lets take a look

DATE,OPEN,HIGH,LOW,CLOSE

01/21/2021,21.340000,22.220000,21.090000,21.320000 01/22/2021,22.240000,23.730000,21.270000,21.910000 01/25/2021,22.310000,26.630000,22.200000,23.190000 01/26/2021,23.910000,23.940000,22.550000,23.020000 01/27/2021,23.820000,37.210000,23.710000,37.210000 01/28/2021,33.250000,36.290000,27.390000,30.210000 01/29/2021,35.160000,37.510000,29.240000,33.090000 02/01/2021,31.450000,33.960000,29.030000,30.240000

Do you know the date of the first tiny short squeeze?  That's right.  It started rising on 1-26 and was reaching its peak before being shut down and plummeting after 1-29.

The same thing for our rise to 270

DATE,OPEN,HIGH,LOW,CLOSE

02/19/2021,23.10, 23.190, 20.84, 22.05 

02/22/2021,24.460, 25.090, 21.96,2 3.45 

02/23/2021,22.820, 27.01, 22.50, 23.11 

02/24/2021,23.760, 25.04, 21.310, 21.340 

02/25/2021,21.730, 31.16, 21.52, 28.89 

02/26/2021,28.73, 30.820, 25.230, 27.95 

03/01/2021,25.200, 25.39, 23.17, 23.35 

03/02/2021,23.58, 24.60, 22.80, 24.1 

03/03/2021,22.80, 26.790, 22.45, 26.67 

03/04/2021,26.520, 31.90, 24.90, 28.57 

03/05/2021,29.40, 30.03, 24.33, 24.66 

03/08/2021,27.61, 28.39, 24.07, 25.47 

03/09/2021,25.11, 25.250, 22.90, 24.03

We had that big quick jump on 2-25 to 170.45, then on 3-4 was the start of our rise upward.

So now we've proven that it correlates to GME rapid price movements, probably because of GME's negative beta affecting the broader market and the S&amp;amp;amp;amp;P 500.

Which leads me to why my tits are jacked.

5-4, there was, at it's peak for the day, a 19.06% increase in VIX for a high of 21.80.  With a lot of this sideways trading, the implied volatility has dropped considerably.  Here's the data.

DATE,OPEN,HIGH,LOW,CLOSE

4/09/2021,17.05, 17.34, 16.20, 16.690 

4/12/2021,17.43, 17.910, 16.81, 16.910 

4/13/2021,16.990, 17.86, 16.43, 16.650 

4/14/2021,16.71, 17.690, 15.38, 16.9

4/15/2021,16.780, 16.920, 15.940, 16.570

4/16/2021,16.650, 16.88, 16.050, 16.25

4/19/2021,17.040, 18.610, 16.78, 17.29

4/20/2021,17.360, 19.70, 17.24, 18.68

4/21/2021,18.48, 19.29, 16.91, 17.50

4/22/2021,17.280, 19.90, 16.990, 18.710

4/23/2021,18.560, 18.780, 16.80, 17.330

4/26/2021,17.94, 18.17, 16.87, 17.64 

4/27/2021,17.62, 18.160, 16.97, 17.56 

4/28/2021,17.47, 17.84, 16.77, 17.6

4/30/2021,17.67, 19.25, 17.64, 18.61 

5/03/2021,18.65, 19.12, 17.8, 18.31

You see how low VIX has been even and it's peaks?  Now there's a pretty sizable jump in implied volatility.  I'm keeping an eye on VIX from here on out that's for sure.  (It's able to be seen on Yahoo Finance and you can follow it right along with GME.  Not sure how else but that's the easiest way I've found)

Now time for my opinion on what we could possibly see.  This is purely speculation and just my thoughts.

After looking at all the historical data, my thoughts are that anything over 30 for VIX is significant.  But really it's not about those big jumps, because those are just days that there is massive movement.  It's really about those days leading up and seeing a steady climb in VIX that's telling.  I personally think that whatever is about to happen is going to bring a massive market crash, larger than at least the one last year.  I feel that if we see VIX rise past the 24-26 mark for a high on the day, and stay around there for maybe 2 or more days (May not even be needed.  It could be a major quick jump, like a rocket launch?), then it's about to go down.  THAT is why my tits are jacked.

TL;DR: Please just try to read the most you can because it's pretty awesome to see.  The VIX shows the implied volatility for the markets based off the S&amp;amp;amp;amp;P 500 and can accurately predict major movements that will happen in the market.  VIX has a direct correlation with GME rapid movement.  Today there was a massive jump in VIX.  I predict more to come.  Just buy, hodl, vote.  

Ground Control to Major Tom....

????????????????????

[VIX Historical Data](https://www.cboe.com/tradable_products/vix/vix_historical_data/)

[VIX Volatility Chart](https://www.macrotrends.net/2603/vix-volatility-index-historical-chart)

[Info About What VIX IS](https://www.investopedia.com/terms/v/vix.asp)