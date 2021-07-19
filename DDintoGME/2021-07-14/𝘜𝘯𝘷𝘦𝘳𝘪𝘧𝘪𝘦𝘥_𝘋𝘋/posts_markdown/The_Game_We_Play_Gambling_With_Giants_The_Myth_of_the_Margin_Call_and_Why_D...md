# Title: The Game We Play: Gambling With Giants, The Myth of the Margin Call, and Why Dates Disappoint (Updated DD)
# Author: welcometosilentchill
# Post URL: [https://www.reddit.com/r/DDintoGME/comments/okixbv/the_game_we_play_gambling_with_giants_the_myth_of/](https://www.reddit.com/r/DDintoGME/comments/okixbv/the_game_we_play_gambling_with_giants_the_myth_of/)


**tl;dr -** *Due to a web of contracts and shared responsibilities, prime brokers are in a prisoner’s dilemma with GME shorts and are incentivized to keep short positions open to protect themselves against losses. By neglecting to raise rates and ignoring events of default, prime brokers can manage the fallout of these toxic assets by enabling a relationship of inaction; this makes it difficult to use metrics like FTDs for price forecasting. We are winning: buy and hodl.*

**This is not investment advice and references my opinion. Seek a licensed professional for investment advice.**

I’ve noticed some confusion over core concepts and relationships related to the institutional side of trading, so I set out to create a simple primer post. As I learned more about prime brokerage firms and their contractual agreements, I realized the margin call process is deeply misunderstood. No one seems to be talking about ***prime brokerage agreements*** or ***margin lock-up agreements***, which are both critical elements that impact how shorts are held accountable and to what degree.

**We have been repeatedly disappointed by forecasted dates and it’s my belief that understanding the above agreements will demonstrate how these predictions will never be reliable.**

&#x200B;

# Part 1: Meet The Players and Learn The Rules

## 1.a - Meet the Player: Hedge Funds

[Everyone’s favorite topic.](https://www.investopedia.com/terms/h/hedgefund.asp) You know what they are: a group of rich people pool money together to be managed by an investor. Hedge funds are notorious for utilizing aggressive investment strategies to secure high active returns. This is accomplished by multiplying a fund’s buying power through the use of margin accounts which allow for leveraged trading.

Margin and leverage are similar terms that are often found together, so for now understand that 1) margin accounts allow investors to make trades with credit, 2) margin is a form of collateral requested by the lender (cash deposited as insurance), and 3) leverage is a measure of credit utilization relative to deposited cash in their account (represented as a factor e.g.,10:1).

Think of a margin account as a credit card, but instead of having a credit limit that you pay towards, it's the inverse: you can only use a certain % of credit depending on how much money you have deposited into your account. In the above example, the money deposited into the account is the hedge fund’s “margin” and the amount they must deposit in order to use x% of credit is their “margin requirement”. Because requirements are measured as a percentage of value, brokers will require more margin to be deposited as the value of open positions (price of shares) rises. Similarly, because securities (or entire portfolios) can be substituted for typical margin deposits, if a hedge fund's portfolio starts to lose value they will need to deposit more margin. In short, it’s a balancing act.

