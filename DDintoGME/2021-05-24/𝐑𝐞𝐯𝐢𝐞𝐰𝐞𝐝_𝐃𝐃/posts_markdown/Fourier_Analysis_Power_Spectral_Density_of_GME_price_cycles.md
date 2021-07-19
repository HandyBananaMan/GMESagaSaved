#Title: Fourier Analysis: Power Spectral Density of GME price cycles
#Author: positive_root
#Post URL: [https://www.reddit.com/r/DDintoGME/comments/njt2q9/fourier_analysis_power_spectral_density_of_gme/](https://www.reddit.com/r/DDintoGME/comments/njt2q9/fourier_analysis_power_spectral_density_of_gme/)


Hey everybody, I've been lurking for a while, thought I might have something to contribute to the hivemind. I'm submitting this late at night California time cause it took me a while, it turned out to be very long. Anyway, good morning Euro friends! Can't wait to visit you all again someday!

So I've seen a lot of speculation on FTD cycles of 20-something days, 30-something days, etc, plenty of people wonder if there's really something wonky with GME's price, it sure looks like there are some cycles there, but is there anyway to measure that in a quantitative way? Yes, it's called Fourier Analysis, also known as looking at a plot of power spectral density.

I've heard some people use this phrase "technical analysis" of price movements, which I believe is called that because it is only just technically a form of analysis? Haha, ok but I seriously don't know why they call it that. I know I'm not the only science-type here, I have a background that does not involve finance but does involve using statistics and I will attempt to perform a statistical analysis. There will be some hand-waving by the end, and in that sense, this may remind you of a so-called technical analysis.

Here's a meme to explain some of the deep secrets of statistical analysis:

&#x200B;

