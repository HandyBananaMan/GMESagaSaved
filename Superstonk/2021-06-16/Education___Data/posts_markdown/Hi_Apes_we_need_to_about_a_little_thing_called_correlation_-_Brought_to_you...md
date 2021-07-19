# Title: Hi Apes, we need to about a little thing called “correlation” - Brought to you by the Superstonk Quants 🦍 📊 👨‍💻🚀
# Author: orangecatmasterrace
# Post URL: [https://www.reddit.com/r/Superstonk/comments/o1a73z/hi_apes_we_need_to_about_a_little_thing_called/](https://www.reddit.com/r/Superstonk/comments/o1a73z/hi_apes_we_need_to_about_a_little_thing_called/)


Hi everyone, u/orangecatmasterrace here to discuss correlation, statistics, and things that we need to keep in mind when putting together our DD, specifically using this particular measure. I'm hoping to share this information so that this sub as a whole can be **more data-driven** in the compiling of our DDs and **more purposeful** in how we share this information with the rest of the apes.

**TA;DR** – “Correlation” should be considered a *sacred word* for DD writers. We need to use this word only when talking about statistical relationships between things, not just when things “look similar.”

&#x200B;

**Disclaimer**: I'm going to try to keep this post as smoothbrain-certified as possible. There's going to be some more technical parts of this that I'm going to omit for ease of explanation, but I'll be more than happy to hash out that kind of stuff in the comments.