**This post will be focusing primarily on short selling and, while other institutions can short sell, hedge funds are the most typical example.** [**For example, Citadel LLC is a multi-national hedge fund group.**](https://en.wikipedia.org/wiki/Citadel_LLC) **For the purposes of this post, assume that hedge funds = short sellers.**

## 1.b - Meet the Dealer: Prime Brokerages

[Prime brokerage firms are the middle man for big money bullshit.](https://www.investopedia.com/terms/p/primebrokerage.asp) Prime brokerage firms are commonly compared to regular brokerage firms (Fidelity, Robinhood, etc.) but for institutional investors. ***This is not an accurate comparison.***

Where a regular broker facilitates trades by matching buyers and sellers, [prime brokers function as *financing* firms.](https://www.investopedia.com/articles/professionals/110415/role-prime-broker.asp) In the past, hedge funds would utilize multiple brokerage firms to execute trades, so prime brokerages were created to route and clear these trades through a central broker. This meant hedge funds could manage finances through one firm instead of accounting for several. As time went on, prime brokers expanded their services to include margin and securities lending, trade settlement, execution of trades, and more. It should be noted that [there is significant competition between prime brokers](https://www.preqin.com/insights/research/blogs/what-makes-a-successful-prime-broker), which has resulted in more lenient rates and specialized services for clients. **Nowadays,** [**prime brokerage refers to a bundle of services**](https://primer.prooftrading.com/assets/pdf/03.05_participants_brokers.pdf) **provided by investment banks exclusively for hedge funds and other investment firms.**

Prime brokerage firms use two primary investment methods to make money: *rehypothecation* and *financing*. Rehypothecation involves re-using the collateral of a client to fund the broker’s own investments. Financing broadly involves using the value of one client's portfolio as collateral to raise cash which is then lent out to other clients for interest.

Prime brokers supply hedge funds (and other institutions) with additional cash to increase their margin and also supply shares for short-selling, with a specific talent for locating hard-to-borrow shares. [The importance of a prime broker's function as a financier cannot be overstated: **on average, 50% of hedge fund financing comes from prime brokers, of which 35% is extended on an overnight basis.**](https://www.sec.gov/files/2020-pf-report-to-congress.pdf) Additionally, modern prime brokers provide faster trade executions and clearing than traditional brokerages, which is one of the main reasons why high-frequency quant trading has dominated the market.

**So if you know nothing else, know this: hedge funds need prime brokers in order to be effective.**

## 1.c - Meet the Banker: Investment Banks

[Investment banks are the big money institutions who supply prime brokerage services for institutional investors.](https://www.investopedia.com/terms/i/investmentbank.asp)  In essence, they are large financial institutions that help high net worth traders access large capital markets. They include the likes of JPMorgan Chase, Credit Suisse, Wells Fargo Securities, and[ many more.](https://en.wikipedia.org/wiki/List_of_investment_banks)

They are different from commercial banks in that they do not directly provide business loans or accept deposits. Instead, they serve as intermediaries for large financial transactions, provide financial advice, and assist with mergers and acquisitions—oh, and they’re regulated by the SEC instead of the Fed.

If you’re concerned about the conflict of interest for a single institution to a) loan money through auxiliary services, b) provide investment advice to members, c) oversee mergers, acquisitions, and IPOs, d) are themselves divisions of larger orgs, e) exist to make profit for these larger orgs, and, f) facilitate short selling via rehypothecation of client portfolios, then you are not alone. But don’t worry, they’re expected to use a figurative [Chinese wall](https://www.investopedia.com/terms/c/chinesewall.asp) so that no two divisions can profit off of one another unjustly. [It works as well as you'd expect.](https://www.bloomberg.com/news/articles/2014-12-11/finra-fines-10-wall-street-firms-over-analysts-ipo-pitches)

**You should remember that they control the prime broker services and supply large sources of cash and equity for margin trading.**

## 1.d - Meet the Supplier: Pension Funds

When hedge funds want to short stonks, their prime broker finds a pension fund or mutual fund (oh fuck more funds). These funds function as massive stores of securities and have become the largest supplier of loaned shares in the market (especially pension funds). If the prime broker is lucky, the pension fund is already a client of theirs and they can freely loan out their shares and [pay them rebates on the interest they collect](https://www.investopedia.com/terms/s/stock-loan-rebate.asp)—otherwise they borrow directly from the pension fund for a nominal interest rate.

*Wait, my retirement fund may be shorting GME?* [Yep.](https://www.forbes.com/sites/edwardsiedle/2021/01/30/your-state-pension-is-unknowingly-shorting-stocks-like-gamestop-all-the-time/?sh=6cc2c3f4752d) Private pension fund managers are only beholden to their requirement to act as fiduciaries for their sponsors. There are no specific regulations in place to dictate investment strategy, though they traditionally invest in bonds, stocks, and commercial real estate.

But pension funds have not been doing well: at the end of its 2020 fiscal year, the [PBGC](https://www.pbgc.gov/) (insurance org for all private pension funds) [had a net deficit of $48.2 billion](https://fas.org/sgp/crs/misc/95-118.pdf) and the average state and local pension fund could only cover 70% of their sponsors. Oh, and [they grossly overestimate annual returns](https://www.pewtrusts.org/en/research-and-analysis/issue-briefs/2020/06/the-state-pension-funding-gap-2018) and, also worth mentioning, have been some of [the largest sellers](https://www.lohud.com/story/money/business/2021/01/28/gamestop-ny-state-pension-fund-sold-off-600-k-shares-last-10-months/4283205001/) of [GME shares](https://www.barrons.com/articles/giant-pension-sold-alibaba-palantir-gamestop--bought-zoom-retirement-51621348055).

So you can understand why these funds have been making riskier investments in search of higher returns (lending shares, derivatives, and investing in hedge funds).

**In our game, prime brokers borrow x amount of shares from a pension fund for a low interest rate, then lend them to hedge funds for a larger interest rate.**

## 1.e - Meet the Pro Gamers: Market Makers

While hedge funds are the focus of our twisted story, market makers are there to provide the initial stakes to gamble on through the facilitation of derivative trading. However, by definition, market makers are fairly simple.

[Investopedia defines market makers as:](https://www.investopedia.com/terms/m/marketmaker.asp)

>*a participant that provides trading services for investors, boosting liquidity in the market. Specifically, market makers will provide bids and offers for a security in addition to its market size.*

Many people think of the stock market as a trading house where buyers are instantly matched with sellers and stocks are exchanged for the current share price. *This isn't the case.* Instead, market makers facilitate trading for brokerages through their willingness to both buy and trade assets. Without this service, traders would have to wrestle with *liquidity risk*, which is the inherent risk of not being able to locate a counterparty to trade with. This is good; market makers fundamentally serve a good purpose in this bare-bones framework.

Also, [here are](https://www.jstor.org/stable/1341823) some [articles explaining](https://www.investopedia.com/terms/g/ghosting.asp) how [market makers](https://scholarship.law.stjohns.edu/cgi/viewcontent.cgi?article=3322&context=lawreview) make [money and](https://www.investorschronicle.co.uk/shares/2018/11/09/the-truth-about-market-makers/) how [some market](https://www.reuters.com/article/us-trading-markets-gaming/traders-manipulating-cheap-stocks-market-maker-idUSTRE68P27W20100926) makers [primarily serve](https://www.nasdaq.com/articles/5-market-manipulation-tactics-and-how-avoid-them-2018-04-11) their [own self-interest](https://www.tradersmagazine.com/xtra/payment-for-order-flow-is-undeniable-conflict-of-interest/) over [the interests](https://www.investopedia.com/articles/forex/06/ecnmarketmaker.asp) of [the market](https://www.forbes.com/sites/greatspeculations/2010/04/30/when-does-market-making-become-market-manipulation/?sh=1bcd99031e04).

## Market Makers and Derivatives

For our purpose, we want to focus on how market makers facilitate the trading of derivative contracts.[ Derivatives](https://www.investopedia.com/terms/d/derivative.asp) are securities contracts that derive their value from the price fluctuations of underlying assets (stocks, bonds, or commodities). Market makers serve a similar function by both creating and trading derivative contracts to boost the liquidity of the derivative market. Common derivatives include [option contracts](https://www.reddit.com/r/wallstreetbets/), swaps and futures.

**The derivative market is seriously fucked up:** the total notional value of the derivative market, which is the total underlying value of assets multiplied by associated leverage, is [**$582 trillion**](https://www.bis.org/publ/otc_hy2105.htm) (or more than [7 times the amount of total cash in global circulation](https://www.businessinsider.com/heres-how-much-money-there-is-in-the-world-2017-10)).

The value of the derivatives market is so incredibly high primarily due to leveraged trading, which is why hedge funds love derivatives. I don’t have much more to say about market makers, so [here’s an article detailing how derivatives are commonly used to hide short positions.](https://www.investopedia.com/articles/optioninvestor/09/naked-short-selling.asp)

**All you need to know about Market Makers is that they provide a way for hedge funds to gamble and cover short positions. For example,** [**Citadel Securities**](https://en.wikipedia.org/wiki/Citadel_LLC) **is a market maker.**

## 1.f - Setting Up the Game (A Recap)

* A hedge fund walks into the casino that is institutional trading and finds a table. They tell the dealer, a prime broker, that they want more casino chips so they can play high stakes poker with the big boys.
* The prime broker wants to make money off the game, so they go to the casino banker, an investment bank, and show the banker how many chips the hedge fund has already won and ask for a loan. The banker’s books look a lot nicer when their chips are loaned out (because of interest) so they happily loan the chips to the prime broker.
* The prime broker returns to the table with the extra chips and lends them to the hedge fund for a modest rate, but asks to hold some of the chips as collateral. Now that the hedge fund has lots of chips, they want to start gambling and ask the prime broker to deal them in.
* The prime broker goes to a pension fund, who manages the casino supply closet, and asks for a full deck. The pension fund lends the prime broker a deck of cards but charges some interest on it—mainly to ensure they’ll get the cards back.
* The prime broker goes back to the hedge fund and deals them a hand, but not before charging more interest than they are responsible for paying back to the pension fund (the house always gets a cut).
* A few market makers pull up to the table and start placing bets. The hedge fund waits for a nice looking setup and places a bet. The game begins.
* Oh fuck the hedge fund is broke.

## 1.g - Rules of the Game

You’ve probably seen margin calls described like this: a short seller borrows stonks and sells the stonks back to the market, hoping the price will go down. When the stonks go up in price, the broker who lent out the stonks margin calls the short seller and says, “pay up, Fucko". The short seller is broke and can’t post more collateral so they must buy shares to cover or else they'll be liquidated by the broker, who would then be responsible for buying shares.

This description may get the fundamental points across, but when talking about institutional trading this is akin to using a crayon to draft up architectural blueprints. In fact, it’s even worse than that. It’s just plain wrong.

&#x200B;

# Part 2: How the Game is Played

## 2.a - The Typical Borrower/Lender Relationship

[It has been confirmed that no DTCC members defaulted in January](https://www.reddit.com/r/Superstonk/comments/n6er77/holy_balls_from_the_dtcc_ceos_own_mouth_no_margin/), which seems crazy considering the $500 share price and rapid run up (note the post confuses a margin call with a default). This means that, despite the likelihood of brokers making margin calls, no shorts failed to post margin.[ While one short firm was saved by a $2.8B bailout](https://markets.businessinsider.com/news/stocks/steve-cohen-ken-griffin-invest-3-billion-gamestop-short-seller-2021-1), it's hard to believe that a 26:1 run-up wouldn't have caused at least one other DTCC member to default. To understand WTF happened in January, we need to understand the underlying principles of a borrower/lender relationship.

When a borrower asks for a loan, the lender must evaluate the short-term risk of the borrower defaulting on the loan vs. the long-term profit gained from interest. Likewise, a borrower must evaluate the long-term cost imposed by interest vs. the short-term value of the loan. This fundamental understanding creates a system of checks and balances that ensures both parties enter into a mutually beneficial agreement. When there is shared exposure to evenly weighted risks and rewards, both parties have reasonable assurance that the other will adhere to the terms of the loan and continue to act in the best interest of the borrower/lender relationship.

Let’s talk about that last part: *“both parties have reasonable assurance that the other will adhere to the terms of the loan and continue to act in the best interest of the borrower/lender relationship.”*

Imagine you are renegotiating a business loan with your bank after an unexpectedly bad quarter. Per the original terms, you risk missing payments and defaulting, which will expose you to a cascading effect of increased rates. The bank recognizes this and, since your credit and payment history is good, offers you a forbearance agreement that pauses payment until the next quarter. Even though the bank had no obligation to pause payments, this amended agreement serves the interest of the borrower/lender relationship because, 1) it’s more profitable for the lender if you finish paying off the loan than it is for you to go bankrupt, and 2) the lender can better secure the return of loaned assets through delaying payments, further reducing their risk exposure. **Both the borrower** ***and*** **lender have benefited more from acting in the mutual interests of the relationship, rather than had the lender acted only in self-interest.**

## 2.b - The Prime Broker Borrower/Lender Relationship

The lack of defaults in January makes more sense when viewing the prime broker as a *lender*. While prime brokers have a reputation for callously cutting off smaller defaulting funds, they seem to be much more risk-tolerant of bigger, more established funds with large diversified portfolios and access to robust alternative financing options (remember, prime brokers make most of their money through rehypothecation and financing).

However, unlike our bank loan example, securities loans don't have expiration dates and can remain open as long as margin is posted ([or the original lender requests their shares, which never happens](https://www.investopedia.com/ask/answers/05/shortsaleclosed.asp)). The longer that these positions remain open, the more profit brokers stand to make as they continue to reap interest. In fact, as financing organizations,  **prime brokers assume zero market risk from the underlying position of loaned assets**. Instead, they are only exposed to risk if a borrower defaults. Most importantly, because prime brokers continue to profit off of short-seller interest at a greater rate than what is owed to lenders, **prime brokers are exposed to less risk the longer a position remains open and have less incentive to raise collateral requirements (especially if it would interfere with payments).**

Even if prime brokers wanted to raise rates, it’s unlikely they could. *Wait...what?*

## 2.c - Rigging the Deck: Prime Brokerage Agreements and Margin Lock-Ups

You’ve probably heard before that Wall Street is competitive at the moment. [Nowhere is this more clearly seen than the competition between prime brokers.](https://finadium.com/the-long-and-short-of-us-prime-brokerage-pricing-in-2019/) When investment banks have [excess liquidity and interest rates are low](https://www.reuters.com/business/finance/tsunami-cash-is-driving-rates-ever-lower-what-will-fed-do-2021-06-03/), they are free to offer more competitive prime brokerage financing and amenities.

This increase in competition has had the notable effect of unbalancing the lender/borrower relationship by shifting more power into the hands of hedge funds (borrowers). Hedge funds are now empowered to negotiate for more lenient **prime brokerage agreements** and attractive **margin lock-up agreements** are more widely available.

Here's a random fact: the National Bureau for Economic Research estimates that, despite excess liquidity, [the six largest US banks can not withstand 30 days of a liquidity crisis](https://www.nber.org/system/files/working_papers/w28124/w28124.pdf) as caused by either[ deposit runs](https://www.forbes.com/sites/moneyshow/2021/07/13/easy-money-and-the-risks-of-inflation/), [loss of repo agreements](https://www.marketwatch.com/story/feds-reverse-repo-program-sees-demand-soar-to-just-under-1-trillion-overnight-11625079189), [prime broker runs](https://www.reuters.com/breakingviews/nomura-extends-prime-broker-woes-2021-07-07/), or [collateral calls](https://www.ft.com/content/267d00fb-f623-4850-a82b-4ef88a41d4b5). (*This means investment banks are overleveraged*).

Now back to our scheduled programming.

## 2.d - Prime Brokerage Agreement

[Investopedia again:](https://www.investopedia.com/terms/p/primebrokerage.asp)

>*A prime brokerage agreement is an agreement between a prime broker and its client that stipulates all of the services that the prime broker will be contracted for. It will also lay out all the terms, including fees, minimum account requirements, minimum transaction levels, and any other details needed between the two entities.*

At its base, this agreement exists as [a templated prime brokerage agreement ](https://www.sifma.org/wp-content/uploads/2017/08/Prime-Brokerage-_Prime-Brokerage-Agreement-Form-150.pdf)(which differs from broker to broker). A template agreement typically only requires the broker to extend financing on an overnight basis and gives the broker sole discretion to determine margin requirements. This means that a fund's broker can pull financing or significantly increase the manager’s margin without notice. Additionally, template agreements tend to provide brokers with broadly defined default rights against borrowing parties, which allows the broker to put a fund into default and liquidate their assets with considerable discretion.

These template agreements are *no bueno* for hedge funds, as being put into default can create a cascading effect for any other trade agreements that contain a [*cross-default provision*](https://content.next.westlaw.com/1-382-3377?__lrTS=20210110035720384&transitionType=Default&contextData=(sc.Default)&firstPage=true) ([ISDA](https://www.investopedia.com/terms/i/isda-master-agreement.asp) and repos). This is a common provision in trade agreements which states that when a party defaults on an agreement, it simultaneously counts as a default in other agreements—even third-party agreements.

Because of this, most hedge funds seek to negotiate the terms of a prime brokerage agreement. Depending on the pedigree of client, most brokers are fine with providing borrower-friendly amenities within the agreement. A prime broker's ideal client is one that uses generous amounts of leverage, employs a market neutral strategy, shorts hard-to-borrow stocks and has high turnover percentages (high volume of trades). [Quant funds](https://www.bloomberg.com/news/articles/2021-06-11/citadel-securities-settles-with-hedge-fund-over-secret-algorithm) are particularly attractive as they often execute trades directly through prime brokerages.

## 2.e - How Agreements Are Negotiated

## Financing Rates

On longs, a prime broker extends financing, thereby allowing a manager to “lever-up” its fund’s positions. The more leverage a manager employs, the greater the financing it needs. When lending, a prime broker will charge the fund an interest rate as follows:

* Interest rate = \[Benchmark rate\] plus a \[Spread\]
   * e.g.: = \[Overnight Bank Funding Rate (“OBFR”)\] plus \[35 basis points\]

On shorts, a prime broker lends the fund stocks, which the manager then sells in the market. The prime broker will charge stock loan fees, often expressed as interest earned on the proceeds generated from the short sales, calculated as follows:

* Interest rate = \[Benchmark rate\] minus a \[Spread\]
   * e.g.: = \[OBFR\] minus \[30 basis points\]

Funds are then charged [interest on open positions](https://www.tradingdirect.com/pricing/Interest-Rates) at a rate determined by the contract.

Negotiating financing terms is pretty straightforward: lower rates.

## Margin Requirements

Margin requirements are whatever is greatest between the *regulatory requirement* or the *house requirement*.

The regulatory requirement is the minimum margin required by regulation. In the U.S., the relevant regulation is either **Reg T:** 50% margin requirement of position, or **Portfolio Margin:** 15% margin requirement of portfolio. I’ll touch on the difference between these in section **2.l**.

The house requirement is the minimum margin required by the prime broker determined from a risk perspective. Essentially, brokers have their own proprietary ways of calculating risk for both individual positions and portfolios; if the house requirement overshadows the regulatory requirement, you pay more margin.

It’s also worth noting that many prime brokerage firms offer *cross margining* or *bridging*, which is the ability to cross margin cash products with synthetic products (e.g. cash equities with equity swaps), which can lower the overall margin requirement.

The SEC requires $500,000 of minimum net equity (comprised of cash and/or securities) to be deposited in a prime brokerage account, meaning brokers should have access to at least this much collateral at any given moment. Hedge fund managers commonly try to negotiate for this minimum to not be raised further. Similarly, prime brokerage accounts can be subject to other minimum requirements imposed by agreements outside of the prime brokerage agreement, such as an [ISDA master agreement.](https://www.investopedia.com/terms/i/isda-master-agreement.asp)

*Note: info from the above two sections was primarily taken* [*from this source*](https://hedgelegal.com/wp-content/uploads/2019/12/Prime-Brokerage-Agreement-Negotiation-Part-1.pdf) *(and checked with other sources).*

## 2.f - The Fine Print: Margin Lock-Up Agreements

Here’s where shit gets fucky.

In a competitive lending market, margin lock-up agreements are frequently offered as a way to entice prospective clients (note: margin lock-up agreements and prime brokerage agreements are **separate agreements**). [Here’s an example of one.](https://www.sec.gov/Archives/edgar/data/929351/000119312511272819/d237132dex2.htm)

Margin lock-up agreements lock-in a prime broker’s margin requirements for anywhere between 30-180 days based upon the client’s credit history and the riskiness of the position. The lock-up prevents the prime broker from altering pre-agreed margin requirements or margin lending financing rates, or demanding repayment of margin or securities loans or any other debit balance. Effectively this means that, should a hedge fund’s position change and the prime broker would like to implement a stricter margin requirement, the prime broker is contractually obligated to give the hedge fund x days' notice. Within this period, the broker cannot demand any repayment—so no interest or returned shares. This is big, as [funds also pay interest on margin debit.](https://www.investopedia.com/ask/answers/07/margin_interest.asp)

Now remember when I said that there’s a lot of competition between prime brokers? It’s typically not in the broker’s interest to actually impose an adjusted margin requirement. Instead, these lock-up agreements function as a 30-180 day notice period for hedge funds to adjust portfolios to fit within the original margin requirement. Actually imposing an adjusted margin requirement is considered detrimental to the business relationship and will prompt the hedge fund to take their business to a more lenient broker. This has the added adverse effect of impacting the broker's reputation amongst other clients.

## 2.g - Margin Lock-Up Termination Events

[Termination events are clauses that allow the prime brokerage to terminate the margin lock-up agreement and adjust margin requirements as needed.](https://hedgefundlawblog.com/prime-brokers-margin-lock-ups-hedge-funds.html) Typically these events include net asset value decline triggers or a removal of key persons. It’s also important to note that these margin lock-up termination events apply specifically to margin lock-up agreements, and not the prime brokerage agreement as a whole. So if a hedge fund pulls something shady, the prime broker reserves the right to terminate the lock-up agreement (but this doesn't mean they will necessarily have the right to terminate the prime brokerage agreement).

## 2.h - Terminating a Prime Brokerage Agreement Without Cause

Now let's talk about how a prime broker could terminate the overarching prime brokerage agreement. There are two types of termination: *without cause* and *with cause*.

Either party can terminate the prime brokerage agreement without cause, meaning at any time the hedge fund or prime brokerage can decide to stop doing business with the other for no stated reason. However, a prime broker must usually give a notice period before terminating the agreement, which is often the same period as the margin lock-up period. Because of this, bigger hedge funds often have multiple brokerage accounts with different brokers, should they ever need to transfer balances.

## 2.i - Terminating a Prime Brokerage Agreement With Cause (Events of Default)

Since margin lock-ups fundamentally increase a prime brokerage’s exposure to risk, the broker tries to include as many fail-safes in the prime brokerage agreement as they can. These fail-safes are commonly called termination events (not to be confused with the aforementioned margin lock-up termination events) or [*events of default*](https://www.investopedia.com/terms/e/event-of-default.asp), and allow the broker to terminate the contract with cause.

Hedge funds want as few events of default included in their agreement as possible because, when triggered, they give brokers the power to take control of a hedge fund’s account (usually for liquidation). Notably, this power is used sparingly. If a contract is terminated with cause, the hedge fund has seriously fucked up or the market is crashing.

Common events of default include: failure to pay or deliver, non-payment failures, adequate assurances or material adverse change provisions, and cross-defaults.

Last thing to note is that most of these agreements contain something called a [fish or cut bait](https://jollycontrarian.com/index.php?title=Fish_or_cut_bait) provision, which is akin to a statute of limitations. If an event of default occurs, this provision states that a prime broker has x days to act on it or else they waive the right to act on it.

Info regarding the above two sections is primarily taken [from this source.](https://hedgelegal.com/wp-content/uploads/2019/12/Prime-Brokerage-Agreement-Negotiation-Part-1.pdf)

## 2.j -Termination Events vs. Events of Default

Wait, aren't these terms used interchangeably? Yes, in general application they can mean the same thing. However, there are some nuanced differences, explained [in this white paper (p.6)](https://www.kramerlevin.com/images/content/4/2/v4/427/HFLR-Best-Practices-for-Hedge-Fund-Managers-When-Entering-into-ISDAs-Negotiating-Callat.pdf):

>*Events of default were historically viewed as circumstances where the defaulting party was to blame, while termination events were viewed as something that happened to the affected party. While triggering an event of default or termination event tend to lead to the same end result – the ability of the non-defaulting party to early terminate and employ close-out netting – there are three key differences under the Master Agreement, explained Rimon Law partner Robin Powers:*  
>  
>*1. An event of default will result in the early termination of all transactions, whereas certain termination events only result in the early termination and close-out of affected transactions.*  
>  
>*2. Under the 2002 Master Agreement, a party is required to notify the counterparty when it experiences a termination event but not an event of default.*  
>  
>*3. Section 2(a)(iii) of the Master Agreements makes it a condition precedent for the non-defaulting party to continue to make payments on transactions for which no event of default has occurred and is continuing. A similar condition precedent does not exist with respect to termination events*

I'll touch on this more in the comments, but just know that these differences affect who is responsible and/or obligated to close out, notify, and make payments on transactions post-default. It's also worth noting that this white paper is specifically discussing **ISDA master agreements**, which is an adjacent agreement that influences the prime brokerage agreement.

## 2.k - ISDA Master Agreement vs. Prime Brokerage Agreement

Published by the [International Swaps and Derivatives Association](https://www.isda.org/), ISDA master agreements specifically dictate terms that govern over-the-counter (OTC) derivative transactions. 

Unlike a prime brokerage agreement, which can vary widely from broker to broker, ISDA master agreements are standardized. These preprinted forms are signed and executed without modification, while a second "schedule" document houses any negotiated amendments. Finally, a third contract is added to the mix called a Credit Support Annex (CSA), which outlines collateral arrangements between the two parties. In most cases, all three contracts fall under the *ISDA master agreement* moniker.

What’s important about ISDA agreements is that they are negotiated in a considerably similar fashion to prime brokerage agreements, using identical language, identical provisions, and serving near-identical purposes. This is great, as there are more publicly available resources and insights available for ISDA agreements than for prime brokerage agreements and these insights are largely transferable between the two—especially with respect to how margin is treated.

## 2.l - Margin Calls: Initial Margin vs. Maintenance Margin

While margin lock-up agreements require 30-180 days' notice prior to a given margin rate increase, it does not protect against minimum *maintenance margin* requirements.

**Initial Margin:** the collateral that must be in your account to open a position. Looking back at our base minimum regulatory requirements for stock markets, **Reg T** establishes that initial margin must be 50% of a position's value.

**Maintenance Margin:** supplemental margin needed to maintain an open position. **Reg T** establishes this as a minimum of 25% of the current value of a position.

**Reg T vs. Portfolio Margin:** created as a response to the Crash of 1929, Reg T has been around for a *long* time and had little in the way of changes (its margin rate was last adjusted in 1974). Because of its age, Reg T is incredibly simple: 50% initial margin, 25% maintenance margin, and every position is financed separately. [Finalized in 2008](http://www.themargininvestor.com/regulatory-timeline.html), [**portfolio margin**](http://www.themargininvestor.com/portfolio-margin-101.html) is the hot younger sister of Reg T and provides an alternative method of margin financing based on the estimated risk of a portfolio. With portfolio margining, initial margin and maintenance margin requirements are the same and also considerably smaller (between 8 - 15%). Funds are given the option between the two systems; most opt for portfolio margin.

Regardless of which system they use, **whenever the price of a shorted security goes up, margin must be deposited based on whatever the agreed upon rate is.** A failure to maintain appropriate margin results in a [margin call](https://www.investopedia.com/terms/m/margincall.asp). Failure to post margin within two to five days of a margin call results in an event of default.

## 2.m - What Happens When A Hedge Fund Defaults?

Once a default occurs, the prime broker has the power to liquidate a fund’s portfolio ([here are some fun example default clauses](https://www.lawinsider.com/clause/investor-default)) or, at least, close out positions in default. Notably, the prime broker doesn’t have to act upon an event of default and can simply ignore it. Regardless, hedge funds typically require a notification requirement and a default and remedies clause. We’ve already discussed notification requirements, so let’s cover the default and remedies clause. This fairly standard clause states that any private sale using their liquidated assets should be done in good faith and not unjustly benefit competing firms or entities. [This article explains more about liquidation, albeit from a voluntary perspective.](https://www.eisneramper.com/bakker-hedge-ai-blog-0920/)

&#x200B;

# Part 3: What's Next?

## 3.a - Wrap Up

If it isn't obvious yet, prime brokers are incentivized to keep margin rates manageable for clients as long as they have reason to believe their client can continue to make payments. While they have the option to increase rates, it's often not in their best interest to exert additional pressure on a borrower (nor is it easy to do). Prime brokers and short sellers have found themselves in a prisoner's dilemma where, as long as everyone is making payments and nothing moons, the situation is at least manageable. The critical issue is that for a prime broker to enforce their right to amend the situation, they have to assume the responsibility of closing out open positions and—with only the client's portfolio to help cover—could find themselves footing the bill for massive losses. Depending on the size of a given position, this could be a large enough loss to bankrupt a major institution.

With the deck rigged, the situation can seem daunting—but it’s important to remember that the fundamental game hasn’t changed: whoever is short on GME is juggling a losing position. At this point, we are watching these bad bets get shifted from player to player and they are bleeding out at every ante. **the difference in magnitude of market cap between a $4 and $200 share price, and a $200 and $1000 share price is massive. Literally by a factor of 45 (50-5).**

One thing we *should* take away from all of this is that, while clusters of dates can provide good general estimates and support pattern analysis, **we should avoid forecasting dates or using specific dates as indicators.** As shown by the sheer flexibility of these confidential agreements and the impetus for brokers to not enforce their own terms, retail traders simply do not have access to enough information to accurately anticipate institutional responses.

Instead, let’s keep in mind that buying momentum with GME has remained high since Jan, OBV trend is solid, the price floor is higher making it increasingly hard to drive the price down, the abundance of liquidity in the market is a greater risk to institutional investors than retail, the regulatory changes support retail, GameStop has no debt, $1bn+ in cash, and a leadership team driving significant industry-leading initiatives. **Shorts have to cover: buy and hodl.**
(more DD in comments)