![Stats](https://preview.redd.it/ei0uzlf751171.jpg?width=590&format=pjpg&auto=webp&s=c4bf87786cf8a90809253558712ff5c39da29deb)

Ok so the first question here is how to slice and dice our data. A Fourier analysis requires an unbroken series of consecutive samples of the signal for which you wish to know the power associated with any variable cycles in that signal. That is, if you want to know how much amplitude power is associated with price movements on a 30-day time-scale, you would need an unbroken series of prices many times longer than 30 days. This is because if you only had a random stretch of 60 days, for example, you would only be likely to catch one 30 day-cycle in the middle. If you had data for a consecutive stretch of 120 trading days, you could see 3, maybe 4 cycles with 30-day periods depending on when the cycle starts.

&#x200B;

So one thing to watch out for is the maximum length of a period under consideration in a Fourier analysis, and only trust power reported for cycles 2 to 4 times shorter than that stretch. So that said, we've got several long time periods of interest to choose from. For this analysis, I choose 3 main periods: The before times of 2016-2019, The Short Period when prices were very low in Q3,Q4 2019 - Q1,Q2 of 2020, and The Ape Days which are obviously the recent times in 2021, but appear to really begin in August 2020, so I will subset Aug - Dec 2020 as The Ape Days of 2020 to see if anything special was going on in the price movements during that time before the coverage became significant:

https://preview.redd.it/9hu5l3rdn0171.jpg?width=1857&format=pjpg&auto=webp&s=611f819b995f2aca97f1e68a738e91a0d7a3d5ba

I have tried slightly changing the boundaries of these time-frames, especially the boundaries around "The Short Period", and it does not have a significant effect on these results. We need to have a signal that is regularly sampled for Fourier Analysis, and I currently only have access to Open and Close price data. To get a uniformly spaced signal, I'm going to pretend the Open price for each trading day occurred at 6am and the Close price occurred at 6 pm, and those are my samples, 2 per day, equally spaced. If anyone has access to long stretches of hourly data they are willing to share, I would perform this analysis on it with interest. I interpolate across weekends to complete long stretches of consecutive calendar days. I am worried about how the interpolation over weekends may affect the conclusions, so I will focus on periods of consecutive trading days, but know that I've considered it. Look how the interpolation is a little wonky over the weekends depending on interpolation choice:

&#x200B;

https://preview.redd.it/7k485qupt0171.jpg?width=1750&format=pjpg&auto=webp&s=dd8d2c6d09c75dce18d01e1a2e609e54806f341c

Now, a short primer on how to interpret the types of figures I'm about to show you. Prepare yourself, they look messy. They are best to view by kind of blurring your eyes and looking only briefly, you are not supposed to read too much into any of the many peaks, unless they look like a local maximum. We could come up with a series of ad-hoc criteria to determine local maxima and call it objective, but this is somewhat subjective. Here's the first one, no pressure, just get a feel for how it looks:

&#x200B;

![Cool cool cool, spectrally flat](https://preview.redd.it/wafp2qfyp0171.jpg?width=2813&format=pjpg&auto=webp&s=76863332efe1bf675d480de88d075e9d6efdbc42)

What we see for the Before Times and the Short Period is a "spectrally flat" slope, consistent with statistical noise. There is no particular cycle with a peak that stands above the crowd, if you will. The power spectral densities (PSDs) plotted in blue and green above seem like they have a lot of noise for periods of a few days, and then become big loopy waves out at the long time scales of 100-day periods and beyond. The messiest part is over-sampled, but those long cycles are significant fractions of the total signal length, and power associated with a potential cycle at those long ranges can "alias" themselves out (under-sampled). So don't read too much into the far right side, but do consider the left side and the middle. We discussed this before when thinking about looking for a 30-day pattern with only a 60 day stretch, but here we have 400 and 800 day stretches of days. Note that 10\^0 = 1 day. I note this looks to me like [pink noise](https://en.wikipedia.org/wiki/Pink_noise), I have no idea what to make of that but it's very interesting.

The y-axis shows the power per cycle associated with any cycle, and the x-axis shows the period of that cycle. The fact that the units on the y-axis are decibels per cycle per day is supposed to clue you in that dB is a type of log-scale. The x-axis is log scale too. What we see for both the Before Times and the Short Period is a generally constant slope of higher power at longer and longer timescales. Note that this doesn't tell us anything about the trend of price, whether generally up or down, Fourier analysis does not care about that. It only tells us the power associated with cycles of variable periods unrelated to background rising or falling trends. Before August 2020 there were no predictable cycles.

&#x200B;

Now, the result you've been waiting for, here are the PSDs for the Ape Days, and the 2020 only subset, and a normal 200-day period, without annotations:

&#x200B;

![T+2 days is wack](https://preview.redd.it/3co2m0imu0171.jpg?width=2813&format=pjpg&auto=webp&s=76a3239f8fdc0e6c1073738b7767eb4048ce9718)

Here are some annotations to guide your eye and go with the following discussion:

&#x200B;

![My discrete transform is tingling](https://preview.redd.it/qe0ju7j0v0171.jpg?width=1623&format=pjpg&auto=webp&s=8055e15d7e92ec611a931326ff5a46d7339dc872)

In the above figure, I color as orange the PSD of price movements during the most recent 200 trading days (Ape Days). In blue, I plot the PSD associated with 200 trading days during the Before Times, as a comparison to show what a normal 200-day period would look like. This helps us be sure that the Ape Days are indeed unusual. In black, I plot a shorter period of the 115 Ape Days of 2020 only.

While there are particular peaks at 24 trading days, and 35 trading days, it is difficult to be sure these peaks are really local maxima. Could be, say, 21 and 33, I mean, but not 20 and 40. In the shorter Ape Days of 2020 only period, it seems like the 30-day cycle is gone, and the 24 day cycle was longer at 26 days... this may be due to the shorter sampling period of only 115 days.

The peaks at 6, 7, 10, and 15 trading days are only slight local maxima. I imagine some of the power over these time periods is due to options activities, could be people closing out their weeklies or monthlies a various few days or weeks early. The peak around 4.15 days is curiously well resolved, I tried a lot of slicing and dicing and it kept showing up as 4.13, 4.16, but never just 4 days. I note that 4.17 ish days is exactly 100 hours. Could there be some fundamental finance cycle on that time scale... maybe it's algos? I need to find hourly data to have more insight.

But the number one thing I was surprised to see with this analysis is the wonky way the power seems shifted around the 2-day time period. It's almost as if price movements on shorter time-scales have been somehow damped.

This Fourier analysis indicates that, given a certain price movement in GME (up or down), there is much less price movement before 2 days have passed, and much more price movement after 2 days have passed, in these modern Ape Times, as compared to previous years.

&#x200B;

TL;DR: The appearance of a strong FTD cycle at both 20-something and 30-something trading days over the past year is supported by Fourier analysis. The analysis also showed a curious shift in price amplitude power from less than 2-days to longer than 2-days. Something's wonky with the T+2 cycle.

Edit: Just wanted to add a link because I was thinking of a slightly different interpretation of what I've done here, I basically turned GME's price into a sound, and during the before times, it was all [pink noise](https://en.wikipedia.org/wiki/Pink_noise)... and then sometime around the end of 2020, it starts to beat, at a rate curiously similar to the FTD cycle...