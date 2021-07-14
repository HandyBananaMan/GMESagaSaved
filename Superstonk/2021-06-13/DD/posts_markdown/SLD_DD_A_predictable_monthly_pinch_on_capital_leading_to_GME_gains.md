# Author: dentisttft
# Post URL: [https://www.reddit.com/r/Superstonk/comments/nz7mwl/sld_dd_a_predictable_monthly_pinch_on_capital/](https://www.reddit.com/r/Superstonk/comments/nz7mwl/sld_dd_a_predictable_monthly_pinch_on_capital/)


# Preface

Alright, I got some info I’ve been looking into for a couple of months now. Three weeks ago when [I originally posted about it](https://www.reddit.com/r/Superstonk/comments/njgs66/rc_tweet_analysis_part_2_dumb_and_dumber_turbolax/), I didn’t know how big of a deal it was. But after May it has become more clear.

For those who have seen u/Criand ‘s [net capital post](https://www.reddit.com/r/Superstonk/comments/ny2ov4/a_revisit_to_net_capital_what_is_truly_driving/), this info is an alternative look at very similar ideas. Hedge funds have time periods where they need to make sure they have money. When FTDs coincide with these time periods, GME goes brrrr. Criand’s net capital posts and this post probably both happen, but we both focused on different areas.

&#x200B;

 Posts with memes seem to get more attention, so here’s a meme. 

[Photo of me from the past month.](https://preview.redd.it/ru7ahkfet3571.jpg?width=1024&format=pjpg&auto=webp&s=663262c95306797eee84275665ae49c7694b5dc6)

# Introduction

Every month, hedge funds need to deposit money to the NSCC near the time of monthly option expiration. They do this in order to have extra money in case things go horribly wrong during monthly expiration. After some time, the money is returned to the hedge fund and everything goes back to normal. This deposit is called **Supplemental Liquidity Deposits**. Everyone remembers NSCC-2021-803. 803 changes this monthly SLD period that I'm about to explain into daily checks instead. But for now, the old rules still apply.

For the rest of this post:

* Hedge funds will be called **Members**.
* The place where the money goes will be called the **Clearing Corporation**.
* Supplemental Liquidity Deposits will be called **SLD**.

&#x200B;

Now let’s talk about Liquid Deposits...

https://preview.redd.it/9irecyztt3571.png?width=444&format=png&auto=webp&s=a33d5a0c86779a29131b3a2693b1d183416ba677

# How does it work?

SLD rules are defined in the NSCC rulebook, Rule 4(a). Rule set can be found here: [https://www.dtcc.com/\~/media/Files/Downloads/legal/rules/nscc\_rules.pdf](https://www.dtcc.com/~/media/Files/Downloads/legal/rules/nscc_rules.pdf)

If you’re a smooth brain that thinks 0 wrinkles is way too many, skip the Definitions and Rulebook sections. I’m just going to summarize the important stuff.

 

**==== DEFINITIONS START ====**

***Monthly Expiration Date:*** The Saturday where the monthly options expire. It’s the Saturday after the third Friday of the month. (Often people think of options expiring on Friday, but they technically expire on Saturday. You just can’t trade them after regular trading hours on Friday, so it’s essentially Friday).

***Options Expiration Activity Period*****:** It starts at the opening of business on the Friday before the Saturday Monthly Expiration Date and ends at close of business on the second Settlement Day after the start. So, essentially close of business on Tuesday.

***Special Activity Calculation Date:*** The date where the amount needed for the deposit is calculated. There is no set date when this happens, the only requirement is that it has to be done no later than the fifth business day preceding the *Options Expiration Activity Period* (the Friday of the week before monthly expiration).

***Special Activity Prefund Deposit:*** The name of the deposit that the member will have to make based on the Calculation Date.

***Special Activity Liquidity Call:*** Between the monthly calculation dates, if the clearing corporation realizes the deposit isn’t big enough, they will require a larger deposit to be made within 2 business days of the call. The Liquidity Call deposit is then held for 90 days. (So if Melvin and Robinhood really did get liquidity called, they wouldn’t get that money back until April 28-30)

**==== END OF DEFINITIONS ====**

&#x200B;

**==== RULEBOOK START ====**

**When the deposit needs to be made...**

>*SEC. 6 Notice of Special Activity Liquidity Obligations and Payment of Special*  
>  
>*Activity Supplemental Deposits. Promptly after the Special Activity Calculation Date,*  
>  
>*the Corporation shall provide each Special Activity Liquidity Provider with the amount of*  
>  
>*its Special Activity Liquidity Obligation for that Options Expiration Activity Period.* ***Not***  
>  
>***later than the close of business on the second Business Day preceding the applicable***  
>  
>***Options Expiration Activity Period, a Special Activity Liquidity Provider shall make its***  
>  
>***Special Activity Supplemental Deposit to the Clearing Fund.***

&#x200B;

**When the deposit needs to be returned…**

>*“Special Activity Prefund Deposit” means a cash deposit of a Member to the Clearing*  
>  
>*Fund made by wire transfer to an account designated by the Corporation:*  
>  
>*\[...\]*  
>  
>*c.* *that the Member undertakes to keep on deposit in the Clearing Fund for at*  
>  
>*least seven Business Days after the end of the applicable Options*  
>  
>*Expiration Activity Period*\*; and\*

**==== END OF RULEBOOK ====**

&#x200B;

**Hey you! I know you skipped those sections, come back!**

&#x200B;

Putting it all together:

* Early in the month, the Clearing Corporation tells the 30 largest Members how much money they need to deposit for the Options Special Activity Period.
* The Options Special Activity Period starts on Friday and ends 2 business days after (usually Tuesday).
* Two days before the Options Special Activity Period, the Prefund Deposit is made (Wednesday).
* The deposit is returned after 7 business days following the Options Special Activity Period (usually Thursday).
* If for some reason the deposit amount needs to be increased, there is a Special Activity Liquidity Call for Members to deposit more money.

&#x200B;

This means there is a 12 business day period every month where the Members are tight on money... meaning less money for any potential tricks/price suppression. Any liquidity calls get held for 90 days. Interestingly when Robinhood shut off the buy button in January, they said they were asked for more money. This is because they got liquidity called. (The congressional hearing revealed Melvin also got liquidity called in January) 

&#x200B;

# Chart Time

 Now to highlight the SLD period on the 1 day chart. 

[1D GME Chart with SLD periods highlighted \(from time of payment to when the deposit is returned\)](https://preview.redd.it/9is0brqdv3571.png?width=1246&format=png&auto=webp&s=cbdd7218099a82c29adbab153e8aa956a8473451)

 **Okay great, but why are some SLD periods bigger than others?** 

&#x200B;

*Warning:* I’m about to connect a bunch of numbers and dates using text. It gets hard to follow. So I’ll include a chart afterward and you can follow along at home. But the chart is also confusing...

&#x200B;

* **January:** Most of January had 600,000-1,000,000 FTDs due from December. So there is a large price increase immediately when the payment is made. GME continues to rise the entire period, Robinhood cuts off buying GME when they are liquidity called, and GME promptly starts falling at the end of the period.
* **February:** Using my [T+35 theory](https://www.reddit.com/r/Superstonk/comments/nsady3/t21_is_not_actually_a_thing_counter_dd/), January 19-21 needed 1-1.5 million FTDs due on each day (Jan 19: 1.5 million, Jan 20: 1 million, Jan 21: 1.4 million). The FTD numbers are a cumulative total, So I believe that on January 19 only 500,000 FTDs were taken care of (leading to the small February 22 bump), nothing was covered on January 20, and January 21’s 1.5 million FTDs were done at the end of the day on February 24 during SLD.
* **March:** The beginning of March is due to T+35 from January 26-January 28 FTD’s. The price was suppressed, but not dropped in order to avoid another liquidity call. February’s large FTD days (Feb 24th and 26th) are due March 30 and April 1, outside of SLD. So nothing big happened.
* **April:** The largest FTD days due in April are April 15 (March 16 and 19),  April 26 (March 23), and April 29 (March 26 and March 29). Some of the April dates correspond to two March dates because the FTDs are due on the weekend. April 14 bumps right after the deposit, April 15 FTDs are covered in the second half of the day after a drop, April 26 is in SLD, April 29 is right at the end of the SLD (see note after this section).
* **May:** The largest FTD days due in May are May 11 (April 7), May 13 (April 9), and May 24 (April 20). The FTD numbers are all similar (about 80,000), but the first two are out of SLD causing small bumps. The last one is in SLD, causing a big spike which can’t be controlled until SLD is finished, leaving a continual price increase from every FTD covered thereafter.

&#x200B;

[1D GME Chart with big FTD dates mapped out to where they get covered \(the numbers represent the day of the month to hopefully help read this extremely confusing chart\)](https://preview.redd.it/s7xkhb5mv3571.png?width=1093&format=png&auto=webp&s=f7f80b4e2aa06abad5bf657072aac77337cd34db)

Remember that exercising an option will take two days to settle (buying and selling contracts it T+1, but exercising is T+2). So the days with big FTD numbers that I highlight come from options that are exercised two days earlier.

 

**Important Note:** GME’s price often drops during the last two days of SLD. I don’t know exactly why. My current theories are:

1. Options premiums get way too expensive from the FTDs and gamma ramp slows down.
2. The liquidity calls allow you up to two days to pay them. So if the Member’s deposits are going to be returned within the next two days, there is no point in giving them a liquidity call.
3. A new calculation day comes for the next month making the current SLD period not important.
4. Some interaction between SLD and Net Capital.

I’m leaning towards a combination of (1) and (2).

# Wrapping it all up (tl;dr)

* FTDs are due all the time. The FTDs due during SLD lead to a much larger price increase than the FTDs due outside of SLD.
* Once FTDs due from SLD has increased the price dramatically, it is hard to suppress the stock price without getting liquidity called until the SLD period ends.
* The recent GME runup from May should create a lot of FTDs. The majority of ITM calls get exercised on Friday, which will correspond to July 5th (outside of June’s SLD). If a lot of apes exercised early in the week (specifically on May 24), then there could be a handful of FTDs that fall at the end of June’s SLD period.
* Predictions will be more accurate after the new FTD data comes out on Wednesday. I’ll make a follow up post on my thoughts.

 

That’s all I got for today. I was quite busy last week and it made posting hard, but now I should be free to start making more posts.

&#x200B;

Until next time,

\- u/dentisttft

&#x200B;

PS. I’m starting to get to the point where it’s hard to respond to everyone. So apologies in advance if I leave you hanging. Thanks for all the support!