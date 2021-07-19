#Title: Benford’s Law test shows high likelihood of fraudulent manipulation of GameStop prices
#Author: animasoul
#Post URL: [https://www.reddit.com/r/Superstonk/comments/nnvmtj/benfords_law_test_shows_high_likelihood_of/](https://www.reddit.com/r/Superstonk/comments/nnvmtj/benfords_law_test_shows_high_likelihood_of/)


**Update:** Following responses to criticism and kind advice, this version - except for the **Counter to the Counter DD** \- is now invalid and replaced by the **"Jumbo Compilation"** over at DDintoGME subreddit.

"Counter to Counter DD" still stands - it is not part of the original post. It shows that at least at the theoretical level, there is no reason why BL can't be applied to stock prices and no literature was found - so far - which shows that BL does not apply to stock prices.

Critics have raised other questions beyond the theoretical level which I never intended to address when I wrote this first post. I am not a data scientist. It was never my intention to offend data scientists or to challenge data science. Any expert and valid criticisms must be answered if the basis established in the "Jumbo" post is extended to the highest level of rigour, worthy of publication in an academic journal.

Someone assumed I am a "professional researcher". I am not. In that non-professional capacity, I tried my best to respond to the criticism. I learned a lot which I never would have on my own if I hadn't published the post.

From the standpoint of a hobby, non-professional project, I think it is cool that Fiskars conforms. I don't have lots of time for this but have since found two other conforming stocks quite easily. I may or may not continue this hobby project in private. I personally think it is solid "DD" on that basis and on par with other "DD" which tackle questions about securities law or the functioning of the capital markets on a non-professional basis. But maybe this particular DD/non-DD is different and the implications are too serious. That's also fine. I leave it to the mods, sorry for making a job for you!

&#x200B;

**Start of original post**

For a while now, apes have been saying that the prices of GME look very sus, e.g. closing at perfectly round numbers and weird movements intraday. So I wondered what the Benford’s Law test would show if applied to the daily closing prices of GameStop. These days, Benford’s Law is most often used in forensic accounting, e.g. it is used by the IRS to investigate tax fraud and is used a ton by academics to investigate collusion and financial crime in asset prices, fund returns, the LIBOR manipulation, etc. It is not hard evidence of fraud but if a set of numbers deviates significantly from Benford’s Law that is a serious Red Flag 🚩. So in that sense it is a good screening test and widely accepted as reliable if used on appropriate data.

# What is Benford’s Law?

Basically, according to Benford’s Law, naturally occurring sets of numbers (e.g. country populations) are not randomly distributed. You might expect them to be, in which case each number from 1 to 0 would have an equal chance of appearing as the leading digit in a number. But it’s not the case. When such sets of numbers are unmanipulated, they stick to a quite strict distribution. The unit of measurement also doesn’t matter (proven by Roger Pinkham in 1961), whether dollars, centimetres, quantity of leaves on trees, or whatever. This is Benford’s Law. It will not work for made up numbers or randomly generated numbers, say by a computer. But it will always apply to naturally occurring sets as long as it is not something very restricted like, say, people’s heights, because the leading digits in people’s heights don’t range across all the numbers from 1-9. So you do have to use your common sense when you apply it.

People found out in the 1970s that you can use it to detect fraud in socioeconomic data and in the 1990s Mark Nigrini, a chartered accountant, proved in his thesis that accounting data conforms to Benford’s law. It is now a standard tool of forensic accountants.

If you’re wondering why numbers don’t appear randomly, it is basically because the probability of 1 appearing as the leading digit goes down as numbers go up, e.g. through the 20s, 30s, etc. until you get to 100. And then it starts again as you go through the 100s, 200s, etc. There is a good and fun video explaining this from Numberphile on YouTube.

&#x200B;