The impetus for this post is something that I, along with other members of the [Superstonk Quants](https://www.superstonkquant.org/) have noticed recently – there have been some fairly high-visibility posts using the term “correlation” in their DD somewhat colloquially, and I think we need to re-ground ourselves about this term and what it actually means, *particularly so* within the DD writers.

“Correlation” is not a term that should be used flippantly when attempting to address the relationship between two things. I know it's easy to fall back on it to talk about two things being related somehow; it's become almost synonymous with the term “relationship” when discussing the market dynamics in here. However, I'd like to discuss how we can be better as a data-driven (and banana-fueled) sub to ensure that we're using as many wrinkles as we can when pulling important DD together and communicating that information out to the wider group. 

I'd like to break this discussion down into 4 parts:

1. What is Correlation?
2. Examples and Visualizations
3. Application to our DD
4. Closing Thoughts

&#x200B;

# What is Correlation?

We need to start things off by growing a wrinkle here. Let's do just that by learning **what the heck correlation is**. According to [Investopedia](https://www.investopedia.com/terms/c/correlation.asp), correlation “describes the degree to which two variables move in coordination with one-another. If the two variables move in the same direction, then those variables are said to have a positive correlation. If they move in opposite directions, they have a negative correlation.”

Alright, lets highlight the key points from this to know what we need to focus on:

* We need to look at 2 variables
* They have to "move"
* Direction matters
* Strength of relationship isn't a true or false matter - it's on a spectrum

Ok, so lets go through each of these points and see if we can't grow some *more* wrinkles. I promise this is good for you.

I brought mayo memes to help 😏

**Variables** – We know that we need 2 things to compare. What kinds of things can we compare to arrive at a correlation? Generally speaking, we need 2 variables that are continuous and numeric (number of bananas, or volume of mayo). Trying to compare categorical, or descriptive variables (color of Lambos, or brand of mayo) on their own makes this calculation something different altogether. For the sake of this conversation, we're going stick with the conclusion that we need to work with 2 number-like things to analyze.

**Movement** – So when the definition says that the variables have to “move,” this basically means that we need more than 1 data point from each of the 2 variables to compare against. Ideally, you want many data points to compare to each other. Attempting to conduct this kind of analysis on a small dataset (3 - 6 data points, for example) can lead to issues where correlations may appear to be present, even though none exist. You tend to need more than just a handful of data points to confirm that a relationship truly exists.

**Direction and Strength of Relationship** – Direction and Strength of Relationship are measured on a continuous scale (the correlation coefficient) from -1 to +1.

* Our variables can be positively correlated when their values change in tandem – as one variable increases, the other increases (as the volume of mayo that Kenny consumes increases, the measurement of his waistline in inches increases).
* Our variables can also be negatively correlated – as one variable increases, the other decreases (as the number of bananas I purchase increases, the amount of tendies in my bank account decreases).

Positive and Negative correlations determine the Direction of the relationship. But remember, these aren't a true or false sort of thing; a relationship can exist an any level between 0 and +/-1. The closer to +/-1, the stronger the relationship, and the closer to 0, the weaker relationship. A correlation coefficient of 0.5 would show that a positive correlation exists to a medium degree, but the variables are not completely interlinked in their changes.

This visual does a pretty good job of showing what this spectrum can look like:

https://preview.redd.it/ouyj0afjpn571.png?width=797&format=png&auto=webp&s=5e568a93825969e3a8522f34b7c09f6e852a7d66

&#x200B;

Alright, now that we've gotten through most of the wrinkly bits, lets [look at some graphs](https://www.youtube.com/watch?v=sIlNIVXpIns). 

&#x200B;

# Examples and Visualizations

I want to share some examples of where correlations exist, and where they don't. Hopefully this will give you all some points of reference when looking at this kind of information in the future.

We're going to be looking at one of my favorite things in the data visualization space to illustrate this, the scatter plot. Lets look at some examples first of what correlation looks like when we plot the relationship between 2 variables on a scatter plot.

Let's say we want to compare the relationship between the amount of mayo that Kenny has on hand (in gallons) and the number of mayo baths that he can take with that mayo. Loading that data into a spreadsheet and putting it in a scatter plot might look something like this:

![🛁🛁🛁](https://preview.redd.it/kpltucfrpn571.png?width=782&format=png&auto=webp&s=7a23ce3c7a9ce03f5c4697d6b5535d5162838985)

See how the relationship between the number of mayo baths is perfectly linked to the amount of mayo that Kenny has? As the amount of mayo increases, the number of mayo baths increases as well, at a perfect rate. This relationship has a correlation coefficient of +1.

Now lets look at the inverse of that. What happens to the tendies in my bank account as I purchase more bananas?

![🍌🔼🐓🔽](https://preview.redd.it/eu7623bxpn571.png?width=784&format=png&auto=webp&s=444c4cd7c59507e28961e7ea18879dddc814e1a4)

As the number of bananas I purchase increases, the number of tendies in my bank account decreases at a perfect rate. This relationship has a correlation coefficient of -1.

More often than not within the real world, we're not going to see perfect correlations like this. We'll often have some degree of variation in the data, causing the points to not fall perfectly along the line each time. This is when we'll see some degree of relationship within that scale of -1 to +1.

Here's an example of the relationship between the number of DFV tweets in a day and the duration that my tits get jacked:

https://preview.redd.it/c5op48m9qn571.png?width=785&format=png&auto=webp&s=7a25808f7cd5d1ca353631ecb18cb04aa458c727

We can see that it's not a *perfect* relationship, but generally, whenever DFV tweets more frequently, my tits tend to be jacked longer. Something like this would have a correlation coefficient of 0.85.

When two things aren't related to each other at all, we might see something like this plot, where I plotted the number of times I checked the GME ticker each day compared to the number of banana smoothies I drank: 

![🍌🥛](https://preview.redd.it/xvarpz7kqn571.png?width=789&format=png&auto=webp&s=7cceb2fbe043f5506a5fb42f8482ea5d7759f9b1)

Even though I thought that drinking more banana smoothies would cause me to check the ticker more often, we can see that the data shows otherwise. There's no trend within the data emerging, indicating that there's no relationship between the 2 variables, and we can conclude that these two things are not correlated.

Now that we know what this data looks like and how we might see it presented visually, lets talk about how this impacts us in our pursuit for bananas, tendies, and a wrinklier future.

&#x200B;

# Application in our DD

If you were to ask a deep-wrinkled statistician like u/braaaaiiinnnsss \-senpai where you can and can't use correlation, he might hand you a list half a mile long of statistical assumptions, scenarios that break those assumptions, scholarly references and top it all off with a stern look of fatherly concern.

It's ok though apes, he's just trying to make sure we don't analyze things incorrectly, and when we're actually carrying out this kind of analysis, we're doing it the right way, and coming to the right conclusions! We wouldn't want to do this wrong and incorrectly conclude that the frequency of Kenny's mayo baths aren't intrinsically linked to the share price of GME, now would we?

I share all of this information to help you all understand that correlation isn't something that can just be applied to a couple charts that “look kinda similar.” There's *absolutely* some rigor behind carrying out the calculations and making sure that you can prove or disprove a hypothesis using data and analytical techniques before saying that something is correlated, and to what degree.

Making posts saying that 2 things are correlated without providing evidence of the correlation can mislead the audience of the post into thinking that 2 things are inextricably linked to each other in some way. Remember, we learned that correlations can exist at varying strengths and directions. If we want to share information about things being correlated, we can't just point at some graphs that look similar and say. “See! Look at the charts! They have to be correlated!” We have to provide the data to back up the claim that a correlation exists. Jumping to this point without doing the work to actually *test for that correlation* can be a quick path down the slippery slope of spreading misinformation (even if unintentional).

![actual picture of me](https://preview.redd.it/dgjg5hg6rn571.png?width=490&format=png&auto=webp&s=a9c963c0baea268ab0787ebfc7454edb89900463)

This is a great place mention that the Superstonk Quants have a [request system](https://github.com/SuperstonkQuants) that anyone can use  to ask for data, analysis, peer review, or assistance on their own projects. We want to be available to help this community grow in the pursuit of deeper and more numerous wrinkles. 

Now, I want to highlight a few recent posts as examples of what I've seen shared in this sub that I found fault with, for various reasons.

**HOLD ON NOW.** Before you get out your pitchforks for calling these posts out, know that one of the most important aspects of quantitative analysis is peer review and critical discussion of the results. We can't just assume that every DD that gets posted is grounded fully in fact and cannot be incorrect. That's a big pitfall that leads to an overload of confirmation bias. We really need to be careful about both **what** we communicate and **how** we communicate it. I recently saw one of these posts referenced in the [Daily News](https://www.reddit.com/r/Superstonk/comments/nzingy/the_daily_stonk_06142021/) where u/Rensole was using the same “correlation” nomenclature when there wasn't a proven relationship within the post. I use this example to stress how important this is – information can travel *so dang quickly on the internet*.

I'm hoping that the authors of these posts don't take this as an attack on their work, but more a critical review with recommendations for approaches that could be taken next time around. I think all three of these authors are apes of the highest order, and have some fantastically attractive wrinkles.

I'd first like to cover [this post](https://www.reddit.com/r/Superstonk/comments/nzajpv/the_matrix_is_everywhere_a_quant_dd/) by u/BurnieSlander.

* Their post sought to find a correlation within a subset of stocks that had significant, sustained gains through 2021.
* The Good 😁
   * I really liked how they pulled together a pretty sound set of assumptions to create the subset of stocks that were categorized as “gainer-maintainers”; this was a great way to kick off the analysis and subset things down to a more meaningful group other than just *the whole stock market.*
   * The memes were pretty dang good 🤩
* The Not-so-Good 😔
   * One of the most important things that the Quants and I learned over the course of our work with time series data (really any stock ticker data) is that you have to control for autocorrelation. u/braaaaiiinnnsss did an amazing post on this subject [here](https://www.reddit.com/r/Superstonk/comments/nym1ua/an_update_on_relationships_between_stocks/) if you'd like to dive into the details. If you just run a straight correlation on raw price data, you can potentially find correlations where they may not actually exist. This is a false positive, and it can cause the analysis to arrive at an incorrect conclusion.
   * The approach to actually calculating the correlations between the stocks appears to have been carried out incorrectly; this is solely based on our educated guesses about the methodology, as the code & methodology for the work wasn't shared. Unfortunately, when working with stock price data you can't just type corr(x,y) in your code and run with the output. [This KDnuggets post](https://www.kdnuggets.com/2018/06/correlation-coefficient-time-series-angel.html) does a great job of explaining this concept very succinctly.
   * Another problem with this analysis was the correlation matrix constructed at the end. Correlation matrices like this can be useful in certain circumstances, but in this case, they can lead to false positives or skewed results. The problem is that running a massive 75x75 matrix will end up finding correlations between things where they don't actually exist due to multiple comparisons. 

&#x200B;

Next, I'd like to cover [this post](https://www.reddit.com/r/Superstonk/comments/nyqnqh/so_the_reverse_repos_are_definitely_related_to_gme/) by u/jaybaumyo.

* Their post sought to find a correlation between Reverse Repo and GME.
* The Good 😁
   * Pattern recognition - being able to spot the increases in both RRP and GME at common time intervals.
* The Not-so-Good 😔
   * Referring to the relationship between RRP and GME as a correlation without providing quantitative evidence of it.
   * Comparing the graphs side by side is *not sufficient* *enough* analysis to conclude that RRP and GME are correlated. I recently addressed the lack of strong correlation between RRP and GME in my post [here](https://www.reddit.com/r/DDintoGME/comments/nype4f/is_gmes_price_related_to_the_reverse_repo_rate_in/).
      * While yes, the moves in RRP and GME are timed curiously, the data underlying these moves suggest that the two are not as interlinked as many have suggested, particularly from a quantitative perspective.
      * For us to truly come to the conclusion that RRP and GME are **absolutely related to each other**, we'd have to see a more sustained movement in both direction and magnitude between RRP and GME; for the past 18 months, we don't see a strong enough relationship there to make that conclusion.
      * Is it theoretically possible that those transient changes in RRP were due to GME? It's certainly plausible. Are we seeing enough data to support that RRP and GME are moving in relation to one another? At this time, there's not enough evidence to make that conclusion.
      * This doesn't rule out that a correlation could begin to develop over time if RRP and GME continue to move in the same direction with similar magnitude, but we'll have to wait and see what happens, there.

&#x200B;

Finally, I'd like to cover [this post](https://www.reddit.com/r/Superstonk/comments/nz0fsz/i_found_a_correlation_in_why_reverse_repo_rates/) by u/con101smd.

* Their post sought to find a correlation between RRP, GME and Crypt0.
* The Good 😁
   * Piecing together so many dang puzzle pieces! Seriously, this was awesome work. Pulling together the timing of the events and showing where they all aligned was really impressive!
   * The conclusions – I certainly resonate with the findings from this post.
* The Not-so-Good 😔
   * I wanted to specifically use this post as an example of how the majority of the work can be carried out extremely soundly with great results, but we have to really keep terminology in mind when sharing information like this. Saying that a correlation was found between these things is a misnomer – while there are **absolutely** similarities in timing and movement in various factors, we can't call these things *correlated*. We'd need to run a statistical test against the underlying data to truly determine if a correlation actually exists within that data before making that conclusion.
   * Additionally: after discussing with u/con101smd, they're 100% in agreement with the feedback that I've provided on the DD.

&#x200B;

# Closing Thoughts

Gonna get on my data analyst soapbox real quick, pardon me.

&#x200B;

If you take away anything from this post, let it be this: 

***Unfounded assumptions are inherently dangerous within the data space. Proof is everything.*** 

As an analyst by profession, I hear wild assumptions by my business partners about all sorts of things day in and day out by. I regularly ask them to show me the data that backs up their assumptions. More often than not, they shy away from this, comfortable within their own bubble of ignorance and/or confirmation bias. 

I have to approach analysis as skeptically as possible to remove bias from my approach so that my results are reproducible and representative of the reality within the data. Remaining skeptical and non-biased about information can be a really hard thing for humans to do; we're naturally apt at pattern recognition (particularly visual patterns) and we're part of a society that tells us that we have to have a binary opinion on every topic out there. 

Approaching analysis with a critical, open mind and letting the data lead you to the correct conclusions is an extremely challenging thing to master. Even though your preconceived notions may be shattered in your findings, you can learn so much from having your hypotheses proven invalid.

In short – I want this community to ***thrive*** off of well-sourced data, sound conclusions, and clear communication. These things are key to raising all of us up to the next tier on the wrinkle scale.

Finally, I want to give a big shout out to the other Superstonk Quants for their support with this post. You all are truly amazing and working alongside you for the past couple weeks has been one of the most uniquely enjoyable experiences. This group has taught me so much in the short amount of time that we've collaborated together, and I truly think we can make a (statistically) significant difference in this space for good. 🙌

&#x200B;

**APES STRONG TOGETHER. 🦍🐒🦧**  


**BUCKLE UP. 🚀🚀🚀**

&#x200B;

Correlation references if you'd like to learn more:

[https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5079093/](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5079093/)

[https://www.displayr.com/what-is-correlation/](https://www.displayr.com/what-is-correlation/)

[https://www.kdnuggets.com/2018/06/correlation-coefficient-time-series-angel.html](https://www.kdnuggets.com/2018/06/correlation-coefficient-time-series-angel.html)