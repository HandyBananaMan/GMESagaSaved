# Author: PWNWTFBBQ
# Post URL: [https://www.reddit.com/r/Superstonk/comments/ny68t6/technical_analysis_from_an_enginerd_that_has_a/](https://www.reddit.com/r/Superstonk/comments/ny68t6/technical_analysis_from_an_enginerd_that_has_a/)


I am not a financial advisor. I am merely a fucking autistic number crunching, experiment running engineer. This is my view point.

With all the various technical analysis people chiming in, I figured I would provide my thoughts from an engineering statistics view. Engineering stats is different from financial stats because we are more focused on the data as a whole and only concerned with outliers when there are a shit ton of outliers. This is an over generalization but I’m giving a quick explanation on how this approach is different from the rest. I also only used log ape’s data since the EW, sideways trading, and gamma apes use a financial analysis technique that is too financial analysis-y and not pure mathemagically.

I’m not bothered by how the last few data points were below the log equation and here’s a few reasons why:

1. Outliers are common in any distribution.
2. Data points usually deviate from a trend due to some form of bias.

**Outliers are common in multivariate regression.**

For the sake of easier understanding, I am only going to address the normal bell curve distributions. There are two important statistical values to this type of distribution. The first is the average / mean represented by μ. The other is the standard deviation represented by σ.

For a given data set that has a normal distribution, 68% of the data will fall within +/- 1 σ. 95% of the data will between +/- 2 σ. Finally 99.7% will fall within +/- 3 σ. This is called the 68 - 95 - 99.7 rule in stats.

&#x200B;

