# Title: 1000 Cuts 2: The Hard Way
# Author: No1Important_4real
# Post URL: [https://www.reddit.com/r/Superstonk/comments/oa9ivv/1000_cuts_2_the_hard_way/](https://www.reddit.com/r/Superstonk/comments/oa9ivv/1000_cuts_2_the_hard_way/)


**PREFACE**

A special thanks to u/yelyah2 for providing me with option data

Not long ago I noticed an anomalous price action, when the price should have been rising, it was dropping. I ran some math against it and could not find a mathematical explanation and ended up coming to procedural explanation, that the reported short interest would rise as SHF wouldn’t be able to hide their short positions any longer.

[https://www.reddit.com/r/Superstonk/comments/o0mn0y/in\_death\_by\_1000\_cuts\_shf\_just\_received\_their\_999/](https://www.reddit.com/r/Superstonk/comments/o0mn0y/in_death_by_1000_cuts_shf_just_received_their_999/)

I was wrong. I have now found what happened and how this will affect the price action we should expect going forward.

I will break this post down into two parts. Part 1 will be more technical and will present my numbers. Part 2 will be in ape with the crass language that so many enjoyed from my first post, explain the basic concepts at play, and explain how timelines have shifted.

**PART 1 - MATH**

**DATA SOURCES AND REASONING**

I have compiled data from FINRA numbers on the total of reported shorts on any given day for both the normal market and darkpool. Separately I have taken the time to tally all option trades under a certain dollar amount and over a certain quantity on each day as well. I don’t want to reveal the exacts of my query, in an attempt to prevent hedge funds from slightly altering their tactics to avoid detection.

The numbers provided will be used as a basis for understanding how many shares minimally need to be covered before a FINRA SI report settlement. The number of shorts is derived from the number of reported shorts in a given day, minus the number of reported longs in a given day. Effectively, I am working under the assumption that every long trade closes an open short position to find the most conservative estimate of shorting in a given day. Option data is tallied based on the order flow for the day and filtered to find cheap OTM puts and ITM calls that expire on a date later than the current SI report cycle. Using this method, we get the maximum number of options on any day that could have been used to hide shorted shares. To reiterate, the minimum number of shorts, the maximum number of options. I am calculating based on the best-case scenario for the hedge funds.

**HOW FINRA SI REPORTS WORK**

Before we dive into the numbers I want to cover the quick basics on how the SI report works. When a short is created there is a T+3 settlement window. Settlement is when the creation of the short is acknowledged, the receipt effectively. In normal functioning, it is intended to be the period where the person creating the short can find a share to borrow, but when you’re naked shorting the settlement window gives you just another way to hide your movements. FINRA only requires settled shorts to be reported in their bi-monthly reports, which means short sellers can have up to 3 days before the FINRA report to open new short positions without reporting them in the current SI report cycle. Historically, we would see the closing of excess short positions on the day or two before the SI report, but they always had the ability to extend three days.

**DAILY SHORTS CREATED**

&#x200B;

![Daily short positions on public exchanges and dark pool](https://preview.redd.it/t6z3mt7hs7871.png?width=376&format=png&auto=webp&s=9e32172df438a602d7618c193d94cf2943d34710)

This table displays the minimum number of short positions entered for the SI cycle from June 1st through the 15th. As per usual, the two days before the report date on the 28th, the stock price rose. We can further validate this was covering of excess short positions by seeing the large volume of new short positions created on those days relative to the rest of the chart, especially on the normal market. They simply opened new short positions to balance the ones they closed. Therefore, when calculating the period of June 1st through the 15th, we should include May 26th onward. The report on the 28th stated they had 12.67 million short positions open, so we can take 12.67 million and add it to the sum from May 26th to June 15th.

Following the typical process, they would have started closing their positions for the June 15th report on June 14th and 11th, but that does not appear to be the case, noticing no upward price movements on those days or an excess number of new short positions created. Even pushing the date to the full T+3 on June 10th doesn’t seem to show them covering their short positions. This is where I fell to my previous conclusion that they must have just not covered for this week.

Before I provide a solution however, I need to provide the next dataset, daily option volume.

**DAILY OPTION VOUME**

&#x200B;

![Maximum shares hidden in options](https://preview.redd.it/e7zytpzqs7871.png?width=344&format=png&auto=webp&s=73666b2bcb79c5902bdf77345aacfc3a7a978a4d)

As mentioned previously, I have taken the time to total the maximum number of shares that could have been hidden in options on any given day. The table above displays the minimum number of shorts opened, the maximum number of shares hidden in options, and the difference being the number of excess short positions in a given day.

**5M SHARE OFFERING CHANGES STRATEGY**

Taking these two data sets together, we can go back to the question of when they hid or closed their excess short positions for the above SI report cycle. The answer is part speculation, part math. I believe the SHF knew the 5 million share offering was coming before it was announced.

If you can accept that assumption, then the behavior changes from typical algo processes to one of manual strategy. After market on the 9th the 5 million shares were announced and affected the market on the 10th. Notice on the 8th and 9th we do see behavior indicative of the end of an SI cycle. On the 8th alone the price climbed 20% in a single hour. I believe, in preparation for the share offering, SHF closed and hid most of their excess short positions and used the rest of the cycle through the 11th shorting minimally, so that the price would move down on the announcement of the share offering and they wouldn’t have any part in propping it back up again.

What this strategy would do is not close any more short positions, but just juggle them so they wouldn’t be seen on the reporting cycle and would have to be hidden away early in the next cycle, which is exactly what happens.

&#x200B;

![Running Total minimum number of shares shorted](https://preview.redd.it/2tx0e9nzs7871.png?width=425&format=png&auto=webp&s=1b42553fd191ba60ba486d0204eb2f5a33779479)

Note: The running total starts with a base of 12.67 million, the reported SI on May 28th.

Beginning immediately after the 15th, options start running wild and provide a place for hiding of short positions. They did all of it to try and keep the momentum of the 5 million offering, pushing the stock price down and that feeds into the T+21 cycle we all knew was coming. They can choose to exercise some options early, free all those new short positions, and then immediately tuck them into new options, without upsetting the share price. The modest price swings seen on the 22nd and 23rd could have been the remainder of a now stunted T21.

**PART 2 – APE**

**-CONTENT WARNING: BAD WORDS-**

**SUMMARY**

For all you apes whose eyes gloss over when technical details start being discussed, let me summarize Part 1 in language easy enough for you. Instead of letting a computer do the trades like always, the hedgies manually did a sneaky thing to keep the price down. That’s why the price didn’t go up for the short interest report and the T+21 cycles. Even more simply: fuckery is afoot.

**HOW SHORTING WORKS: BLUES CLUES EDITION**

Get your pudding snack and gather ‘round because I’m going to explain how shorts integrate with options and the T+21 cycle at a level a six year old can understand. Since the start of this cluster-fuck that we know as the GME short squeeze the hedgies have been following a simple strategy that is carried out by their computer systems. The hedgies agree to sell you a share today that they don’t have. They’ll buy someone else’s share tomorrow and give it to you. That’s how it’s supposed to work. In reality they don’t ever buy that share they owe you. Your share is a placeholder, they still owe you 1 share, but they want to worm out of their end of the deal. Only way to do that is bankrupt GME; voiding the share they owe you.

There are controls in place to stop this kind of ass-hattery, and that is called Failure To Deliver, or FTD. After so long of not giving you the share they owe you, they will be forced to buy that share for you. That timer is 21 market days. If the timer gets past 21 days, they’ll be forced to buy shares. Sneaky Pete hedgies though can borrow shares from lenders to pay back the shares they owe. Instead of taking one dick in ass today, Kenny opted to take two in the ass tomorrow. Get used to the symbolism of Kenny getting fucked, it’s a metaphor I’m about to run into the ground.  They’ll keep repeating this homo-erotic dance until they manage to hide enough of those shares into options. What are options, you ask?

People bet on what the price of GME will be. They bet the price will go above a number or below a number and other morons can take that bet. It is blatant gambling, but everyone knows it’s fixed and still plays. The bets are sometimes called Options, also known as Puts, Calls, or even Fucking Stupid.

The worse the odds are on a bet, the cheaper that bet is to buy and if you win, you get 100 shares per bet. The hedgies will buy ass loads of cheap as shit bets so that they can cook the books and claim “here’s all those shares we owe you, as soon as the bet pays off”. And just like your crackhead uncle, they are completely full of shit and they’ll never pay you what they owe you. You’re never getting your $20 he owes you and you’re never getting your share the hedgies owe you.

One day though, these options expire and all the shares they had tied to them come crashing back onto their books. The FTD timer starts again, creating a new beloved T21 cycle. They get flooded with so many shares on these dates they have to go crazy trying to get them all under control. Every month this bomb goes off. What was one dick in the ass turns into 50, which is more than any one man can bear, even 🌈🐻 .

**THE FINRA SHORT INTEREST CYCLE: THE OTHER END**

So Ken is swinging bed posts battling off suitors from behind, but he also has polite competition coming in front of him. That sentence can be understood in two ways, and both are accurate.

FINRA is the lazy grandpa who’s supposed to be watching the kids while mom and dad get drunk, but FINRA only is interested in doing the bare minimum. Twice a month FINRA asks for a status report on short positions not an audit though, a self-report. The same game the hedgies can play with their FTD cycles they can play with their FINRA report but on a smaller timeframe. They can create new short shares, promising to pay them back later, to pay off the shares they owe, and if they create these new shorts 3 days or less before FINRA asks for the report, they don’t have to disclose them! All of this adds up to short term debt that, if Little Bitch Ken (as he's known around Chicago) doesn’t handle quickly, will begin piling up. Keeping with the metaphor, if the T21 bombs are fucking Ken in the ass, the short interest cycle is going for his face.

While these dates are bouncing around, SHF are busy buying up as many options as they can, as cheaply as they can, to pretend to close their positions, deflating the current T21s, and fueling up new ones.

**WHAT HAPPENED: THE HARD WAY**

We had a time bomb of opportunity go off on the 9th, a 5 million share offering. I believe Ken The Mayo Man saw that news and seized the carp, turning off the computer and going in raw. Instead of letting the dance play out as it has for months, SHFs stuttered the timing and started their process of covering with shorts on the 8th and 9th before the 5 million offering was announced. How and why? Fuck you, that’s why.

I think ole Kenny had a mole in GME that gave him a heads up on what was coming and was looking for a way to gain tactical advantage on his insider knowledge. If he had to cover for the FINRA SI report and two T21 cycles during a 5 million share offering, it would potentially flatten the price drop. But by juggling some numbers and his balls, he was able to settle the process early. On the 8th and 9th he started shorting with abandon while the stock price climbed, just like you’d see during a normal FINRA SI report cycle, but he was two days early, a full five trading days before the Short Interest Report. That’s fine, because Citadel is a “Market Maker” which is a financial term for someone who is allowed to cheat in the market. Rule 204 of the SEC’s rules on short selling, if a market maker that feels like it, they can extend the Settlement date from T+3 to T+6. ([https://www.sec.gov/investor/pubs/regsho.htm](https://www.sec.gov/investor/pubs/regsho.htm)) The prick just gets to pick when he wants to declare shorts as settled.  So SHFs bought up a shit ton of options on the 8th and then on the 10th and 11th, more options were bought than shorts created. Drenched in lubricant, Ken slid right under the noses of the FINRA. Then, there’s another classic trick Kenny-small-dick can pull, which is the “forget” to mark batches of shorts as short. Effectively you get to short a stock free of charge! You get a fine for it, but if done strategically you can use it in your moment of need, and Kenny needed it. Kenny only had to “forget to mark” 7% of his shorts for that period to reach 9.67 million open short positions by June 16th.

So, assuming Kenny had inside knowledge and tried pulling a fast one on the FINRA report, he would have been able to make the reported SI go down, the sell off hit harder, and sow some FUD. The catch? He on one new suitor, a third group wiggling in; regulators. Kenny is naked shorting, Kenny is insider trading, Kenny is misreporting, Kenny is a douche bag. All of these things are illegal, and that pound of flesh will come due someday. Kenny is taking it front back and center.

![A great blaxploitation film and a very perinate title](https://preview.redd.it/xi2sdbh8t7871.jpg?width=356&format=pjpg&auto=webp&s=f9dc177bf34073f6b114a0fa38a52de2a68970cc)

**THE T21: I WAS PROMISED TENDIES**

Now you’re up to speed on Kenny’s plan, he wanted the share offering to feel like a falcon punch abortion, and cause as much FUD as he could. If you can glance up at the charts above without having seizures, you might see that on June 16th options purchased went ape shit. There’s a string of massive movements when it comes to option buying that likely was done by SHFs. Typically a large string of options is one or two million, they bought 14 million and then 5 million more the next day. Either those options were used to hide their current excess short position, bringing it effectively down to zero, or they were deflating that T21 cycle to yet again spread FUD and allow the share offering to play out to maximum effect.

**THE FUTURE: WEN MOON (AND TLDR)**

The actual useful bit for everything above is this: Kenny is still fucked (if all the dick jokes weren’t hint enough), but now he’s even more fucked. Like usual, he did a dick move on his way out though and fucked up the T21 calendar. Going forward it might not line up anymore on the cycles we had previously mapped, but now there’s a fucking Fat Man sitting on July 16th and Little Boy in Oct. That’s a World War 2 A-bomb reference, but also those are the street names of two of Kenny’s suitors, purely coincidence.

How 002 factors into anything going forward, or if it does at all I can’t tell. I just know that based on the behavior of the last two weeks, our calendar of hype dates is doubtful. Going forward I’ll keep an eye on these price movements and provide updates and best guesses as to what the current cycle’s progress is. **Just to be safe, I think we should all get hyped every day.**

**EPILOGUE**

This isn’t a moon soon post but I do want to close with one last idea. Kenny’s been in, what will soon be, a sticky situation for months and is trapped. His strategy clearly hasn’t worked to keep the price down. If it had, he wouldn’t need to deploy a desperate and ‘short term win for long term loss’ strategies like the ones he just did. He’s sinking, and it’s moves like the ones he’s making now that really prove his overall strategy isn’t working. Day after day the hedge funds are generating a minimum of tens of thousands, sometimes millions, of shares they can't cover. Their desperate attempts to hide them and juggle them are getting more and more uncontrollable. MOASS isn't a question of if, but when.

I will leave this section for answering questions in the comments.

&#x200B;

Q: ([Apprehensive\_Royal77](https://www.reddit.com/r/Superstonk/comments/oa9ivv/1000_cuts_2_the_hard_way/h3gg1da/?utm_source=reddit&utm_medium=web2x&context=3))  I'm interested in your assumption that the SHF knew about the ATM offering. It implies that they have insider trading knowledge of Gamestop even after the old board has been removed.

A:  Share offerings have a workflow involved both internally and in terms of regulation. Lawyers have to draft filings, those filings have to be submitted to the SEC and any other relevant entities, accepted and approved, then the actual handling of the shares and the cash flow has to be handled. There are a lot of folks involved outside of the board. Any one of them from an SEC desk jocky to a finance department middle manager to even a janitor could of leaked the info.

With how connected Kenny is to the world of finance, I would think him having some competitive intelligence operative entrenched in his major interests is likely. The second most likely scenario is that he guessed randomly a day before the share offering. I see no other reason why the behavior for an SI cycle would be carried out 5 days before an SI cycle when it has always been 1 or 2 days before an SI cycle. Seems far too coincidental.

&#x200B;

Q: ([TheDragon-44](https://www.reddit.com/r/Superstonk/comments/oa9ivv/1000_cuts_2_the_hard_way/h3g1j8v/?utm_source=reddit&utm_medium=web2x&context=3))  So June 16th was 14 million options correct? What is t+21 from June 16th? Could that be the new reset?

A:  That is the purchase of options, those options expire at a different date and not all of them expire on the same date, but many of them expire on July 16th.