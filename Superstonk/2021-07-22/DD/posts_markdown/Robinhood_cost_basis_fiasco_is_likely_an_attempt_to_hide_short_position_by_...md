# Title: Robinhood cost basis fiasco is likely an attempt to hide short position by truncating the position - Rule 4560. This could explain dark pool usage and decreasing SI%.
# Author: Precocious_Kid
# Post URL: [https://www.reddit.com/r/Superstonk/comments/opna24/robinhood_cost_basis_fiasco_is_likely_an_attempt/](https://www.reddit.com/r/Superstonk/comments/opna24/robinhood_cost_basis_fiasco_is_likely_an_attempt/)


I'm sure you've all seen a number of the posts regarding RH users posting screenshots of their cost basis being all out of whack and cobbled together through various fractional shares, though they never purchased fractional shares. Examples: [1](https://www.reddit.com/r/Superstonk/comments/ngs81d/just_got_my_cost_basis_information_from_robinhood/), [2](https://www.reddit.com/r/Superstonk/comments/ngkrg3/proof_that_rh_had_to_scramble_to_find_shares_when/), [3](https://www.reddit.com/r/Superstonk/comments/ncj1sm/if_you_transferred_out_of_robinhood_look_at_your/), [4](https://old.reddit.com/r/Superstonk/comments/ncezct/so_robinhood_finally_sent_over_my_cost_basis_from/), etc ad nauseam. 


Well, as it turns out, this may have been an intentional ploy by RH/Citadel to circumvent the short interest reporting requirements from FINRA. If you read the [Regulatory Notice 12-38 regarding FINRA's Short-Interest Reporting Rule](https://www.finra.org/rules-guidance/notices/12-38), you'll come across this particularly relevant question in the FAQs. 


>**Q7 How should a firm reflect fractional shares in its short-interest reports?**

>A7. If a firm has a fractional short-interest position (e.g., 125.6 shares), it ***should truncate the position to reflect a whole number*** when reporting such positions to FINRA pursuant to FINRA Rule 4560, ***instead of rounding the position up or down***. For example, firms should report short-interest of 125.6 shares in XYZ as 125 shares. 

So, what does this mean? Well, it means that all shares are rounded down when it comes to short interest reporting. If you purchased a single share, and Citadel is forced to short that position, they could break it into multiple pieces across two or more transactions (e.g., 0.4 shares and 0.6 shares) and **COMPLETELY AVOID REPORTING THE SHARE AS SHORT!** 

This is about as egregious as it gets and is another way for the MMs and SHFs to hide short positions. This might also explain why they're running so many shares through dark pools. If they have a complicit party involved and are taking their short positions, covering and re-shorting via fractionals to SHF2 through the dark pool, they could run their short interest down to 0% based on this ridiculous truncation rule. 

Tagging /u/criand /u/luridess /u/Leaglese /u/atobitt to get some further eyes on this one.

EDIT: Thankfully it's not too late to change what's happening. The comment period is still open for **Regulatory Notice 21-19** ***[FINRA Requests Comment on Short Interest Position Reporting Enhancements and Other Changes Related to Short Sale Reporting](https://www.finra.org/rules-guidance/notices/21-19)***. I took a quick look through their proposed changes and do not see anything regarding a change to fractional share reporting. A simple comment requesting that they report all amounts, fractional and whole, and that they report all outstanding loan obligations should be sufficient.

EDIT2: /u/ammoprofit has a fantastic call out in the comments, [here](https://www.reddit.com/r/Superstonk/comments/opna24/robinhood_cost_basis_fiasco_is_likely_an_attempt/h66mie1/). 

>Normally this wouldn't matter, because it would be less than 1 share * number of orders affected. For example, 126.99 gets truncated to 126 shares. 1000 orders * 0.99 = 99 shares [sic]. Yeah, it matters. It's a non-zero number, but it's truly negligible in a sea of volume.

>Except [RobinHood's shares per transaction volume is exactly one](https://www.reddit.com/r/Superstonk/comments/mzwipl/robinhood_is_11_trading_against_every_ticker_they/). Those fractional shares reduce the short interest position from the sum of the orders' volume to zero.