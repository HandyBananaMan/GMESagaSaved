# Title: Found a few interesting things in the newly filed SR-NSCC-2021-004 that came out today.
# Author: Klone211
# Post URL: [https://www.reddit.com/r/GME/comments/mg5z30/found_a_few_interesting_things_in_the_newly_filed/](https://www.reddit.com/r/GME/comments/mg5z30/found_a_few_interesting_things_in_the_newly_filed/)


Thanks to [u/Shooting4daMoon]( https://www.reddit.com/user/Shooting4daMoon) for posting the [filing]( https://www.sec.gov/rules/sro/nscc.htm#SR-NSCC-2021-004)!

&nbsp;

*Not a financial advisor, it's just what I got out of the filing. If I wrote anything incorrectly or missed a key point PLEASE let me know and I will append it when I can.*

&nbsp;

**TL/DR: The NSCC is tightening the noose around over-leveraged firms. [Bears r moar fukd](https://youtu.be/OLmQTIS9Rv4).**

Edit 1: The VaR does not need HV to be calculated, however, removing IV still provides better accuracy.

Edit 2: Added fitting video reference for TL/DR. Thanks [u/desertrock62](https://www.reddit.com/user/desertrock62)!

&nbsp;

#There were two things that got my attention:

##1. [Implied volatility]( https://www.investopedia.com/terms/i/iv.asp#:~:text=Implied%20volatility%20is%20a%20metric,it%20to%20price%20options%20contracts.)(IV) will no longer be incorporated into the calculation of the [Value-at-Risk](https://www.investopedia.com/terms/v/var.asp)(VaR)

Under Section 5.2.1
> … the amount of [Clearing Fund]( https://www.dtcc.com/~/media/Files/Downloads/legal/rules/nscc_rules.pdf) required from each Member is determined principally by Value-at-Risk (“VaR”) calculations,21 and that in order to ensure the VaR model accurately reflects market conditions and provides adequate protection against market risk, NSCC evaluates several factors on an ongoing basis. The proposed rule change would remove the following factor as one of those evaluated, because it is no longer part of NSCC’s model calculation, “Implied volatility to assess whether a potential increase in market price volatility may not be fully incorporated in the historical price moves."22

&nbsp;

The [NSCC]( https://www.investopedia.com/terms/n/nscc.asp) is now ~~strictly~~ using [historical volitility]( https://www.investopedia.com/terms/h/historicalvolatility.asp#:~:text=Historical%20volatility%20%20is%20a,in%20the%20given%20time%20period.)(HV) instead of both historical and IV to calculate a firm’s risk (*See Edit 1*). This allows them to perform more accurate VaR calculations. **It just got harder for firms to lie about the overall risk of their positions.**

&nbsp;

##2. The NSCC can pull funds from the Clearing Fund to help pay for a Member’s losses 2 business days after a [loss allocation notice]( https://www.sec.gov/rules/sro/nscc/2018/34-82428.pdf).

Under Section 6.4
> In order to be consistent with the language formulation set out in Rule 4, the proposed rule change would revise this sentence to state, “Losses charged to Members are required to be paid by Members on the second business day after the Corporation issues any such notice of a loss allocation charge and, if not timely paid by any Member, the Corporation may treat that Member as having failed to satisfy its obligation and apply the Clearing Fund deposit of that Member to satisfy its loss allocation obligation.”

&nbsp;

The NSCC will use the Clearing Fund to pay for losses (2 business days after a loss allocation notice) if a Member cannot. This amendment doesn’t really change things for us directly but after looking further into loss allocation notices I found that after the first issuance of a loss allocation notice one of two scenarios may happen. The Member either has:

- 2 business days until the NSCC pulls from the Clearing Fund (up to a loss allocation cap) to help pay off the Member’s losses and continue to send loss allocation notices until those losses are paid

OR

- 5 business days to notify the NSCC of its election to withdraw from membership which will limit their loss allocation exposure to their loss allocation cap (meaning they would only have to pay up to a certain amount once) **but they would no longer receive help from the NSCC or DTCC**.

&nbsp;

##What’s the point? Let’s circle back to the change regarding the VaR.

Remember how IV will no longer be used to calculate VaR? Back to Section 5.2.1:
> … the amount of Clearing Fund required from each Member is determined principally by Value-at-Risk (“VaR”) calculations

&nbsp;

So… If  the amount required relies heavily on the VaR and the NSCC is calculating VaR more accurately, Members with riskier portfolios who have been underreporting their risks and losses will have to pay more into the Clearing Fund because the new VaR calculations excluding IV will show higher risk numbers.

&nbsp;

##My theory:

**The NSCC will now be able to verify a Bear’s risk better through a more accurate VaR calculation which makes it harder for firms to fake their risk numbers. More accurate risk numbers will increase their deposit requirements into the Clearing Fund which leaves them with less available capital. Large short positions with less capital means more general risk and liabilities which further increases the deposit requirements. This compounding effect will lead to nonstop loss allocation notices which eventually forces the Member to either cover positions to help pay for loss allocations or pay their loss allocation cap and stop receiving help altogether from the NSCC and DTCC.**

&nbsp;

*Again, this is just what I got from the filing. I could be completely wrong. My brain hurts.*