![Go to YT - no links](https://preview.redd.it/a0b1ym9f94271.png?width=822&format=png&auto=webp&s=20095aec0e0f2d97ad23ad53e0e2845b0d6951e6)

Here’s a table of the distribution for reference. I’m just going to look at the **first digit** distribution in this post.

![Benford's Law frequency table](https://preview.redd.it/zk6nzvmj94271.png?width=467&format=png&auto=webp&s=e6c22e10759d620e3d9cf53090db6cb49a978eeb)

# Benford’s Law and some famous Ponzi schemes and fraud

Here’s an example of normal and manipulated hedge fund data. You can see that the **Global Barclay Hedge Funds** index, which is an index of HF performance, is pretty close to Benford’s distribution. But **Bernie Madoff’s Fairfield fund** is off.

&#x200B;

![Source: Frunza \(2016\), Introduction to the Theories and Varieties of Modern Crime in Financial Markets](https://preview.redd.it/wx6ah28u94271.png?width=414&format=png&auto=webp&s=c5b1104004ee86b6c5c1aa79984fd40fb3d0cff7)

Here’s another comparison – this time one is a normal bank and one is a failed bank suspected of fraud.

&#x200B;

![Source: John P. O’Keefe et al. \(2017\) Offsite Detection of Insider Abuse and Bank Fraud among U.S. Failed Banks 1989-2015, Federal Deposit Insurance Corporation](https://preview.redd.it/pn9h8as7a4271.png?width=692&format=png&auto=webp&s=2f65c600cee22446bdacfc17247d689847f5f547)

&#x200B;

![Source: John P. O’Keefe et al. \(2017\) Offsite Detection of Insider Abuse and Bank Fraud among U.S. Failed Banks 1989-2015, Federal Deposit Insurance Corporation](https://preview.redd.it/a6oh0m79a4271.png?width=691&format=png&auto=webp&s=f0b06db340124ecbf40b62d3b528958b2a5da47d)

&#x200B;

For kicks, here's **Enron** too.

&#x200B;

![Source: towardsdatascience DOT com](https://preview.redd.it/c854xtpxa4271.png?width=708&format=png&auto=webp&s=2e9babcf4232a5d242afb8a337942c1eb843bd0d)

# Here are the GameStop charts

OK but what about **GameStop** right? That’s what we want to know!

I pulled the historical daily closing prices of GME from Yahoo Finance and generated three charts. A BL chart for the entire set of historical prices starting from 2002; a chart for the past 5 years – to cover the specific period of the sus directors who have now resigned and the period of short selling/the narrative of GameStop’s demise; and a chart from 2020-2021, to cover what we all suspect is the period of highest f\*ckery in the GME share price. The range of numbers is wide and good for all three charts. Even the 2020-2021 chart ranges from prices around 3 or 4 dollars right up to the top of the aborted squeeze in January 2021.

&#x200B;

![Max historical data](https://preview.redd.it/6kgcbzn8b4271.png?width=3372&format=png&auto=webp&s=a1594d672dc1e2331f6d7302f7b2922cf925fe51)

&#x200B;

![5 years](https://preview.redd.it/4j756b3bb4271.png?width=3349&format=png&auto=webp&s=7efe121a05fa6219bceb93aa27e260dede5a98b2)

&#x200B;

![15 months](https://preview.redd.it/gr4qek0db4271.png?width=3671&format=png&auto=webp&s=95ac44a262c25e4eace7daf216c64fc17e00e6c2)

I can’t be bothered to share my Excel file right now but here is a screenshot and if doubting apes really want the file with all the numbers and to look at the formulas, let me know and I can do this.

&#x200B;

![Raw data in Excel](https://preview.redd.it/fmwsxznib4271.png?width=991&format=png&auto=webp&s=2c1f1844dd39078d62c752992aabf9b876043d28)

# TLDR

Generally you can see that even when we take the entire data set going back to 2002, the GME share price is pretty off. The distorted pattern in the 5-year chart becomes even more exaggerated in the 2020-2021 chart. When you compare to **Madoff** or **Enron** for example, **GME looks much worse**.

# Playing with Benford’s Law by yourself

If you want to play with BL by yourself, google **"How to use Excel to validate a dataset according to Benford’s Law"**. It is pretty easy, so give it a go!

And this is a good and simple background reference which I used for this post - google: ©2011 **THE IMPACT AND REALITY OF FRAUD AUDITING BENFORD’S LAW: WHY AND HOW TO USE IT** by GOGI OVERHOFF, CFE, CPA Investigative CPA California Board of Accountancy Sacramento, CA

I am not a quant, far from it, so if anyone more experienced wants to counter or dispute, please feel free! Because I am currently writing an MSc dissertation about hedge fund fraud, I needed to read about fraud detection methods for my literature review, which is how I found out about Benford’s Law, but my dissertation is more about public policy implications, it’s not quantitative.

**Disclosure:** I bought the Friday dip! 🚀  🚀  🚀

Love from u/animasoul 29 May 2021, 21:25 BST

# EDIT 29 May 2021 22:44 BST

I am adding this because it is coming up in comments - i.e. it is disputed that Benford's Law can be applied to closing stock prices. This was my response to u/brickhouse1013:  *Well generally in academia you will always find people who position  themselves on both sides of an argument. For example, I googled quickly  just now and near the top of the search list one paper says this: “In  general, in a given financial market, the probability distribution of  the first significant digit of the prices/returns of the assets listed  therein follows Benford’s law, but does not necessarily follow this  distribution in case of anomalous events.” But another paper says this:  “Application of Benford's Law in the field of financial analysis is very  rarely covered. ... Stock turnover data conforms to Benford's Law,  while daily closing stock prices do not. Probably, psychological factors  significantly influence daily closing stock prices, so these values do  not conform to Benford's distribution.”* ***Science can’t tell you the truth of anything, it can only persuade you either way or make you  investigate more.*** *But definitely it would be interesting to do more  charts for other stocks to compare.*

# EDIT 29 MAY 2021 23:09 BST

OK in response to comments here is a quick and dirty chart of **Google** all time closing prices. It's not perfect but generally follows the shape better than GME, especially the more recent charts. It even starts and ends perfectly. Intuitively, you would expect that it is harder to manipulate Google over its entire lifetime, although I wouldn't exclude manipulation in any stock when you take into account the context that manipulation of financial markets is probably the norm rather than the exception:

![Google blue\/Benford orange - couldn't be bothered to make it the same as my other prettier charts](https://preview.redd.it/jjt3ogu7v4271.png?width=1653&format=png&auto=webp&s=17c88133990305bddc6b96c01988f7769a03f1f3)

# Last edit?

Based on the comments I just want to also point out that **what I have done with BL is very very simple**. This is the most basic application of it, that's why I pointed out in the original post that I am not a quant. It can be and is applied in much more complicated and subtle ways, so see this post as a very small intro. You will need to go to google and find papers using the method to get a better picture, as far as you want to take that, which is beyond the scope of this post. Please take my post for what it is, which is something I produced in the middle of the night because I am bored of the other work I have to do this weekend. I hope you enjoyed learning about Benford's Law if it is something new to you. But this is only scratching the surface. Peace.

# Not the last edit - 30 May 2021

Am adding this on behalf of u/RogueMaven who doesn’t have enough karma to post. This is a valid perspective to take into account regarding **the notable favouring of the numbers 1 and 4** in the data. I think this shows that it is worth giving any data a good chance before dismissing too quickly. It is a process and we aren't going to come to the conclusion when we are standing at the beginning.

*Really interesting article on applying Benfords Law! I didn’t know of it until your post.* ***Intuitively I’ve known that manipulated stocks close with 1’s and 4’s more often. My assumption is 1’s mess up PUT buyers by being $1 over strike and 4’s mess up CALL buyers by being just under a $5 increment - people seem to have a tendency to think in $5’s.*** *Not enough karma to reply in forum, but I always appreciate learning something new, so thank you for writing the article 👍*

&#x200B;

# 30 May 2021, COUNTER TO THE COUNTER DD

# 1: THE DATA SET IS TOO SMALL

See *Benford's Law : Applications for Forensic Accounting, Auditing, and Fraud Detection*, 2012 by Mark J. Nigrini and Joseph T. Wells

![Benford's Law : Applications for Forensic Accounting, Auditing, and Fraud Detection, 2012 by Mark J. Nigrini and Joseph T. Wells, page 12](https://preview.redd.it/f9abus3ajb271.png?width=740&format=png&auto=webp&s=610fb11e97a2cbc534678a335e5e1d3d3058b019)

This is a book entirely dedicated to Benford's Law as a method.

The GME Max all time chart starting from 2002 has **4857** records.

The GME 5-year chart has **1259** records.

The GME 15-month chart has **355** records. This is more than 300 records so the first-digit test can be used.

So according to **Nigrini**, who, as I said in my original post, is acknowledged in the literature as establishing the validity of BL in forensic accounting, **the number of records available for GME is large enough and furthermore, there is nothing wrong in principle with testing small data sets**.

# 2: NOT ENOUGH MAGNITUDES IN GME DATA

Elsewhere in Nigrini's book, he uses the first-digit test on a small data set of a hairdresser's daily sales. The sales look like they rarely go over $100. He has no problem to test within this magnitude and to conclude that the hairdresser is fudging her numbers.

&#x200B;

![Benford's Law : Applications for Forensic Accounting, Auditing, and Fraud Detection, 2012 by Mark J. Nigrini and Joseph T. Wells](https://preview.redd.it/oc2bkrkpob271.png?width=756&format=png&auto=webp&s=2cdd20689d08cdfa230e5bca6184192930fce348)

&#x200B;

![Benford's Law : Applications for Forensic Accounting, Auditing, and Fraud Detection, 2012 by Mark J. Nigrini and Joseph T. Wells, p. 191](https://preview.redd.it/i8b8ydtnpb271.png?width=749&format=png&auto=webp&s=7c5af0b1369dfc587ca595f2c05cce8d94179f5f)

&#x200B;

# 2. BENFORD'S LAW CAN NEVER BE USED TO TEST THE PRICES OF A SINGLE STOCK

\- It has been done very recently in 2020 in *Designing Shorting Strategies with Benford’s Law,* Sedrick Scott Keh, supervised by Dr. David Rossite

![BL applied to one stock](https://preview.redd.it/kc03n0k8kb271.png?width=677&format=png&auto=webp&s=1f0071b16b09f1efef92a490dcd41888f0ca299e)

&#x200B;

This is the paper that the **Counter DD** and others cite:

https://preview.redd.it/wt8a3ozekb271.png?width=841&format=png&auto=webp&s=32f68ab1861ccc7425fb82ab9f2e77045a8feecb

&#x200B;

https://preview.redd.it/5qu80dewlb271.png?width=424&format=png&auto=webp&s=7edf79545f26de0f960e0d54b8c57284ef3bd105

\- Just because something is **"rarely covered"**, or has never been done before, doesn't mean you aren't allowed to be the first. This is a good thing. In academic research it is called **"filling a knowledge gap"**. If you are a student you will get credit for finding and filling a knowledge gap. You are pushing the boundaries of knowledge.

\- The **Counter DD** makes it sound as if the paper is arguing that BL cannot as a principle be used on stock prices because they are not natural data sets. **The paper does not say this.** The paper simply says that in Zagreb the stock prices do not conform and offers two possible reasons: *either* psychological *or* **manipulation**. Which means that BL is a proper method to use to screen for potential manipulation.

# TLDR

The data sets for all three GME charts are large enough; the magnitudes are enough; it is permissible to use BL on historical prices of single stocks; if a stock is not conforming to BL, **"the influence of financially powerful groups"** might be the reason.