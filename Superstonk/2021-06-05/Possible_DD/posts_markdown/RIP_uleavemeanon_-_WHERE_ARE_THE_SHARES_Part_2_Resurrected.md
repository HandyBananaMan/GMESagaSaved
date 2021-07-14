# Author: VoxUmbra
# Post URL: [https://www.reddit.com/r/Superstonk/comments/nt8qzj/rip_uleavemeanon_where_are_the_shares_part_2/](https://www.reddit.com/r/Superstonk/comments/nt8qzj/rip_uleavemeanon_where_are_the_shares_part_2/)


[\[Part 1\]](https://www.reddit.com/r/Superstonk/comments/nt8ot8/rip_uleavemeanon_where_are_the_shares_part_1/)

[\[Part 3\]](https://www.reddit.com/r/Superstonk/comments/nt8t9n/rip_uleavemeanon_where_are_the_shares_part_3/)

&#x200B;

Hi all,

There were a lot of apes in the daily discussion thread wondering why the DD by [/u/leavemeanon](https://www.reddit.com/u/leavemeanon/)  was gone. Turns out they've deleted their account for some reason,  along with their posts. I did a bit of digging and managed to recover  their posts (shoutout to [https://camas.github.io/reddit-search](https://camas.github.io/reddit-search)), which I'll be shamelessly reposting as there seems to be some demand:

&#x200B;

https://preview.redd.it/pbclog2zbj371.png?width=800&format=png&auto=webp&s=6c8fe49a4a3fb88e4e1fb98b9160acf4c39ef473

So, without further ado:

&#x200B;

\-----

&#x200B;

## Acronym Index and Glossary

Because I always wish the SEC included these, for the Fed if nothing else

**ETF** \- [Exchange-Traded-Fund](https://www.investopedia.com/terms/e/etf.asp) \- Simply put, ETFs are a hybrid between funds and stocks. They, like any fund, hold some portfolio of securities. And like any stock, they trade as shares on open exchanges. For example, SPY is an ETF with a portfolio designed to mimic the S&P 500 index.

**NAV** \- [Net-Asset-Value](https://www.investopedia.com/terms/n/nav.asp) An ETF’s NAV is the value of the funds assets, minus liabilities. Regarding ETFs, the NAV is the value of the underlying, as opposed to the trading price of ETF shares.

**FTD** \- [Failure-to-Deliver](https://www.investopedia.com/terms/f/failuretodeliver.asp) \- after the sale of a security, the seller (believe it or not) has 3 days to deliver the security to the buyer, otherwise the share is deemed failed-to-deliver - a FTD.

**AP** \- [Authorized Participant](https://www.investopedia.com/terms/a/authorizedparticipant.asp) \- “An authorized participant is an organization that has the right to create and redeem shares of an exchange traded fund (ETF)….When there is a shortage of ETF shares in the market, authorized participants can make more. Conversely, authorized participants will reduce ETF shares in circulation when the price of the ETF is lower than the price of the underlying shares. That can be done with the creation and redemption mechanism that keeps the price of an ETF aligned with its underlying net asset value (NAV).”

**MM** \- [Market Maker](https://www.investopedia.com/terms/m/marketmaker.asp) \- Market Makers, very generally, oversee markets and quote bid/ask prices to create a spread. They stand ready to buy or sell in their market, and they have algorithms coded to hedge these transactions and profit from arbitrage along the way.

**HFT** \- [High-Frequency Trading](https://www.investopedia.com/terms/h/high-frequency-trading.asp) \- “High-frequency trading, also known as HFT, is a method of trading that uses powerful computer programs to transact a large number of orders in fractions of a second. It uses complex algorithms to analyze multiple markets and execute orders based on market conditions. Typically, the traders with the fastest execution speeds are more profitable than traders with slower execution speeds…In addition to the high speed of orders, high-frequency trading is also characterized by high turnover rates and order-to-trade ratios. Some of the best-known high-frequency trading firms include Tower Research, Citadel LLC and Virtu Financial.”

//

## TLDR:

Various “financial instruments” can be combined to create *synthetic* positions. These often include options, and, with respect to the positions they aim to “synthesize”, they are frequently cheaper and carry the benefit nondisclosure. [This SEC risk alert from 2013](https://www.sec.gov/news/press-release/2013-151) discusses the potential for the combination of ‘profit and nondisclosure’ to promote dishonest (and possibly fraudulent) bookkeeping. This post discusses these positions, the bookkeeping tricks, how hedging is involved, and how it might all relate to GME.

If you like taking things apart to see how they work, you’re in the right place. If you prefer to throw things at the wall to see how they break, the final chapter should be done in a day or two. It’s the coolest, imo

## A Step Back

This post contains the second of 3 chapters. [**Chapter One, on ETF arbitrage**](https://www.reddit.com/r/Superstonk/comments/nplv75/where_are_the_shares_a_beginners_guide_to_hiding/?utm_source=share&utm_medium=ios_app&utm_name=iossmf), discussed AP’s crucially important role in supplying market liquidity, their reliance on ETFs to fulfill this role, and the **20 million share tip of the Glacier** that merely the *reported* ETF shares outstanding represent.

It was technical and complicated, I know (there were some fantastic questions in the comments, however, so keep em coming). Unfortunately, this post, too, is technical and complicated. And long. Imo, I *have* to start with the boring stuff, because, frankly, the *very fact* that it is so boring is partially what makes it so dangerous. Chapters One and Two examine the moving parts. Chapter 3 will zoom out and look at the whole machine.

To be clear, I am *very intentionally* presenting the information in this specific order - from granular to grand. *Everyone* knows something is wrong when you see smoke, but to truly understand the problem, you *must* try to understand the moving parts. Otherwise, when the machine’s owner shows up and says - *ehh, it was steam* \- you might go back to work and end up smelling like smoke for 6 months. Or worse.

Keeping that in mind, I hope you stick with me - it will make sense in the end.

//

If you grudged through [**Chapter One**](https://www.reddit.com/r/Superstonk/comments/nplv75/where_are_the_shares_a_beginners_guide_to_hiding/?utm_source=share&utm_medium=ios_app&utm_name=iossmf), hopefully you got a sense of how APs oversee the markets like a referee, moving shares from ETFs into securities (and vice versa) to meet demand wherever it shows up. [**This post, by u/made\_thisforhelp**](https://www.reddit.com/user/made_thisforhelp/comments/nqq7t6/response_to_uleavemeanon/?utm_source=share&utm_medium=ios_app&utm_name=iossmf) brilliantly explains this process with a simple example.

APs have a responsibility to meet increases in buying or selling pressure via so-called *liquidity provision* mechanisms, and, “Traditionally, authorized participants are large banks, such as Bank of America (BAC), JPMorgan Chase (JPM), Goldman Sachs (GS), and Morgan Stanley (MS).” - Investopedia.

Citadel Securities, LLC is *also* an AP in many markets, and before discussing them further, I think it’s **vital** to consider them in light of a few important facts -

1)Citadel Securities takes pride in being able to “provide continuous liquidity - every second of every trading day.” per their founder. They take this responsibility very seriously, and through arbitrage, it is *extremely* profitable for them.

2)Citadel Securities is among the largest, if not [**THE largest**](https://www.insidermonkey.com/blog/10-biggest-hft-firms-in-the-world-586528/?singlepage=1) HFT firm in the world. They handle that remarkable volume with lines of code stuffed into black boxes - stacked by the thousands in some data center - monitoring exchanges around the world and trading in microseconds to net pennies on price discrepancies through arbitrage.

3)Liquidity provision (the providing of liquidity) regulations were written by the SEC, and I *highly* doubt that all of the provisions (*and* their amendments) were proposed internally. It is far more likely that big banks (who had watched Citadel do this for years before the SEC gave in and let them have HFT desks) and Citadel suggested the changes be made to improve their *beloved* liquidity power. Naturally, they omitted the ‘free money’ part.

To be fair, I don’t know wether the SEC was complicit with, or ignorant to, the implications that this level of control over liquidity provide. Either way, Citadel is **not** just Ken standing on a balcony and yelling out trades. A “citadel” is, by definition, a *fortress* \- in this case the fortress is some data center. **They make money by filling your buy order with a cheaper version of whatever you’re buying.** That *is* arbitrage: buy low, sell high.

These facts are important to consider in unison. When buyers flood the markets - arbitrage provides a profit opportunity, HFT is designed to seize that opportunity as many times as possible, and the SEC calls that opportunity a *responsibility* in the name of providing liquidity.

In practice, when liquidity is needed, the black boxes monitor markets and look for arbitrage profit opportunities. **This is what the black boxes are told to do.** My last post discussed one of these opportunities via ETF creation/redemption, and here I discuss another: options.

# Chapter Two: Options and Hedges

## The 3 Levels

If you read the intro, I apologize for rambling on about Citadel but this is why I did it -

We’re about to get down and dirty and it might get dense pretty quick, so while you’re flexing that wrinkle try to pretend you are *the eye of Citadel* \- an etherial codebender controlling a Market Maker, Authorized Participant, and the biggest, fastest HFT firm on the block - you oversee the markets, create the spreads, and distribute liquidity where its needed - all the while looking for split-second arbitrage opportunities to profit from.

Also some of you apes are probably levels beyond this stuff so read (or not) as you please

## Level 1

A single options contract has a value, called a premium, that is derived from the price movements in some security. Options are bets for/against a stock’s trading price to reach some **strike price** by a set expiration date. You can bet it’ll go up (call) or you can bet it’ll go down (put). Note though - these are *contracts*, not stocks - they have an assigned expiration date and their ownership is **bilateral**, meaning every contract, until settled, represents **open interest** between the two parties.

Specifically, a **call** option is the right to *buy* 100 shares for the strike price and a **put** option is the right to *sell*\* 100 shares at the strike price. And because these are contracts, positions can be opened by buying *or* selling a call *or* put.

Those are the four trades in Level 1 of this hierarchy I just made up. Buy/Sell a Call/Put.  It’s the most innocuous level, yet its important. Consider *selling* a call - the buyer owns the right to buy 100 shares, meaning you have an *obligation* to deliver those 100 shares.

Some traders mitigate the risk of this obligation by “covering the call”, leading me to -

## Level 2

[**“Covering a call”**](https://www.tastytrade.com/definitions/covered-call) is a hedge against the sale of a call. A simple example to follow will make this smoother -

Call seller (S) simultaneously sells a call for XYZ and buys 100 XYZ shares. This way, S can deliver the 100 shares if the call buyer (B) exercises the call option.  If B does *not* exercise the call because the price of XYZ fell, S sells the XYZ he bought to “cover” for a net loss (that is equal to the premium he received for selling the call.

(( Note that the *premium* B payed for the option is calculated such that this “covered call” position is perfectly hedged. ))

In English, options can be hedged with shares. In fact, [**delta-gamma hedging**](https://www.investopedia.com/terms/d/deltagamma-hedging.asp#:~:text=Delta-gamma%20hedging%20is%20an%20options%20strategy%20that%20combines,refers%20to%20the%20rate%20of%20change%20of%20delta.) is common Market Maker practice.

P.s.) if you’ve ever heard the term “gamma squeeze”, this is what the “gamma” refers to. Rapid call buying **forces** Market Makers to buy shares to hedge, and the buying pressure forces the price up. P.s.s.) Calls *expiring* ITM/OTM, as far as I understand, shouldn’t really matter unless those investors are buying more calls to extend their position, or… the marker maker is a little late on hedging..

Level 2 is the bilaterally hedged option - using (s) to hedge position (L) or vice versa

Buying calls is a long position (L), its bullish. Thus, selling calls is a short position (s).

Conversely,

Buying puts is a short position, its 🌈🐻ish. Thus, selling puts is a long position.

The nature of the options position (L)/(s) determines the nature of its hedge, and the hedge can consist of a (L)/(s) trade in the security *or* the option.

For example, S sells *puts* (L) on XYZ. He can hedge this position by shorting x number of XYZ shares (s), selling XYZ calls (s), or buying XYZ puts. The *degree* of the hedge would depend on the strike prices (or x).

Market Makers are constantly hedging against options trades. Its another responsibility they enjoy. Because, through arbitrage, any trade they’re responsible for is a potential profit opportunity.

The essence of hedging is combining a long position with a short position. Well that’s pretty broad so let’s step it up a notch to -

## Level 3

The compound hedges. The synthetic positions. If you’re still reading after that last section, I’ll just save you the headache on this one.

Just know a few things. Generally, that (L) hedges (s) and vice versa - and (L)/(s) could be any combination of options, equities, etc. Also, “synthetic positions” mimic the risk profile of other positions, and creating a synthetic position is often cheaper than closing a real one.

Oh and one last thing, \*\*[any shares CLOSED FUNDS use for hedging are NOT reported, as of July 1, 2000](https://www.sec.gov/news/press-release/2018-291).

Naturally, it’s in the fine print at the bottom. [**This article**](https://capitalmarkets.lockelord.com/2019/01/02/secs-new-rules-on-hedging-disclosure/) discusses, however:

“The SEC excluded closed-end funds from the requirements of Rule 407(i). It noted that the **special structure**, **regulatory regime** and **disclosure obligations** of registered closed-end funds **makes the new disclosure requirements less useful to fund investors**.”

lol how dare disclosure and regulation made something less useful

“In addition, the SEC noted that the **compensation scheme** often associated with closed-end funds is either inapplicable to the new disclosure requirements (as shares are not typically a component of incentive-based compensation), or if compensation does occur in the form of shares, it is often difficult to hedge these shares. Thus, Congress’ concern about the undermining of the objectives of long-term compensation through hedging is unlikely to be raised in the case of closed-end funds.”

Not sure what the “compensation scheme” was/is, but I’d guess it’s either [**front running**](https://www.investopedia.com/terms/f/frontrunning.asp#:~:text=Key%20Takeaways%201%20Front-running%20is%20illegal%20and%20unethical,reasoning%20behind%20it.%20Transparency%20and%20honesty%20are%20key.) with HFT or the arbitrage/liquidity provision stuff.

Oh, and unless the big banks swallow the profit and file their HFT trading desks as separate, closed funds - there’s only one big league AP with a closed fund: Citadel Securities.

## Here They Are

If, like me, you’ve lurked on r/superstonk for a while, you probably remember seeing some stuff about some weird puts or something. I can’t see into the past, but we can try to break things down a little -

[**GME options data**](https://www.barchart.com/stocks/quotes/GME/options) is.. well, just go look at it.

I’ve been watching it for a while and I can tell you - there are far more expiration dates  (potential contracts) right now than there were 3 weeks ago. The suspicious dates, however, are **7/16** and **1/21/22**.

The open interest (OI, total number of contracts yet to be settled) for puts expiring on those two dates is over 650,000. Multiples of other dates.

Even weirder, almost 350k of that OI is at $0.50 and $1.00 strike prices. Those strikes prices **don’t even exist** on any other dates.

*So what can this mean?*

Who tf knows. It is really weird, I’ll say. I mean, can those puts even *be* relevant at $0.50?…

//

Well, [**this SEC risk alert from 2013**](https://www.sec.gov/news/press-release/2013-151) discusses one way they could be. **This is highly speculative**, but, I think, worth mentioning.

That document discusses two (illegal) practices in regard to covering short positions with options. **Buy-Writes** and **Married-Puts**.

Apes sniffed Buy-Writes out pretty quick, which I’d imagine pissed somebody off beyond belief. The Buy-Writes were those deep ITM calls that were executed immediately, and they functionally serve to rent the Market Maker’s 35 day FTD extension to some firm that was short.

The FTD settlement dates are reviewed in that document, too - T+3,6 or 35 calendar days. But I just wanna note, directly after a social media avalanche and GME on the news everyday, whoever (Citadel or not), was conducting those Buy-Writes either has titanium balls or is painfully desperate. I mean I found that at the top of the search page.

So Buy-Writes are sneaky-ish and add 35 days, but **Married Puts** work slightly differently. From what I can tell, they’re less honest, harder to prove, and can roll FTD’s over indefinitely. Yeah…

To prevent a FTD, a firm buys a put (s) *and* XYZ shares (L) to hedge. The firm uses the XYZ shares to settle the fail, but on the books they’re still marked as **married** to the put. The firm can then sell the shares (again), keep the put, and maintain the short position until the puts expire.

This leaves the put behind, though. So could those 350k cheap puts be *divorced* puts?

I kinda doubt it, but barchart let’s you see each contract’s price history, and I think it’s worth mentioning that over half of those 350k puts at $0.50/$1.00 were purchased between Jan 24 and Feb 2. And these worthless puts *increased* in price by up to 1000% during that time.

That’s a lot of demand for worthless puts, and considering the only real function of the *put* in Married-Puts is a placeholder to prevent a FTD - if I were short 100 million GME shares, I might buy as Married-Puts as I can, as cheap as I can, just so I can resell the shares and prevent the losses.

Also, “put options can be extended very cost-effectively. If an investor has a six-month put option on a security with a determined strike price, it can be sold and replaced with a 12-month put option with the same strike price. This strategy can be done repeatedly and is referred to as rolling a put option forward.” - ![**Investopedia**](https://www.investopedia.com/articles/optioninvestor/07/affordable-hedging.asp)

For this reason (and this is highly speculative), the high activity on puts at such low, OTM strike prices, could suggest involvement in a larger open position. Possibly a position from years ago, when some group of people thought they could profit from selling 35 million GME shares at 50 cents each.

Honestly I’m not sure, and I don’t think it matters all that much.

Don’t forget that a share recall sucks everything back in. All the IOUs, the positions rolled forward, the shares re-re-reborrowed…

You know, when I started down this rabbit hole, I thought the best answer to the question would be some complicated formula or 300 page document. I no longer think this. These detailed hiding places show that it’s *possible* to hide shares. All I’ve done is confirm what you already know - they can put shares wherever they please and never tell anyone.

In fact, that *is* liquidity. Credit. Flexibility. That’s why, I think, the answer to the problem may have looking us right in the face since January.