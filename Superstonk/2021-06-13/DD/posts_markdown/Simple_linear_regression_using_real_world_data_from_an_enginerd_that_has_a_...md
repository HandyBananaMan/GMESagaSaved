#Title: Simple linear regression using real world data from an enginerd that has a hard on for statistical modeling and analysis.
#Author: PWNWTFBBQ
#Post URL: [https://www.reddit.com/r/Superstonk/comments/nzcg0j/simple_linear_regression_using_real_world_data/](https://www.reddit.com/r/Superstonk/comments/nzcg0j/simple_linear_regression_using_real_world_data/)


# Debunked: Incorrect Assumptions

The below data analysis has been determined to be not accurate due to GME trend to not follow a single linear line that fits perfectly by date. I tried to apply the exponential floor theory and make it work but was unable to do so. Also, using the most common rate of change was wrong.

# Post

This is not financial advice.  I am merely a fucking autistic number crunching, experiment running engineer. I decided to do some finagling with some real world data since I was able to get to a computer that has excel. The following is fairly "basic" and none of it required a fancy software. I'll do something with that later.

This is another view point at looking at low share price data that extends from a [previous post](https://www.reddit.com/r/Superstonk/comments/ny68t6/technical_analysis_from_an_enginerd_that_has_a/) I did. I wanted to add a mathematical backing to determining lowest share price versus have to do a guess and check. Below is how I came to the equation that was able to predict the lowest share price and how things are going as planned even if the share dips (PTSDdog.jpg) below the regression line.

# Simple Linear Regression!!! WTF is it?!

Linear regression is a type of trend analysis where a linear relation approach is used to model a relationship between a independent and dependent variable. An independent variable is the entity that is not influenced by a different variable. A dependent variable is one whose value is influenced by an independent variable.

When only a single independent variable is used to analyze the behavior of a dependent variable, it’s called simple. When there are more than one independent variables in the model that has been created, it is called multivariate (multiple – variable).

# Mathemagical Stuff!

Simple linear regression lines have the following format:

y = mx + b

Here, y is represented by our dependent variable. The rate of change (m) is the ratio of how much the dependent variable changes relative to the independent variable. The variable, b, is the y-intercept.

Time for “a perfect world” ape example:

Let’s say we have been tracking the number of apes that have joined the r/superstonk community since it first began. For the moment, we live in a perfect world. The number of apes (our dependent variable) has increased by 1,000 with each passing day (our independent variable). Therefore, the rate of change aka slope (m) would be 1000 apes / 1 day.

So, let’s find our b which is our y -intercept. This can be found by figuring out what y is when x = 0. Sometimes, this is found in a nice data date or looking at a graph. For our particular ape example, we have collected the following data:

&#x200B;

https://preview.redd.it/s35h1t3l45571.png?width=177&format=png&auto=webp&s=49c4491b5ceafca3a54b116edcf0ee608f48d8b6

But I can’t read so let’s also make a graph:

&#x200B;

https://preview.redd.it/eixq0koy45571.png?width=581&format=png&auto=webp&s=10945b222a6f4f33857e86a6dc6977a68f44516d

Looking at the data table and the graph, we see that when Day = 0, there are 2,000 apes. So, when r/superstonk just started, we immediately had 2,000 apes subscribed. All this information would give us the following equation:

Number of Ape Members = 1,000 (Day) + 2,000

The equation looks really nice but life is a struggle, and we don’t live in a perfect world. Let’s look at more likely type of data set where we don’t have such a clear cut regression line. Here is an example data table and the associated graph:

&#x200B;

https://preview.redd.it/6h69b9xg45571.png?width=179&format=png&auto=webp&s=c3bf2ccf9f3447d76fafad4eee52f68a2ae967e6

&#x200B;

https://preview.redd.it/vl3uw4r755571.png?width=783&format=png&auto=webp&s=7a210f2953d1609a45b53d82b1647ee3c827554e

At the top right of the graph, we have our regression line where our slope is 1088.2 and our y-intercept is 1945.6.

WTF is this new R\^2 thing? R\^2 (pronounced R squared) is a goodness of fit measurement. It tells us how good the model and how well we could predict the number of apes members for any given day. In more wrinkle brain speech, it is the percent variance of the dependent data relative to the independent.  This value ranges from 0 to 1 where 0 is the shittiest type of model and 1 is perfect. Depending on the environment where the data is taken as well as what the independent and dependent variables are, anything about 0.8 would mean we have a good model and anything less if questionable to fucking useless.

In our perfect world example, the R\^2 would be 1 since it is a perfect world and the data collected was without any error. For our second graph, our R\^2 is 0.9872. Since 0.9872 is above 0.8 and very close to 1, we can confidently conclude we have made a really good model at predicting the number of apes on any given day. However, since R\^2 is not equal to 1, it means there is still error within our predicted equation.

So, we have error which will be represented by “e”. Incorporating error (e) into the simple linear regression equation from above, we have:

y = mx + b + e

Error, (e), is a calculate value that is unique to each data point. It is the difference between the value that was measured versus the theoretical value.

For our real world ape example, we would calculate the theoretical number of apes using the equation of the trendline.

Apes  = 1088.2 (Day) + 1945.6

For Day = 1, we would have:

Apes = 1088.2 (1) + 1945.6 = 3033.8

Therefore, our error would be the difference of apes we counted and the number of predicted apes we calculated. We would have this table:

&#x200B;

https://preview.redd.it/xgn0tm3b55571.png?width=535&format=png&auto=webp&s=1986fc57f2b8a6c4283cebcbdb294c4f765dfe94

We can also look at the graph we made to see the error. The error is how much the actual value deviates from the regression line as shown in orange.

&#x200B;

https://preview.redd.it/ilddcxbe55571.png?width=782&format=png&auto=webp&s=fad4d54c16ee610cd22195ce475bfcfeaf46ee47

For a better view of the error, I zoomed into Days 4 -7. The blue line is our regression. The blue dots are the number of apes we counted. The green dots are the theoretical number of apes given our regression line. The orange is the error of the actual and the theoretical.

![ ](https://preview.redd.it/upi1u45h55571.png?width=784&format=png&auto=webp&s=c5d785ce7c91f047065d69df5d94f2f7316e4e39)

# Time to Fuck Around with Real Share Price Data

Let's look at GME share price vs. Date. Specifically, I'll be looking into lowest share price by date.

&#x200B;

https://preview.redd.it/b50mxuj5i5571.png?width=679&format=png&auto=webp&s=466673d54dd56bebe4add600164df7631ea8e32a

I decided to do some more accurate trend analysis which would remove the “eyeballing” that's been done to determine  lowest share price. I began by focusing on formatting data. Due to the constant shorting and how the overall trend goes up, I removed a significant amount of data points that were much smaller than the previous day's price. After wards, I looked into the typical rate of share price by day values. Since this is a linear regression and all the rates of change are positive, I knew I would see normal distribution but only half due to a positive rate of change.

&#x200B;

https://preview.redd.it/jvfolhnn55571.png?width=774&format=png&auto=webp&s=2c859ce2e2c986d46cf5a76ccef81802554c5f60

This also helped to determine which data points were more so biased. I was thus able to create a graph focusing on the dates that had an unbiased rate of change.

&#x200B;

https://preview.redd.it/f4qyrdaq55571.png?width=624&format=png&auto=webp&s=2bd20cdebd1abb2dec1a908513a642812e518970

July 21, 2020 was set to my original date because it was the first to have an upwards value as well as a rate of change that was within the previous distribution rate of change histogram. This would suggest that July 21, 2020 was around the first day when things were “chill.”

https://preview.redd.it/7o9xbngu55571.png?width=614&format=png&auto=webp&s=39efab3b67a58b8d1dc0f5ab61b8ceb956c77837

After all that data formatting, we finally came to our conclusive log regression line of

y = 0.0055x + 0.4993

BUT WE DON’T LIVE IN A PERFECT WORLD SO THERE IS ERROR!!

Let’s account for error by using a thing called error bars:

&#x200B;

https://preview.redd.it/0b09ca8y55571.png?width=795&format=png&auto=webp&s=ee9a53d1aa8fbc8ef36114ce3c50c6ee73dd6a6e

Those little cross hairs on the orange dots are called error bars. Given a regression line, these little guys will confidently tell us what values above and below the line are adhering to the trend. This goes back to the error value as explained above. Any value outside these cross hairs typically are outliers. I’ll guess these outliers are due to hedgefunds so we can remove those because we are looking for an unbiased curve. The R\^2 value has increased because we were able to remove outliers and thus produce a better model.

We now have our theoretical predicting equation based on real world data. Our R\^2 value suggest this is a strong model for predicting a share price trend without a bias. So, now let’s apply this to the rest of the share price graph:

&#x200B;

![  ](https://preview.redd.it/u5ygjiu165571.png?width=793&format=png&auto=webp&s=54bc96cfd3b5bff4d7e2cc858414d178f92eda99)

The areas I find of most interest are where the blue share price data is parallel to the regression line. This is great because there are multiple areas throughout a long history. We now have the equation:

y = 10\^(0.0056x + 0.5103)

And get this graph:

&#x200B;

![  ](https://preview.redd.it/cga2l8w465571.png?width=790&format=png&auto=webp&s=93e47fe4bcd6335de4679764bbdb34ebd15a90d0)

There you go, folks. A simple linear regression of the share price using a regression line that was derived from real world data.

**TL;DR**

The lowest share price value has been following a solid trend and we are still heading on an exponential path to Valhalla. There will be values above and below a regression line when using actual data. Given enough data points, one can create a decent model of an independent and dependent variable. We don’t live in a perfect world so just chill your tits if a share value doesn't go as predicted. Shit happens. Hold the line.

Edit 1: [Stock Price Data](https://finance.yahoo.com/quote/GME/history?p=GME)

Edit 2: [tweet](https://twitter.com/pwnwtfbbq/status/1404267817562644484) and added to TLDR.

Edit 3: Added some more to the introductory.

Edit 4: Added some more intro shit / grammar