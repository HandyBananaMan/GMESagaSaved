# Title: Everything I know about the TD TOS "Glitch" Volume
# Author: jsmar18
# Post URL: [https://www.reddit.com/r/Superstonk/comments/o8wjh7/everything_i_know_about_the_td_tos_glitch_volume/](https://www.reddit.com/r/Superstonk/comments/o8wjh7/everything_i_know_about_the_td_tos_glitch_volume/)


So.... The glitch is back, I've personally waged a war against it as I've consolidated my belief that it's actually a glitch. But there are people who are still skeptical, which is totally fine - as we don't have a 100% solid reason for why they occur, just that they do occur.

In light of that, I thought I'd share all I know about the glitch in hope that one of you may pick up on something, or dig further so we can understand the reason why it happens and either put it to bed or at the off chance, discover something cool.

Originally there was a group of us who took a lot of time to figure out WTF it actually is.... and pooled together various screenshots and recordings which I'll share below.

# Video Recording

The link below is a video recording and we've found you can replicate the glitch on any stock by (in this example it's GME and AAPL):

1. Having open TD TOS before after-hours trading which shows normal order book volume (likely skippable)
2. Closing TD TOS app
3. Opening TD TOS app after-hours which then causes the glitch to occur
4. Expanding glitched level II data by pressing the magnifying glass button (essentially zooming in to see lower interval prices in EOB)
5. This moves the "Glitch" from a price of $182.51 (9 bids, 3 ask) to $182.10 (8 bids, 3 ask)
6. This moves the "Glitch" from a volume of 183,971,094 to 183,915,732 - which is a difference of 55,362

![https://imgur.com/a/klTzNal](https://imgur.com/a/klTzNal)

**Original Hypothesis:**

This was all when my previous DD was still very much alive and i was using this "glitch" as some numbers in it, after seeing this i was sold that it was a glitch. My hypothesis for the above was that it was summing the volume between the upper and lower bound price i.e. in the scenario above as it's in $5 intervals between $177.11 and $187.09 to get such an insanely high volume of 183m.

I don't have the analysis on hand sadly, but the hypothesis did not check out, volume traded at that range was nowhere near 183m mark.

I paid $80 for 1m Interval GME data, so if you wanna take a crack at it, PM me, and I'll pass the data on (shhh, don't tell the provider 😉)

I still have an inkling that previous trading volume has something to do with it, if it's order book volume, then well, if you got a data source, hit me up.

# Screenshot Dump #1

This batch of screenshots we had three people check out TD TOS EOB.

**User #1**

This user opened up TD TOS after hours, 4:37pm.

https://preview.redd.it/52j5duy9ys771.png?width=1162&format=png&auto=webp&s=1ea0a1d5db4d2d4fe55ff050a512678f1e60425f

**User #2**

This user had TD TOS **open when after-hours hit,** the screenshot was taken 4:41pm

https://preview.redd.it/s81tqkkfys771.png?width=1442&format=png&auto=webp&s=7e82fb00616801d78b6f752656ca2aa4fc2cad6b

**User #3**

User opened TD TOS after hours at 4:34pm.

https://preview.redd.it/920p9dxnys771.png?width=1176&format=png&auto=webp&s=cba6b9642bbece32bf4f872341953f203eca5535

This was to see if it happened with multiple users in terms of opening it after hours for reproducibility, it worked! We also kept one person in TD TOS when after-hours hit to see if they noticed the glitch, which they did not (user #2).

Note how User #1 and #3 have different volumes as the price moves, this is the same thing we saw in the video.

&#x200B;

# Screenshot Dump #2

The next dump is looking at the TD TOS Glitch volumes over a period of time.

**4:53 pm**

This is the screenshot before the TD TOS app is closed, normal volume after-hours as noted in the video as well.

https://preview.redd.it/ikcvr1qazs771.png?width=1441&format=png&auto=webp&s=8af0c05e329f3b71e4a36f390c9c9644bb633b0e

**6:11 pm**

https://preview.redd.it/omuec99ezs771.png?width=1406&format=png&auto=webp&s=c3307d25fcff614cfa02a464afcde2c309a4ecb6

**7:00 pm**

https://preview.redd.it/li6ej2wfzs771.png?width=1408&format=png&auto=webp&s=492b547e1926cec1517a19b36e847ced48974b99

**7:53 pm**

https://preview.redd.it/i2kml7wjzs771.png?width=1402&format=png&auto=webp&s=7206dd3245b3eb371394324fe5a385692e0b15f2

For those that don't want to squint, for GME the volume, prices are below.

24,950,943 | $181.30

24,950,943 | $181.30

24,950,943 | $181.30

24,950,943 | $181.30

These are all the same across different time periods at the same price, so we can observe that it is static on day end in after hours. A further experiment that just came to mind is to look at it one day, then the next day, replicate the glitch and scroll back to see if it has been wiped.

The last point to note is that it can seemingly be replicated with any stock, only tested 4 here but pls go ahead and try a basket of however many!

&#x200B;

# Contacting TD TOS Tech Team

The last thing we did was to contact the tech team to see what they thought. I did not record it, as someone else was doing it - so you'll just have to take me on my word......

\---------------------------------

They said their technical team is aware of "the bug" in the total volume count in Active Trader; it previously occurred with futures contracts and they're aware that it's currently happening with some stocks and asked for the following:

1. Take screenshots throughout the day **(they are not concerned with after-hours)**
2. Send screenshots to [support@thinkorswim.com](mailto:support@thinkorswim.com) with the title "Active Trader Bug - Excessive Total Volume Binned Data"

\---------------------------------

So the thing that stuck out to me here is that they don't care about the after-hours volume and only market hour volume. Don't know why, but I'd put my money on market open volume showing a huge spike like that causing traders to freak the fuck out and sell/buy. Feel free to dig further on that point specifically, re why they don't care about after-hours.

This indicates to me, there's no plan to fix it unless it starts to happen during market hours...

u/Criand since you did some DD using this.

u/happy_dick_punch, same reason as above.

Edit: Clarifying that this can be replicated on **any day after hours,** which is why I did not bother with dates and only timestamps. 