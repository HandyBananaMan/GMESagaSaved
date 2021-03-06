# Title: DD: Why retail is holding far more shares than you'd think
# Author: thedav1d
# Post URL: [https://www.reddit.com/r/GME/comments/mduj5t/dd_why_retail_is_holding_far_more_shares_than/](https://www.reddit.com/r/GME/comments/mduj5t/dd_why_retail_is_holding_far_more_shares_than/)


*Disclaimer: I am in no way an expert or a financial advisor, this is not financial advice, this is only my understanding of the current situation based on what I have read. I entered the stock market about 8 months ago, so please correct me in the comments if I'm wrong, and I'll edit the post.*

**TL;DR: Retail investors not only hold more long positions that the entire number of shares outstanding, but also control a bunch of shares through deep ITM call options. Therefore, long whales selling during the squeeze would only cause a dip and would not be enough to end the squeeze. In addition, a lot of long whales will not or cannot sell during the squeeze in my opinion, more details below. Conclusion: $2,000,000/share is definitely possible.**

&#x200B;

# A) Estimation of retail long positions

As far as I'm aware, there isn't any data that can provide an exact number of shares held by retail investors, so I'll have to estimate that number.

First, let's look at the most obvious indicator: the r/wallstreetbets [subreddit growth](https://subredditstats.com/r/wallstreetbets) during the fake squeeze in January.

https://preview.redd.it/pmqiwcitzep61.png?width=775&format=png&auto=webp&s=e21adb54879104daa80d6684cfa3602a86bce6b6

On the 23rd of January, the number of wsb subscribers was right around 2 million. It then skyrocketed and reached 9 million by the middle of February, so it's safe to say that the 7 million new users are at the very least interested in $GME. Now, let's assume that each new user holds *on average* 10 shares.(keep in mind that a whole lot of users own hundreds, if not thousands of shares, and DFV owns 100,000 shares by himself, so I think my estimation is quite conservative)

**That would mean that wsb users alone own 70 million shares.**

**That's over 100% of shares outstanding and 155% of float.** [Outstanding vs Float](https://www.investopedia.com/ask/answers/062315/what-difference-between-shares-outstanding-and-floating-stock.asp)

Please note that this number does not even include all other retail investors, nor Reddit users on other subreddits such as r/GME and r/Wallstreetbetsnew, nor wsb investors who have not created a Reddit account/subscribed to wsb. So the actual retail ownership might actually be a LOT more than that.

*Also note that a good portion of the float is locked away in ETFs and mutual funds that rebalance quarterly or even yearly.*

&#x200B;

# B) Shares held through options

