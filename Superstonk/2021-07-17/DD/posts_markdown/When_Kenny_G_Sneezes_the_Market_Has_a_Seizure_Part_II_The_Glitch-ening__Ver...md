# Title: When Kenny G Sneezes the Market Has a Seizure, Part II: The Glitch-ening — Vertical lines in price charts are REAL TRADES outside the NBBO, HIGHLY CORRELATED across different stocks, and correspond to HIGH FREQUENCY and ALGO TRADING
# Author: G_KG
# Post URL: [https://www.reddit.com/r/Superstonk/comments/omegu8/when_kenny_g_sneezes_the_market_has_a_seizure/](https://www.reddit.com/r/Superstonk/comments/omegu8/when_kenny_g_sneezes_the_market_has_a_seizure/)


Gather round, apes and apettes, grab that vintage box of crayons you were saving for something special, and get comfortable.  Oh, first-   **HEY GABE!!!!**  [Gabe's been struggling lately-](https://finance.yahoo.com/news/melvin-t-shake-reddit-attack-205148761.html)

![I needed a reason to link this 100&#37; real completely non-satirical article from July 7th just one more time](https://preview.redd.it/84qap5rw1pb71.png?width=680&format=png&auto=webp&s=3b2b6f6b0fdf94547d6ca63ab14b5118cad9a50e)

Look at that beautiful, gaping mouth-hole.... srsly Gabe, open invitation to scour *my* message boards *any* time you want..... because this ***especially vicious*** reddit trader is about to get DOWNRIGHT SAVAGE...... with stats.  😮  🙈🙉🙊

First, what in the fuck am I talking about?  These little doodads that everyone keeps noticing-  credit to [u/shiftyasiankid](https://www.reddit.com/u/shiftyasiankid/) for grabbing the pic of GME's 3/10 flash crash from a rensole morning post-

![If I haven't gotten my point across, they're fucking everywhere.  GME's flash crash on 3\/10\/21 was especially fun!](https://preview.redd.it/bdjboz2jtpb71.png?width=1115&format=png&auto=webp&s=e1871f9a6b373d82cc33c7fd2b1af62afc2d2439)

Gabe's data scientist have given us ***all sorts*** of fascinating explanations for these lines *other* than "they're market sweep orders."  The first round has to do with some VERY fat fingers:

>1) Some trader fat-fingered their limit order    
>  
>2) Some broker fat-fingered the trade order

Ok seriously, trades are not performed by a bunch of monkeys in a back room, it's 99.9% electronic (unless you're one of those 0.1%'er shady fucks trading out of Philadelphia), and by the way you guys think about fat fingers *a lot.*  🍆    Also, even **IF** some poor ape did accidentally enter a limit order ***buy*** for $69,420.00, your broker is required by law (the Order Protection Rule) to buy your share at the ***National Best Offer****,* or the lowest ask $ available among all visible exchanges (what you see in the level 2 data).  

[If you want the gory details, they're discussed in here.](https://www.reddit.com/r/Superstonk/comments/ok1bta/the_intermarket_sweep_aka_the_straight_upanddown/)  Basically there are usually only 2 reasons that a trade can ever occur ***outside*** the bid:ask range (aka the national best bid/offer or NBBO):  1) ~~some high-frequency jackass submitted 1,000,000 trades in the same millisecond and~~  the computer system responsible for calculating the prices gets .... overloaded ....  for no particular reason ....   and trades are *not* canceled if it turns out they were outside the NBBO after the computer catches up ([~~this is called "quote stuffing"~~](https://www.investopedia.com/terms/q/quote-stuffing.asp) totally not something ***anyone*** would ***ever*** do on purpose).  OR, 2) the trade is marked with trade condition "trade-through exempt" or "611-exempt."  [Here's rule 611 from the SEC.](https://www.sec.gov/spotlight/emsac/memo-rule-611-regulation-nms.pdf)  As I understand it, the type of trade that is given most frequently given this status in U.S. markets is...

# The inter-market sweep, or sweep-to-fill order.

[Here's an ibrokers page that explains what the hell](https://ibkr.info/node/1734).  And if you prefer English to Engrish, [here's Investopedia on Sweep-to-Fill](https://www.investopedia.com/terms/s/sweeptofillorder.asp).  In summary, sweep-to-fill orders: a) value speed over price- the trader overpays when buying and undervalues when selling- just to get the order done quicker; b) are used **exclusively** by **high-frequency-traders and their trading algorithms,** and they happen very commonly; and c) just happen to show up in HUGE numbers during flash crashes.  [Sweeps are covered in FAR too much detail in this previous post](https://www.reddit.com/r/Superstonk/comments/ok1bta/the_intermarket_sweep_aka_the_straight_upanddown/), if you're wanting further info.  

Okay so back to Gabe's data scientists- this next batch of explanations has to do with the poor quality of our trading platforms because our plebeian asses can't afford a bloomberg-

>3) It's just a graphics glitch (***classic***)  
>  
>4) It's just carry-over from previous time and sales data points showing up under the wrong candle  (*uhm?*)  (*more code for lul @ ur poor-person's trading platform graphics glitch??*)  
>  
>5) It's just canceled trades showing up on your ~~dumb poor-person's~~ trading platform

