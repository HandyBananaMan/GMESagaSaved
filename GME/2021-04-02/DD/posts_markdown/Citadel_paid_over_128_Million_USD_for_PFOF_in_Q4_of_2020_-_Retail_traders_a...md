# Author: HawkFrequent9676
# Post URL: [https://www.reddit.com/r/GME/comments/midcwe/citadel_paid_over_128_million_usd_for_pfof_in_q4/](https://www.reddit.com/r/GME/comments/midcwe/citadel_paid_over_128_million_usd_for_pfof_in_q4/)


# Overview

This post is about payment for order flow (PFOF), and specifically how Citadel pays brokers for trade order flow--especially that of retail traders. I won't harp on the "why", but suffice it to say order flow is EXTREMELY VALUABLE. With PFOF, you are not the customer, you are the product.

Most people here have probably heard about PFOF. If not, here is a primer: [https://www.investopedia.com/terms/p/paymentoforderflow.asp](https://www.investopedia.com/terms/p/paymentoforderflow.asp)

Additionally, I HIGHLY encourage people interested in this topic to read Dennis Kelleher's written testimony to Congress during the recent Gamestop hearing by the US Financial Services Committee: [https://bettermarkets.com/sites/default/files/Kelleher%20HFSC%20Testimony%20GameStop%20Hearing%203-17-2021%20FINAL%20%282%29.pdf](https://bettermarkets.com/sites/default/files/Kelleher%20HFSC%20Testimony%20GameStop%20Hearing%203-17-2021%20FINAL%20%282%29.pdf)

And here is Alexis Goldstein's written testimony, also relevant to PFOF and full of good info: [https://docs.house.gov/meetings/BA/BA00/20210317/111355/HHRG-117-BA00-Wstate-GoldsteinA-20210317.pdf](https://docs.house.gov/meetings/BA/BA00/20210317/111355/HHRG-117-BA00-Wstate-GoldsteinA-20210317.pdf)

The focus of this post is Citadel because they are the largest MM in the PFOF business. There are several others such as Virtu, G1X, Two Sigma, Wolverine, and others. I don't have the time to cover them all here so I will stick with Citadel. Maybe in the future (and if there is interest from redditors) I will evaluate other MMs. Terminology note: you can call them Market Makers ("MM"), wholesalers, internalizers, and possibly words not fit to print here, but the terms are interchangeable.

Lastly, [u/atobitt](https://www.reddit.com/user/atobitt/) previously posted links to the various disclosures in their DD here: [https://www.reddit.com/r/GME/comments/mbgsl8/huge\_citadel\_is\_paying\_for\_order\_flow\_from\_nine](https://www.reddit.com/r/GME/comments/mbgsl8/huge_citadel_is_paying_for_order_flow_from_nine/) They left out Interactive Brokers so their list looks a little different than mine.

# Now, to the "OC" part of my post...

Thankfully, SEC Rule 606 requires brokers to disclose this information publicly, although the format is not easy to digest and the raw data doesn't say too much without a little extra effort parsing everything.

I simply took all of the Rule 606 disclosures from various broker websites and pulled them into Excel. I added a few formulas and graphed it.

# Results

&#x200B;

[Citadel PFOF](https://preview.redd.it/3d7a8zigloq61.png?width=1106&format=png&auto=webp&s=fba4cb0e2a0b153f32264f610dc3340f507ad5f4)

&#x200B;

[description](https://preview.redd.it/l71gunzlloq61.png?width=1100&format=png&auto=webp&s=98523c25802a011b090b06375bc2ed985fd22b25)

&#x200B;

[shares](https://preview.redd.it/9g28u5brloq61.png?width=742&format=png&auto=webp&s=706db34b33d17e8bc55ef4aea2a0a15138f1b1a4)

&#x200B;

[shares, pie](https://preview.redd.it/vi7y035xloq61.png?width=730&format=png&auto=webp&s=c51da4b49f0256907c1b0a4c716804ef2441cfef)

&#x200B;

[Net Payments](https://preview.redd.it/pqvmfvw0moq61.png?width=741&format=png&auto=webp&s=2ad8d78a2c51f8291fd47065d8457aa78e03ca85)

&#x200B;

[Net Payment, pie](https://preview.redd.it/1lnzmb47moq61.png?width=738&format=png&auto=webp&s=77ac5f825ab617ab33dd99b70d3c7404a70863ab)

&#x200B;

[$\/Volume](https://preview.redd.it/88mtg5bemoq61.png?width=735&format=png&auto=webp&s=2e3f6c562b78ed40099b8e07a1840d2601a404a2)

&#x200B;

# Here is the data --> [https://drive.google.com/file/d/1jpxGp6zrwdev0lMTf-WN\_fClBWvqb0bO/view?usp=sharing](https://drive.google.com/file/d/1jpxGp6zrwdev0lMTf-WN_fClBWvqb0bO/view?usp=sharing)

&#x200B;

# Analysis

The data is pretty straightforward. I'll mention a few important items.

Robinhood: PFOF is lifeblood for Robinhood. I've thought about doing a broker focused post (rather than MM focused) because it is interesting to see all of Robinhood's "customers" (MMs). Citadel paid Robinhood $31.9 million USD in Q4 in exchange for routing nearly 139 million shares to them. At 23 cents per 100 shares, Citadel pays Robinhood MORE than ANY other broker! (unless we combine TD Ameritrade's branches, see below).

TD Ameritrade: After Robinhood, TD Ameritrade is the biggest broker to send shares to Citadel through PFOF. But is that accurate? I found TWO Rule 606 disclosures on TD Ameritrade's website [https://www.tdameritrade.com/disclosure.page](https://www.tdameritrade.com/disclosure.page)\--one for "TD Ameritrade, Inc." and one for "TD Ameritrade Clearing, Inc." If you combine these, you get volume amounting to 52% of the shares sent to Citadel via PFOF, compared to Robinhood's 16%. Apparently TD Ameritrade gets a better deal, however, because they spend approximately 13 cents/100 shares in PFOF, saving a dime per 100 shares compared to Robinhood. Citadel paid TD Ameritrade $58 million USD in Q4, almost twice what Robinhood made, but with much greater volume.

I believe payment per 100 shares is the fairest comparison as it "normalizes" the payments between big and small brokers. When we do that, we see that the ranking is in this order: Robinhood (23 cents), Ally (21 cents), WeBull (18 cents), E\*TRADE (15 cents), TD Ameritrade (13 cents), and everyone else around 11-12 cents. The average payment is 15 cents per 100 shares.

# Additional Comments regarding methodology and whatnot

Rule 606 disclosures are standardized (thank God) and break down into Market Orders, Marketable Limit Orders, Non-Marketable Limit Orders, and Other Orders. For purposes of this post, I don't care about the separate orders but Math does, so I treated them all separately to run some calculations before combining them.

Number of shares = Net Payment Paid for Specific Order Type \[USD\] \*100 / Net Payment Paid for Specific Order Type \[cents per 100 shares\]

Seriously, they couldn't disclose the number of shares!? Note this formula is prone to errors, e.g. Fidelity doesn't pay for PFOF so I couldn't find out how many net shares they send to MMs via this method.

Total Shares per Venue = Sum of Number of Shares for all Order Types

Net payment paid/received for All orders = Sum of Net Payment Paid for all Order Types \[USD\]

Average Weighted Net Payment for All orders = For every order type, multiply Net Payment paid by the  number of shares, then sum these together and divide by the Total Shares per Venue

Data check: I am trying to provide my calculations to be completely transparent (you can download my excel file from my google drive mentioned above).

As a sanity check, it is good to know my average weighted net payment paid calculation matches that of Robinhood's COO Jim Swartwout [https://robinhood.engineering/demystifying-payment-for-order-flow-119581544210](https://robinhood.engineering/demystifying-payment-for-order-flow-119581544210) ...wait, now that I read his article, maybe I don't think it is good for my numbers agree with his. After all, this is the same guy that chose to compare their 23 cents / 100 shares, not with other brokers who offer zero commission trading and use PFOF (every broker mentioned above), but instead he compares their 23 cents / 100 shares with a snapshot from 1993(!) when a retail trader would have paid $30+1.7% for an exemplary 100 share trade. I'd like to see Jim argue PFOF is necessary (and moreover that 23 cents is a good deal!) when compared with Fidelity. Not to mention that, at least to me, the actual payment amount is less important than the nefarious use of data by the MM who pays for order flow, which causes less tangible, unknown damage to retail traders. See Kelleher's paper mentioned above for more on this.

&#x200B;

\*\*\*\*\*

It is April 2021...I'm expecting Q1, 2021 data to be published by end of month. Are people interested in me doing a post with the Q1 data?

Did I leave out your broker? Let me know and I can add it. (Note, Fidelity is mentioned above and their data is in the spreadsheet, but they do not pay for PFOF so I didn't include them in the Citadel chart).

&#x200B;

 

# Edit 1:

**DISCLAIMER**: I am not a financial advisor nor a lawyer, and I'm definitely not your lawyer. Please don't take my words for gospel and question everything you read in this post. If I'm wrong, which is entirely possible, please correct me. Seriously, we will all benefit from it. Our power lays in the collective brainpower that we amassed over here and it's honestly beautiful to see. But IMHO, we should all question everything we read and do our own DD and research.

Thanks [/u/DwightSchrute666](https://old.reddit.com/u/DwightSchrute666) for the disclaimer

For more on "why" we should stop using Robinhood, see this post by u/killabeezio: [https://old.reddit.com/r/GME/comments/macno0/why\_you\_should\_probably\_stop\_using\_robbinghood/](https://old.reddit.com/r/GME/comments/macno0/why_you_should_probably_stop_using_robbinghood/)  


Notes on other brokers (in no specific order):

(1) Chase (owned by JP Morgan)

JP Morgan (and others?) use VistaOne Regulatory services [https://vrs.vista-one-solutions.com/sec606rule.aspx](https://vrs.vista-one-solutions.com/sec606rule.aspx)

Searching for JP Morgan, there are "No Covered Orders" for Q4 2020. My spidey senses are wondering whether this report offloading is genuine or an attempt at obfuscation / plausible deniability (i.e. the entity can say "Oh, I don't know why that report was unavailable! Not our problem since we have contracted that out to VistaOne!"

Needs more research

(2) eToro - [https://www.etoro.com/customer-service/regulation-license/](https://www.etoro.com/customer-service/regulation-license/)

Operates in UK, EU, USA, AUS, needs more research

(3) Wealthsimple (Canada)

Canada doesn't allow PFOF

(4) Sogotrade (Latin America)

[https://content.sogotrade.com/pdf/sec/606.pdf](https://content.sogotrade.com/pdf/sec/606.pdf)  


Does accept PFOF, mainly CODA and Virtu in Q4,2020. No known Citadel relationship

(5) Trade Republic (Germany)

Fees mentioned here: [https://traderepublic.com/en-de/pricing](https://traderepublic.com/en-de/pricing)

Terms & Conditions (auf Deutsch): [https://assets.traderepublic.com/assets/files/Kundenvereinbarung.pdf](https://assets.traderepublic.com/assets/files/Kundenvereinbarung.pdf)

Relevant post...? (in German) [https://www.reddit.com/r/Finanzen/comments/l8urtb/meine\_ehrliche\_meinung\_zu\_0\_trading\_apps\_und/](https://www.reddit.com/r/Finanzen/comments/l8urtb/meine_ehrliche_meinung_zu_0_trading_apps_und/)

(6) Drivewealth - [https://legal.drivewealth.com/sec-rule-606](https://legal.drivewealth.com/sec-rule-606)

Drivewealth acquired Cuttone recently, here is their 606: [http://public.s3.com/rule606/ttuc/](http://public.s3.com/rule606/ttuc/)

Does not appear to accept PFOF, rather they pay Bofa Securities for execution, looks legit and fair (at least at first glance).

(7) SoFi aka "Apex Investing" - [http://public.s3.com/rule606/apex/](http://public.s3.com/rule606/apex/)

TL;DR **not good, need to add them to the excel file**

accepts PFOF

does business with Citadel, Virtu, Jane Street Capital, Two Sigma, and perhaps others

(8) DEGIRO - EU-based broker

I could not find a US SEC Rule 606 disclosure for order routing. I'm not sure if EU allows PFOF. However, according to wikipedia DEGIRO has been in hot water at least once..."The process of internalization of customer's orders against DeGiro's own [hedge fund](https://en.wikipedia.org/wiki/Hedge_fund) HiQ Market Neutral fund was subject of investigative press."

![Amsterdamtrader.com](http://www.amsterdamtrader.com/2015/10/how-degiro-screws-clients.html), How DeGiro Screws Clients, 20 October 2015  