You may have herd the term **delta hedging** thrown around quite a few times around here. [In case you've never heard of delta hedging](https://www.investopedia.com/terms/d/deltahedging.asp)

Basically, the market makers who sell options contracts have algorithms that will keep them delta neutral, which keeps their risks low. Now, as a call option goes deeper and deeper in-the-money (ITM), its delta becomes closer and closer to 1. Since options are leveraged at 100x, this gives a delta of 100 for each deep ITM call options.

For example, let's say a market maker (MM) **sold** one deep ITM call option. Because they are short the option, their current delta would be -100.

**How do they stay delta neutral?**     2 ways:

1. First way would be to **sell a deep ITM put option**, which is the exact opposite of what they just did, which brings their delta to 0, since deep ITM put options have a delta of -100. Because they are short the option, the delta of this transaction is +100, which brings their total to 0, AKA delta neutral.
2. Second way is to **buy the underlying stock**. The delta of one share of the stock is +1, so that means that the MM would have to buy **100 shares** (delta of +100) to stay delta neutral.

Now that we've gone over the basics, let's see what happens when $GME squeezes. When the price of GameStop shares reach 1k, 10k, 100k, 1mil, etc. every single call option currently held by retail investors will be deep in-the-money. That means that the market makers who sold these contracts would have an extremely negative delta.

**But here's where it gets interesting: the MM can't use the first way of delta hedging, with the put options they sold, because all of their short puts would be far OUT-the-money, which means that all those contracts would have a delta close to 0.**

**THE ONLY WAY THEY CAN BE DELTA NEUTRAL IS THE WAY NUMBER 2: BUYING 100 SHARES PER CALL OPTION.**

*That means that a good chunk of institutional ownership is* ***actually held by retail investors***\*, because as long as retail holds onto their call options, the market maker is going to hold onto the shares needed to keep a delta of 0.\*

For example, DFV, by holding on to his 500 deep ITM call options, would actually control 50,000 shares of $GME. That brings his total to 150,000 shares held under his diamond hands.

Currently, [call open interest](https://marketchameleon.com/Overview/GME/OptionSummary/) on GameStop is 390k (as of 10 AM EST), so hypothetically, if $GME reaches 1k right now, the MM would have to buy and hold 39 million extra shares for as long as the call options holders want.

&#x200B;

# C) Short selling

Now, let's see how short selling works and how it affects the number of long positions. Imagine this:

* A company with the ticker $EMG issues 100 shares and sells them on the market. Float (which in this case is the same as outstanding because there are no insiders) is therefore 100 shares. This number does **not** change.
* Buyer ***Long1*** buys these 100 shares and stores them with his broker. That means that the total number of long positions is 100.
* Now, shorter ***Short1*** borrows these shares from the broker and sells them on the market
* Buyer ***Long2*** buys these 100 shares and stores them with his broker. Now, the total number of long positions is 200, or twice the float, whereas the number of short positions is 100.
* Short interest is therefore 100% (100 short positions divided by float of 100 shares)
* Now, shorter ***Short2*** borrows the 100 shares from ***Long2***'s broker and sells them on the market.
* Buyer ***Long3*** buys theses shares.
* Total number of long positions is now **300**, which equals **300%** of float
* Short interest is now **200%** of float.

https://preview.redd.it/kegamv6wzep61.png?width=1041&format=png&auto=webp&s=4ea34085ecbd2a9168d7fbfe7961e87f03839509

We can see that short selling **artificially dilutes the shares by increasing the number of long positions.** ^((take this with a grain of salt, this is all my own understanding of the market, please correct me if I'm wrong))

*What does this mean?*

It means that if the shorts want to cover (or ***have to***), they'll have to buy back 200 shares to return to the brokers.

But remember, there are now 300 longs out there that they can buy back from.

I wanted to clear that up, since I've seen a misconception going around quite a lot saying that,

>the shorts have to buy your shares multiple times over

This is **misleading**, because shorts don't necessarily need *your* shares. Sure, they need more shares than were ever issued by the company itself, but the shorting process itself creates artificial shares.

Back to our example, after shorts cover (by buying 200 of the 300 longs out there and returning them to the brokers), there will only be 100 shares left, which is exactly where we started.

HOWEVER, since they need to buy back a very large number of shares, the supply won't be able to keep up with the demand, so the price will shoot up until they can find longs willing to sell their shares. Let's say that ***Long1*** decides to sell his 100 shares. The price will stop going up, and might even dip slightly, since supply just increased. But once the order is filled, the shorts still need 100 shares more, so the price will keep going up until either ***Long2*** or ***Long3*** are willing to sell.

![Long whales selling would only be a dip during the squeeze](https://preview.redd.it/3phegvwyzep61.png?width=1225&format=png&auto=webp&s=eb5c4c567d24db8ac0699a699b27fd2f9071f7d9)

1. ***Short1*** need to cover their 100 shares short, so they put in buy orders, supply cannot keep up, price goes up.
2. ***Long1*** sells their 100 shares, the buy orders get filled, price stalls.
3. Because of the price increase, ***Short2*** gets margin called and need to buy back 100 shares. Price goes up again.
4. At some point, ***Long2*** decides that the price is good enough, so they sell their 100 shares. Supply meets demand, price stops going up.
5. Return to equilibrium. ***Long3*** still hold their shares.

We can see that once the shorts all cover, the number of long positions will be equal to the number of shares that the company issued once again. This means that of the 300 long positions in total, the 200 first longs who are willing to sell will be able to sell at the price they set, and the remaining 100 longs will hold through the squeeze and not profit from it.

**The squeeze only ends once the total number of long positions is equal to the number of outstanding shares.**

So why do I bring this up? Remember how we estimated that retail held far more shares than were ever issued, either through long positions or through deep ITM options? Yeah, that means that *even if* every single long institution and insider sold 100% of their shares, retail would *still* have the power to decide the peak price of the squeeze, because shorts NEED the shares that retail hold. If retail wants to start selling only at $2,000,000/share, the price will get there **no matter what**. Whales selling would only be a dip, then once their order is completely filled and the supply dries up again, the price will shoot back up until they can find the next seller.

And that brings me to the next section: why long whales will not sell during the squeeze.

&#x200B;

# D) Who will hold through the squeeze?

So, we learned from the example that, at the end of the squeeze, the total number of long positions will be back to the initial number of shares issued by the company. For $GME, that means that there will be 70 million long positions left after the shorts cover every single short position they had.

We also know that [institutional holdings](https://finance.yahoo.com/quote/GME/holders?p=GME) exceed the total number of shares outstanding. We don't know the exact number, since the date of reporting differs for each institution, but it's safe to assume that the real number is close to 120% of shares outstanding.

https://preview.redd.it/p9tasb910fp61.png?width=905&format=png&auto=webp&s=372ccb47278dcd0ccc4a6f3de6b897f1807b31c2

Who will not sell during the squeeze? (note that this is only my educated guess, we have no way of knowing for sure)

**Exhibit A: Insiders**

According to the [short-swing profit rule](https://www.sec.gov/Archives/edgar/data/704384/000119312504051976/dex995.htm) (here's an [explanation by investopedia](https://www.investopedia.com/terms/s/shortswingprofitrule.asp)), insiders cannot make a buy and a sell transaction within 6 months of each other. This means that they can't just sell all their shares during the squeeze and buy them back a week later. If they do sell, they'll have to wait another 6 months to buy them back.

Now, I'll admit, I don't know much about insider trading and the stock market in general, but I feel like it wouldn't be advantageous for board members to reduce their voting power during the digital revolution of their company. [Yahoo](https://finance.yahoo.com/quote/GME/holders?p=GME) says that over 27% of shares outstanding are held by insiders, which is about 19 million shares.

https://preview.redd.it/qjjwgr630fp61.png?width=399&format=png&auto=webp&s=5dd1869e596fbfaa47c1afd0cf8b6ea8578cab19

**Exhibit B: Papa Cohen, BlackRock and Vanguard**

First of all, since RC owns more than 10% of the company's shares, he is considered an insider by the SEC's definition. That means that he also is not allowed to buy and sell shares within 6 months. Therefore, I think it's safe to say that RC's 9 million shares will be held through the squeeze. Otherwise, RC would lose his voting power to kick out the dead weight on GameStop's board of directors for 6 months.

In addition, as explained by [this DD](https://www.reddit.com/r/GME/comments/md89wg/king_kong_magnum_opus_dd_posted_on_behalf_of_wuz/), BlackRock and Vanguard, which are two of the biggest institutional longs of $GME, are probably helping RC get the votes he needs to kick out the useless board members that slow down GameStop's digital revolution. So these shares would also be locked away during the squeeze.

That gives us 9 million shares from RC, 9 million more from BlackRock, and 5 million from Vanguard, which totals over 23 million shares held by these three Long Moby Dicks.

**Exhibit C: ETFs and mutual funds**

As noted previously, mutual funds and ETFs usually rebalance quarterly, which means that they will likely miss out on the squeeze, since the MOASS is expected to last less than a month. That means that however many shares they have will be locked away, and can't be bought by shorts trying to cover.

https://preview.redd.it/6lis6xd50fp61.png?width=906&format=png&auto=webp&s=c6122f02dc5aed4df2c459bda931acac024cd1fe

According to [Yahoo finance](https://finance.yahoo.com/quote/GME/holders?p=GME) again, the top 10 mutual funds hold more than 17% of shares outstanding, or over 12 million shares.

There are likely millions more from all the other ETFs and mutual funds that didn't make the top 10.

&#x200B;

**So in total, it would mean that at least 54 million of the 70 million outstanding shares are actually locked away and will not be sold during the squeeze.**

*Side note: it might look like I counted RC's 9 million shares twice, since I said he was an insider by the SEC's standard, however when looking at the* [*insider transaction history*](https://finance.yahoo.com/quote/GME/insider-transactions?p=GME)*, we can see that RC's 9-million-share purchase is not listed, therefore he isn't part of the % held by insiders.*

&#x200B;

**This means that every ape will likely be able to get the price they want for their shares.**

&#x200B;

# E) GameStop will not issue more shares

Another thing I'd like to address is the fear that GameStop might raise money by issuing millions more shares and saving the shorts in the process.

*But here's why GameStop won't bail out the hedgies.*

Firstly, during the earnings call, we found out that GameStop actually has plenty of cash to spare and that their earnings were better than expected. Plus, they've gotten a shit ton of free publicity from the January fake squeeze, which means that they're probably making more money than ever before.

Secondly, just think about it. Why would GameStop save the shorts who tried to bankrupt them with illegal naked shorting and maybe even more shady shit I'm not aware of? Why would GameStop issue shares at 1k or 10k when they know they could raise funds at 500k if they need the money? Why would GameStop stop a short squeeze that would benefit millions of retail investors?

GameStop's customers are Redditors. GameStop's customers are retail investors. They're not hedge funds. They're not market makers. They're not any other institution.

If they dilute their shares and help the shorts, they would only shoot themselves in the foot. They would face immense backlash, similar to Robinhood. They would lose the faith of millions of individuals/potential customers. They would NEVER recover from such a nearsighted action, and Ryan Cohen, as the (possibly) new CEO, will never let that happen.

Plus, at this point, since the real short interest is likely to be anywhere from 200% to 900%, they'd have to issue tens, if not hundreds of millions of extra shares in order to save the hedgies. There's simply no way they'd be able to pull that off.

&#x200B;

# F) Sit back and relax

Being long on $GME is literally the easiest thing you could do. You just need to hold! Holding long positions costs nothing and we now know that GameStop is not going bankrupt any time soon. So long positions can literally be held for an infinite amount of time, whereas the shorts pay interest for each short position they have. They can't hold forever. In fact, they probably can't hold much longer at all, in my opinion, considering how many short positions they might have and considering the new DTCC rules that may come into effect soon.

As always, be nice to each other, if you're getting too stressed, turn off your monitor and go do something else.

This is my first attempt at an actual DD, so if there's anything wrong, please let me know. Updoot for visibility :)

&#x200B;

TL;DR at the top.

Edit 1: ??????????????????????????????????????????????????????????? ook ook