Okay so no, no, and no, these trades are in the actual raw data and aren't designated as canceled, more on that below.  Sooooo.... nothing to do with any graphics effects.  The final round of explanations centers on data and data quality:

>6) Those are just smoothing errors from the UI  
>  
>7) Your ~~plebian~~ trading system is bad at averaging and spits out bad values  
>  
>8) Seriously your data must be bad somehow

So no and no, because I said *raw data*, meaning no smoothing or fuckery has touched it yet*.*  And to number 8.....   yea again ***no*** because ***raw data***.

SO LET'S TALK DATA!!  Who in the hell makes those numbers show up on our computers, anyway??  Well, the numbers are compiled by "Securities Information Processors" or SIPs from 6 main data feeds, depending on what exchange the stock is listed on. For **all NYSE-based stocks**, the publicly distributed data is managed by the [Consolidated Tape Assosiation](https://www.ctaplan.com/index) or CTA (yes that's what we need, MORE ACRONYMS):

![If you've got real-time data on a NYSE-listed stock, it's CTS data showing the price and CQS data showing the bid\/ask from the CTA and SERIOUSLY FUCK THESE ACRONYMS](https://preview.redd.it/hrvd35y3iqb71.png?width=858&format=png&auto=webp&s=e88816c0d689d5878701c369d4fe9b7e3055339c)

[Here's the wiki page if you're like me and need a REALLY SLOW explanation](https://en.wikipedia.org/wiki/Consolidated_Tape_Association).   [Here's investopedia to explain the same thing in a different way.](https://www.investopedia.com/terms/c/consolidatedtape.asp) Basically these SIPs spit out the price/bid/ask information for all our brokerage systems, and yes, ***if you live on planet Earth and use a display trading system with*** [real-time quotes](https://www.investopedia.com/terms/r/real-time-quote.asp)***, your brokerage firm is paying for access to THIS SAME data feed that we all see.***  Think about it logically- this is the only way that we can all trade, simultaneously, while still being protected by the "order protection rule" (making sure our trades land within the NBBO).  Don't argue with me, [argue with the SEC, and this VERY long National Market Systems rule](https://www.sec.gov/rules/final/34-51808.pdf):

https://preview.redd.it/acsyzlf4ttb71.png?width=813&format=png&auto=webp&s=37095105c455e708a941168a3ed43b5f004a41f7

If you saw that the pdf was 523 pages long and immediately shat yourself, I got you covered: [Reg NMS for dummies](https://www.nasdaq.com/articles/reg-nms-dummies-2019-05-09).  Reg NMS is actually the only reason CTA exists, see [this site explaining NYSE data feeds](https://www.exegy.com/2019/12/consolidated-tape-nyse-feeds/):

https://preview.redd.it/3c6836uxutb71.png?width=932&format=png&auto=webp&s=e61a259291924c38818888f93728647e28387a51

What does this mean?  

# It means the burden rests with exchanges and other "self-regulated organizations" to report accurate data to the CTA (including the price- CTS- and the best bid+ask- CQS).  

If you have a system that has access to the CQS and the CTS feeds ([real-time quotes](https://www.investopedia.com/terms/r/real-time-quote.asp) of [level 1 data](https://www.investopedia.com/terms/l/level1.asp)), ***that feed is correct by definition*****.**  If that data has weird prices looks fucky, ***it is not our fault as scientists and retail traders for having access to "bad" data, nor is it our responsibility to find "better" data to prove a point.***  This is the data that daddy SEC uses for Reg NMS, and exchanges are ***REQUIRED*** to report accurate information to ***IT.***  All of the "better data" that Gabe's data scientists keep talking about? ***It doesn't fucking matter to the SEC, so it doesn't matter to our research on strange prices.***  So what do you get when you pay for "better data?"  You get decreased latency, increased time resolution, and an expanded level 2 dataset.  From [Exegy explaining Consolidated Tape](https://www.exegy.com/2019/12/consolidated-tape-nyse-feeds/) again:

![I think 64 microseconds \(that's 0.0000064 seconds\) is OK for the level of stats I'm doing.  There's this thing called \\"significant figures\\" ... don't hurt your brain, Kenny](https://preview.redd.it/wi2g79gk6ub71.png?width=923&format=png&auto=webp&s=fe17f7e0b9ae68eeb4a9972b78e4dda4f85224f8)

It's level 2 data that starts to get expensive and varies in quality from place to place- from [Exegy explaining Level 2 market data](https://www.exegy.com/2019/03/level-2-market-data-what-level-supports-your-trading-strategy/)\-

https://preview.redd.it/lr2264k67ub71.png?width=939&format=png&auto=webp&s=53bc0dc7b45f82096fd774b6d5ecc4a7aba4840b

***Note that this data, level 2, doesn't matter one goddamn bit to determining whether a trade was placed at a price outside the NBBO.***  So yea, good level 2 data would be sweet and some day I'll get my hands on it, but it's **completely irrelevant to the vertical lines we are seeing = prices outside the NBBO = because that is ENTIRELY the realm of level 1 data.**

Okay so we're ABSOLUTELY SURE that Fidelity Active Trader Pro(r) gets VALID [REAL-TIME QUOTES](https://www.investopedia.com/terms/r/real-time-quote.asp) of [LEVEL 1 DATA](https://www.investopedia.com/terms/l/level1.asp)?

# Yes.

From a [love letter between Fidelity and the SEC](https://www.sec.gov/comments/s7-15-19/s71519-6526198-200427.pdf):

![That's some high-class pillow-talk right there](https://preview.redd.it/mq07i0aw8ub71.png?width=812&format=png&auto=webp&s=b99e5a6b2ac814cbf360edad0d747f3e13df0de5)

FUCKIN A' PETER, it's taken us LOTS OF READING and LOTS OF LINKS for VERY TENDER APE BRAINS up to this point to say with **FULL FUCKING CONFIDENCE** this **ONE SIMPLE FUCKING THING**:

# What you see with your eyes is real.  Seriously.

**(Btw...**  [**wut iz gaslighting???**](https://en.wikipedia.org/wiki/Gaslighting)**)**  

Okay, so.... where on your screen does this raw data live? [Level 1 data](https://www.investopedia.com/terms/l/level1.asp) dwells in the "[time and sales](https://www.investopedia.com/terms/t/time-and-sales.asp)" window on your platform.  [Level 2 data](https://www.investopedia.com/terms/l/level2.asp), if you have it, can be various places depending on your trading platform.  In fidelity, it's the directed trade window-

https://preview.redd.it/nr1tvumofub71.png?width=1552&format=png&auto=webp&s=460f837d5975862c76ff72ccd10238aab7d31c89

So if you're exporting data, and you do it by r-clicking one of the windows with RAW data, you .... uuhhh ....  get raw data.  How do I know that hedgies do NOT want you to know this??  *Because my materials and methods post on how to collect this data, including some sample raw data sets,* ***was marked as spam and made invisible by reddit despite being posted onto my OWN GODDAMN PERSONAL PROFILE PAGE***.  I seriously don't fucking know HOW your data scientists did it, Gabe, but I'm kind of impressed. Bravo.

# So THAT is where the data comes from, and there is absolutely NOTHING FUCKING WRONG WITH IT.   ahem.

And what does the data say about these vertical lines in our price charts?

# They are REAL trades occurring outside the NBBO called "market sweeps" marked* with trade condition: "trade-through exempt" or "611-exempt"

\*if you're rich enough to have a Bloomberg.  Only expensive platforms reveal or display sweeps because WHY TELL RETAIL TRADERS ANYTHING as always.  Result?  It's a SUPER common form of trading for high frequency and algo trading, but *normal retail traders tend to know nothing about them.*  And based on flurry of explanations offered by Gabe's data scientists, *they want to keep it that way.*

So let's get back to these straight lines!  The following chart displays REALLY CLEARLY where we're going to peek at the prices first.  (This stock tends to have sweeps show up *beautifully* on the price chart and is typically the first place I look to go "glitch hunting.")

https://preview.redd.it/zfqt8hsyiub71.png?width=521&format=png&auto=webp&s=6c66934d40eeab169028587ca1f8b8807c1a5a07

The glitch is SO strong with this one, that anyone navigating back to 7/13 after-hours right now will be able to see some of them.  (If you're now noticing that these sweeps seem to happen right around the *same time* nearly *every day* during *after-hours*....   stay tuned for future posts 😉 this one's too fuckin long already.)

So I peered into the data for this time period- 4:35 to 4:50pm on 7/13- and then decided to graph it for all my friends who don't read so well-

https://preview.redd.it/l2iknlwpkub71.png?width=1834&format=png&auto=webp&s=d4feb6d2ca1dbda2a3d2b106b0704270dc83e132

Those big green crayons?  All sweeps, corresponding to those pink dots (last price of the trade) wayyyyyy above the bid-ask range.   Did I mention something about a correlated pattern?  

**Here's GME for the same time frame**\-

https://preview.redd.it/zjq52z2zkub71.png?width=1848&format=png&auto=webp&s=0652e78e91997825713b3ae198123e6467bb99b8

Gimme some AAPL!

https://preview.redd.it/82evk8hhlub71.png?width=1837&format=png&auto=webp&s=6c938b8c3c3c051721d22d6d59989b986b72cc9b

Mix things up a bit with some TSLA!

https://preview.redd.it/2183rrnjlub71.png?width=1843&format=png&auto=webp&s=7570e6c8690bde7e6f9820c9d5eb62830b3d2b27

Go the OTHER DIRECTION (sweep to SELL!) with amazin' AMZN!

https://preview.redd.it/cg8xr8qolub71.png?width=1843&format=png&auto=webp&s=858289c07f4d86dabb810fc46b4f13224860b574

Come on back with a taste of MSFT---

https://preview.redd.it/c7vmpkaxlub71.png?width=1839&format=png&auto=webp&s=60f48497c01d4288ba84aac92fe0e81558a2ce5a

And then cleanse your pallate with NVDA before dessert--- 

https://preview.redd.it/nq8dccs4mub71.png?width=1840&format=png&auto=webp&s=77bac4135a9330808eba5b9ef57bb8598a1e77c0

Because to finish up I've got an ETF banana sundae for your pleasure...

&#x200B;

https://preview.redd.it/orfedhuamub71.png?width=1844&format=png&auto=webp&s=1d41bb2784465aa105ccbcb85d636cb681d778e7

And no....  I barely understand ETFs as it is....  I have NO idea how this works with ETFs, only that I made a pretty picture of it happening.  Wrinkle brains halp pls.

Is this the *FIRST* time that fucky data has been detected?  Noooope, I posted [these rantings of a stats and crayon-fueled lunatic](https://www.reddit.com/r/Superstonk/comments/n0a0hf/proof_of_artificial_price_movement_spreadsheets/) over two months ago, but didn't know what the fuck I was looking at.

Am I the *ONLY* person who has noticed all the insane crap in this data?  Nope, u/Pubertus posted [similar findings over two months ago](https://www.reddit.com/r/Superstonk/comments/n7ahcl/found_something_funky_on_the_dark_pools/?utm_medium=android_app&utm_source=share).  A HUGE number of trades priced OUTSIDE of the NBBO in an occurrence that was HIGHLY CORRELATED ACROSS MANY STOCKS.  

**This brain wrinkle has been forming for a LONG fucking time now.**

So I guess....  here, at the end of all things...  the only question that I ***still*** have, is....   

# HEDGIES, WHY ALL YOU MA'FUCKERS LYIN' SO MUCH ABOUT MARKET SWEEPS??

![dead. kittens. everywhere. LOOK AT WHAT YOUR DATA SCIENTISTS HAVE DONE, GABE](https://preview.redd.it/pfxghu9kyob71.png?width=638&format=png&auto=webp&s=b9d61d2a0dfb7d2c0820f94c6b4fcdefb2d68a1f)

# TADR: These bitches ain't glitches, "straight line thingies" are MARKET SWEEPS from HIGH FREQUENCY TRADERS and are HIGHLY CORRELATED across many stocks.  hi kenny 🤭  

Obligatory emojis: 🦧🦍🦧🐱‍👤💎🙌🚀🚀🚀🌙🖍🌌🍌

![ ](https://preview.redd.it/0dh1g19bqob71.png?width=1180&format=png&auto=webp&s=a5677bedb01128308e50ec49c1087287cfe39130)