[I'm so pretty, I model.... statistical model.](https://preview.redd.it/i00678hl0u471.png?width=500&format=png&auto=webp&s=e3209c34f950dd5685c044a2220bcc13ab078d5f)

So, if you know the distribution of a data set, you’ll know what percentile a single data point will fall into in comparison to the rest of the data. Percentiles are great because they can also act as probabilities. Here is an ape level example to show how:

Let’s say we have a group of 100 crayons all with different lengths. For this particular group of crayons, the average length of a single crayon is 10 cm, and the standard deviation is 1 cm. That means 68% of the crayons are going to be 9 - 11 cm. 95% of the crayons will be 8 - 12 cm, and 99.7% of the crayons are going to be 7 to 13 cm. It would create this type of distribution:

&#x200B;

[MMM crayons](https://preview.redd.it/eyllc4ipcu471.png?width=1792&format=png&auto=webp&s=5f5d8bfe8283a8ad024a4f6c312f67537bf62dee)

Here is where the probability part comes in:

Let’s say you suddenly had a crayon that was 13 cm long which according to our graph is 3σ away from the average. Looking at the pretty graph, we can see that a 13 cm long crayon is bigger than 99.85% of the rest of the crayons. Where did the 99.85% come from? We counted all the crayons that were less than 13 cm to include anything below 7 cm:

2.35 + 13.5 + 34 + 34 + 13.5 + 2.35 + 0.15 = 99.85%

But what the fuck? Where did that additional 0.15 come from when +/- 3σ is 99.7% It came from also counting in the number of crayons that are below 7 cm in length. Since probability cannot be greater than 100% and this is a symmetrical curve, 0.15% of the crayons are less than 7 cm because

100 - 99.7 = 0.3 (the percent of crayons either greater than 13 cm and less than 7 cm)

0.3 / 2 = 0.15 (the percent of crayons less than 7 cm OR less than 7 cm).

A 13 cm long crayon is super rare. In fact, there is only a 0.15% probability of getting a crayon 13 cm or longer.

Let’s now look at log ape’s graph:

&#x200B;

[That's some pretty fucking solid eyeballing.](https://preview.redd.it/pbtv657s5u471.png?width=1600&format=png&auto=webp&s=164a9db39188d1f6d2aa413a6f478bd8720a0f83)

From this graph there are only 2 values out of a total of 175 data points that would be considered “outliers.” I use outliers to mean values that do not fit the trend which is above the equation. 2 / 175 points is a mere 1.1% of the population. This amount is within reason for any regression type modeling.

Note: this is extremely over simplification and a lot of things have been aped down for easier explanation. I won’t be getting into that statistical calculation stuff because it’s higher end so Imma stick to keeping it smooth brained…. If I were on my work computer that has my fancy statistical analysis software, I would go balls to the wall. Sadly, I left that at work (where it belongs),

**Data points usually deviate from a trend due to some form of bias.**

I’ve been looking into log ape’s data and noticed that his variable “d” accounts for all days to include the weekend. 6/7 is day 250 and 6/4 is day 247.

[6\/7: d = 250](https://preview.redd.it/p03b5h9z5u471.png?width=1431&format=png&auto=webp&s=d312f4a748086d6d2faa8a54fd309fb5135f945f)

[6\/4: d = 247](https://preview.redd.it/elsgsgy36u471.png?width=1414&format=png&auto=webp&s=a58d87829011beda2cbb9b6d36655de92e9b6c5c)

If you were to only do business days, the dates would have a different associated d value. So, let’s try to redo log ape’s equation to only do trading days. The above graph would shift to look like this:

&#x200B;

[Well, fuck. There are lot more dips below the log equation.](https://preview.redd.it/gafj8u3b6u471.png?width=1600&format=png&auto=webp&s=0c80d45ccedd75e99d0f95ad88382c9ae31d1541)

Since log ape’s graph included the weekend, this compounded value would cause an influence on the resulting equation and would get more and more off due to more and more added weekends. Let’s see what those intersections were that are essentially a bias causing a large deviation between the lowest share value and the log ape’s equation:

[This graph has more dates than I do. #4EvaAlone](https://preview.redd.it/coksvisatu471.png?width=2591&format=png&auto=webp&s=d3804613538928b42aa059540c112b28b0d6528f)

Interesting… So from the graph, the most common cause for the lowest share price values to drop below the log ape’s equation is when a new GME board member is announced. Followed by legislation, shares filing, and the holy FTD settlement theory.

Long story short: When a trend deviates from it’s normal trend, it is typically due to a bias. Calm your tits. We’re still gucci. Log ape is fucking amazing for inspiring me and being my mathemagical muse.

**TL;DR**

**Hold the line.**

So big shout out to log ape for eye balling a pretty fucking solid equation. I’m thoroughly impressed. I wish I had excel to do goal seek but I’m not going to pay to buy MS office on my home computer.

Data sources:

[Share Price Data](https://finance.yahoo.com/quote/GME/history?p=GME)

[GME History](https://gmetimeline.com/)

Edit 1: Updated the photos so they aren't for ants.

Edit 2: Worded additonal biases into explanation.

Edit 3: I am not saying exponential floor ape is wrong in any way. I am merely presenting a different method of viewing the data. Without exponential floor ape and his DD, none of this would be possible.

Edit 4: pinging u/JTH1 for his point of view and reponse.

Edit 5: The equation itself is not an exact measurement because the values in the original equation itself were guesstimated. Therefore, there will be inherit deltas due to inaccuracies. Yes, there are a bunch of other variables that can affect this trend but that would require some form of metrology that takes into account the human factors. I would argue this current trend line is capable of describing the majority of the model due to its high R\^2 value. This isn't exact science nor a perfect model. It's hand wavy stats based around real world events.

Edit 6: Updated crayon bell curve for better visual explanation.

Edit 7:  u/WhatCanIMakeToday suggested I replace guy with ape. I took his advice.

Edit 8: I figured I would make a [tweet](https://twitter.com/pwnwtfbbq/status/1403717359899090946) about this to share.

Edit 9: Edited event graph to add all dates.

Edit 10: Added more events within the dates. If you look at the trend and remove the "outliers," you would see the more "natural" lowest share price. It would appear that these specific dates had a greater bias than the others.

Edit 11: Exponential ape derived his equation looking at a definitive value. So, while it would appear that causing a shift would deviate from the original intent, it also doesn't since I'm looking at different types of data. The curve he presented fits the overall trend VERY well and we are viewing the data in different ways. He is looking at a constant value while I am looking into rates of change due to biases. In other words, he can give you a value, and I can give you the most influential reasons why it may change.