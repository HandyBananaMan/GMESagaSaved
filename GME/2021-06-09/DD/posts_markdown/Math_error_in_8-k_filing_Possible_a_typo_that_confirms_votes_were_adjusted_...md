# Author: Rimigo42
# Post URL: [https://www.reddit.com/r/GME/comments/nw9sl1/math_error_in_8k_filing_possible_a_typo_that/](https://www.reddit.com/r/GME/comments/nw9sl1/math_error_in_8k_filing_possible_a_typo_that/)


**TL;DR**

A small typo in the 8-k vote numbers means the vote count is almost certainly altered. No way of knowing actual vote count. Actual vote count could be accurate, could be a bajillion million trillion.

Buy, Buckle Up, HODL. Not financial advice.

**The Post**

By now we all know that the 8-k was adjusted. I think I’ve found definitive proof of that. I found a math error in the 8-k filing that might (maybe) mean something (maybe). I've double checked for typos/errors and it looks like I got it right, but please confirm my math and check for typos.

The total vote count (which was not shown on the 8-k) for every member and every proposal was 55,541,279 shares. EXCEPT for Larry Cheng (see image below, highlighted cell). He got 1 extra vote.

&#x200B;

[Transcribed vote numbers by hand from the 8-K filing](https://preview.redd.it/to7f8iev4g471.png?width=575&format=png&auto=webp&s=192fbfee21a26e7aa642599380c62606f3bcc631)

&#x200B;

[Snip of 8-K filing to compare numbers. I double checked, but typos happen.](https://preview.redd.it/a3k87myx4g471.png?width=624&format=png&auto=webp&s=f264665948ad4fec7c207772ebce71018285ea11)

**Background on me**

I'm an estimator for a construction company. I live in Microsoft Excel, and I do math for a living. Rounding errors are my enemy, so I'm adamant about double/triple checking for them prior to submitting a bid/tender/quote. I always take price tables and calculate by hand to check for typos.

**My smooth-brained speculation**

I think the vote auditing company took the relative percentages for each vote and multiplied it by 55,541,279 (a number that's just under today's float as reported on Yahoo Finance of 56.89M). Why 55,541,279? Either a) no reason, just a random number below current float/outstanding shares, or b) it exactly matches the float on the cut-off date (Apr. 15? Not confirmed). Doesn't really matter why.

Say there were 400M votes (random number again, not fact based) and they were scaling it back to 55.5M. If they took the relative percentage and then rounded to the nearest share, there's a chance that the total number of votes could add up to 1 or 2 above or below the number they picked. That's what I think happened here.

I think Larry Cheng's extra vote is just a miss or typo that no one caught prior to filing. I think the votes exceeded outstanding shares but the numbers were adjusted so the vote could go through and the newly elected officers could take up their positions uncontested. Wes Christian said these numbers get adjusted in his AMA.

So considering that, there's no actual way of telling how many votes were cast (see other peoples' DDs for estimates. Not linked here). We can only infer from the typo in Larry's vote count that the numbers were altered. My opinion: Bullish AF. I'm going to continue hodling. Do whatever you see fit with your own shares (no financial advice given)

Wrinkle brains, please poke holes.

Also, this is my first post. I didn't check for karma requirements first, so I hope this gets through. Second post attempt edit: It did not go through. Had to go farm karma. This is a couple hours delayed because of that. Please excuse the obvious karma farming on my acct. January Hodler, I have been a lurker up until now.

Obligatory rockets: **🚀** **🚀** **🚀** **🚀** **🚀**

Edit 1: Changed flair to DD

&#x200B;

Edit 2: An example for some clarity on how this rounding error might occur. Please remember that I made these #s up and I have no idea what the actual vote count is.

&#x200B;

[Let's assume they got 400M votes](https://preview.redd.it/b08m0wjwdd471.png?width=635&format=png&auto=webp&s=f6e616683a9657dcf8f7fb6057773c52f4133e10)

&#x200B;

[Here's what that looks like as a &#37; \(matches the actual votes on the 8-K filing to 5 decimal places.](https://preview.redd.it/i64d3nnzdd471.png?width=637&format=png&auto=webp&s=8d2217cfeaeda8365d124964871dae4797b8b8fd)

&#x200B;

[Everything looks good here, all votes total to 55,541,279 as expected. No we need to get  rid of those decimals.](https://preview.redd.it/ayv4h1u5ed471.png?width=636&format=png&auto=webp&s=8fbc28cda7a77b8f6a7e63a65cd0e8d33f7f1b28)

&#x200B;

![Using the ROUND function in excel, now we have an error for Larry Cheng's vote total.](https://preview.redd.it/b3edwwoaed471.png?width=636&format=png&auto=webp&s=8529b61672f3da92f11c2b898584b7865490d6aa)

PART 4 is the result we see. I used the actual votes from the 8-K so you could see exactly how this rounding error might occur.Larry Cheng had 3 vote counts with numbers that are over 0.5 for the decimal but not too much over. That's important, because now it rounds up ALL 3 of those numbers. That's where the error occurs. Now our rounding function gave Larry 1 extra vote.There's no way someone just cast 1 vote for Larry because that would have added 1 abstention to everyone else, making the vote count increase by 1 for every proposal.

Remember, I made these #s up. I have no way of knowing what the actual vote count is. If you're looking for a prediction, check out all the posts about % of shareholders voted from our EuroApe friends.

\*\*\* end of Edit 2 \*\*\*

Edit 3:  
Added the first two images back in. Some comments mentioned they weren't loading.