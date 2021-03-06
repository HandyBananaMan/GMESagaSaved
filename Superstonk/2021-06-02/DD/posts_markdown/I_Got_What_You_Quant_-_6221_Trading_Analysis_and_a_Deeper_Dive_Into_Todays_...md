# Title: I Got What You Quant - 6/2/21 Trading Analysis and a Deeper Dive Into Today's Tape
# Author: myplayprofile
# Post URL: [https://www.reddit.com/r/Superstonk/comments/nqzo1o/i_got_what_you_quant_6221_trading_analysis_and_a/](https://www.reddit.com/r/Superstonk/comments/nqzo1o/i_got_what_you_quant_6221_trading_analysis_and_a/)


HOLY MOLY! GME has highest close since 1/29! If you haven't seen yesterday's [POST](https://www.reddit.com/r/Superstonk/comments/nq5xf8/612021_trading_deeper_dive_into_the_tape_and/?utm_source=share&utm_medium=web2x&context=3), I recommend taking a look before getting into today's action, because **BIG THINGS ARE HAPPENING!** Congrats to the 💎🖐🦍 that like movies, as without you, GME wouldn't be on the brink of launch. Prepare yourself, it's time for the tea. This is not financial advice, my 🧠 is smooth.

&#x200B;

Up until 5/27, GME price movements were strongly correlated to AMC, making the year to date R^(2) value between the two 76%. In 🦍 speak, statistically a price change in GME was 76% dependent on a similar change in AMC, and vice versa. After today's trading, that R^(2) value has decreased by 40% to 0.45! MASSIVE DECOUPLING!

![1. 6\/2 Update - Plot of AMC and GME closing prices - R\(square\) = 0.45](https://preview.redd.it/b7atero9ww271.png?width=726&format=png&auto=webp&s=dfa293c3bf7f75e671a8bf24d8ef0d7a968ad380)

From a risk management perspective, especially ones based on linear analysis, this means a long AMC position can no longer effectively hedge a short GME position based on this correlation breakdown. Some entities use more dynamic analysis for certain pair trades, especially volatile ones, and instead of relying solely on linear regression, can adaptively use a "BEST FIT" model. I now present you the logarithmic regression -

&#x200B;

![2. 6\/2 Update - Plot of AMC and GME closing prices - LOG R\(square\) = 0.72](https://preview.redd.it/48522e20yw271.png?width=726&format=png&auto=webp&s=ddfc4ace1a0731029b7cc73a43b81cf8849fa05c)

Well, after the last four trading days, on a logarithmic scale going long AMC can still hedge a GME short as \~72% GME price movements are dependent on AMC price changes. But this comes with SIGNIFICANT risk management implications! I'll explain -

&#x200B;

![3. GME-AMC prices 1\/4 - 5\/26\/2021](https://preview.redd.it/phb7cvdvdx271.png?width=729&format=png&auto=webp&s=a6fec96b401f5ed16b0b8beeac442fd772816c97)

As of 5/26, the price of GME can be modeled by the price of AMC with the equation **GME(price) = 16.8\*AMC(price) - 12.36**. To hedge a GME short, a HF looks at the *derivative* of the off setting long, and in the case of a linear model, a standard hedge would be to buy \~16.8 shares of AMC for every share of GME that is short. This will reduce the VaR (Value at Risk) of the short GME position. I don't want to get into the full details of how to calculate VaR, but the key thing to understand is VaR models take historical prices to determine the daily price variance of a holding, as well as the covariance between holdings, to give a 95% confidence measure of the max drawdown of a portfolio from one day to the next. Some examples below, please scroll past if the math makes your head spin -

\--------------------------------------------------------------------------------------------------------------

&#x200B;

![What a 95&#37; Confidence looks like for single tail normal distribution](https://preview.redd.it/h5kzdaxp7x271.png?width=455&format=png&auto=webp&s=60e0f6f337bb696a9bbe5e6a28a5fed8b6839a1a)

&#x200B;

**VaR Example 1 - 100 shares of GME**

* VaR on a 100 share GME exposure - On 5/26 the YTD variance of GME closing prices was 22.8% from one day to the next, and the volatility of GME is the sq root of variance, which is 47.8%. To calculate a 95% confidence interval, you then have to multiple the volatility by 1.645 to statistically capture 95% of probable outcomes based on a normal distribution, bringing the value to 78.5%. GME closed 5/26 at $229, so 100 shares is worth $22,900 and the VaR of that position is $22,900\*.785 = $17,987. In 🦍speak, hodling 100 shares of GME going into the trading session on 5/27, there was a 95% chance that position would not gain or lose more than $17,987. Another way to look at it, which is what risk management really is focus on - Over the next 20 trading days, 100 shares of GME should statistically **GAIN** or **LOSE** *more than $17,987 in a single trading session.*

**Var Example 2 - 100 shares short of GME with Offsetting AMC Long 1,680 Shares Pair Trade**

* Now, AMC's volatility must also be taken into account, along with AMC's correlation to GME. The variance of AMC on 5/26 was 11.9%, the volatility was 34.5%, and the correlation between the two stocks was 0.81. The math gets a bit more complicated here, but involves linear algebra and matrix multiplication, but by offsetting a 100 share short GME position by going long 1,680 shares of AMC, the overall portfolio VaR is reduced to $9,476 based on my model.

![Model Snapshot - I'm not just pulling numbers out of the sky](https://preview.redd.it/6ku2hp6kex271.png?width=1315&format=png&auto=webp&s=9704496e364bd89f5ed7280043738c9189094d11)

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Whew, lot's of math, but that's what you quanted, right? Just a bit more math, but we need to revisit the now dominate logarithmic correlation GME and AMC have. From Chart 2 - **GME(price) = 101.7ln(AMC) - 73.533**. The derivative (sorry, calculus) of that is 101.7/(AMC). What does that mean? ~~Unlike a linear regression that can provide an optimal amount of shares needed across prices, a logarithmic correlation results in a constantly fluctuating amount of AMC shares needed to hedge a GME short based on the AMC price, and the higher that price goes, the more AMC shares are needed~~. **(Edit 1) -** ***A hedge using a linear regression has a constant capital requirement, because if f(x) = 2x, f'(x) = 2. In regards to a logarithmic regression, f(x) = ln(x), and f'(x) = 1/x. When using a logarithmic correlation of a long position to hedge the short position, the overall capital required to maintain the hedge increases exponentially as the long side of the trade increases in value, resulting in a feedback loop caused by more buying of the long side of the trade as prices rise, with the "hedging" buying also increasing the price of the long position, until a price point that causes the relationship to fully break down. Eventually the hedge becomes non existent because 1/♾ = 0.***  At a AMC price of 101.7, the shares needed reaches a 1 to 1 parity, and beyond 101.7, the effectiveness of a long AMC position to hedge a short GME share begins to diminish exponentially. This is a catch 22, because if AMC is being used to hedge a GME short, more shares are needed as AMC prices rise, causing further upward price pressure on AMC.

&#x200B;

So now I'm going to try and tie everything together for all 🦍 to understand. HFs short GME have been able to hedge their position with AMC, but the last 4 trading days have forced institutions and MARGE to reassess risk models as the linear relationship turned into a logarithmic one. Because of this change, the amount of AMC shares needed to hedge a GME short position has begun to rise exponentially. This has resulted in an exponential increase in buying pressure in AMC, also leading to an exponential price rise. This strategy can continue based on the models until AMC reaches $100, but is becoming exponentially more expensive to execute with each tick higher in AMC's price. If/when AMC reaches $100, the effectiveness of this hedging begins to exponentially decay, and in theory will lead to an infinite amount of AMC shares being needed, which in reality is not possible.

&#x200B;

The next critical point, is today's price action is just now being updated in risk models across all institutions, and these models also determine counterparty risk and MARGIN requirements. Due to the nature of logarithmic relationships in hedging/VaR, there is still time and pricing intervals available to maintain a long AMC position to offset a GME short, HOWEVER, if AMC reaches $100, this will no longer be the case, and institutions lending out margin to counterparties short GME will no longer be able to use the relationship to AMC to lower VaR used with margin calculations. Instead, each position will be taken independently, and the now exponentially larger AMC positions of SHF, combined with whatever short GME exposure the SHF has will almost certainly blow out all VaR models, leading to margin calls.

&#x200B;

Now I want to be clear, everything to this point has been about hedge funds short GME in general, and not HFT trading firms like Shitadel. These are the players with short GME exposure that hold positions overnight for days/weeks/months at a time. The overnight/premarket moves in AMC have significantly contributed to AMC's outperformance of GME since last week, but during the regular trading session the two have moved nearly tick for tick, until today. I present you today's tape -

&#x200B;

![The Most Important Pink 🍆 You've Ever Seen](https://preview.redd.it/m1cobx06mx271.png?width=1742&format=png&auto=webp&s=b67c7001e7d83734bf1a8c321208cc1c5c301b60)

Take in what these two charts are showing for a moment, and specifically what happened during and right after AMC's first trading halt. Now, this is just theory, based off the evidence presented above, but the most exponential price rise GME had all day **WAS DURING THE AMC TRADING HALT**. If there was ever a smoking gun what 💩a🔔 is doing to ward off a margin call, this is it. During the halt, the main vehicle Shitadel has been using to hedge their GME short went away, right before one of the most important times in the day that institutions use in calculating counterparty VaR and margin needs. GME goes parabolic, because they couldn't hedge the short by purchasing AMC stock, they actually needed to start covering, and that volume spike gives all the confirmation anyone should need to infer some serious forced buying started. The exponential price rise continued until the moment AMC reopened. The HFT algos across the markets are currently programmed to respond to AMC price dumps with corresponding price dumps of GME, and the moment AMC reopened, 10 million shares were dumped, bringing AMC down over $10 in 2 minutes (hmm, recalling GME on 3/10 🤔), triggering another trading halt, but effectively stopping GME's exponential price rise. Now I have no idea exactly how the algos are programmed, but after today it's clear to me there is a clear line of logic that states something along the lines of "If AMC price declines >="x", sell "y" GME shares". It also seems the HFT algos have removed most, if not all logic rules for "If AMC price increases >="x", buy "y" GME shares", and this makes complete sense to me after the AMC-GME correlation has shifted from a linear relationship to a logarithmic one, and most likely why AMC upticks had diminishing magnitude upticks in GME shares as the day progressed. This ALSO means the magnitude of downticks in GME is amplified in relation to AMC during big sell offs.

&#x200B;

So what's next? I expect the institutions that solely handle VaR and counterparty margin requirements with linear modeling are going to raise capital requirements for any account with short GME exposure, whereas those with more dynamic modeling still have a few days. I'm not sure what's going to happen with AMC, but I think it is more likely that AMC continues higher for a bit longer to give SHF more ammo with the algos to stop GME price rises by dumping AMC shares, but as shown in this DD, the higher the price goes and closer AMC approaches $100, the more things get dicey. I do not think $100 necessarily needs to be a ceiling for AMC, but it will cause the final breakdown between AMC and GME and cause margin requirements to rocket higher across the markets due to massively increased VaR. If  🦍 that like movies continue to 💎🖐, the entire market will enter a phase never seen before. I am incredibly impressed thus far what 🦍 that like movies have been able to achieve, and gives me even more confidence in hodling GME, for the MOASS is close. I do think things start getting really interesting if/when GME gets above $300, because after the events of 1/28, 3/10, and today after AMC's first trading halt, it is clear $300 is the line 💩a🔔 MUST DEFEND. Nothing in this post should be considered financial advice, do not buy or sell anything based on any wrinkles this post gave your 🧠.

**TL/DR (for🦍 that can't read) :**

💎🖐🦍➡💩a🔔🎆➡🔥🚀🚀🚀🌙➡🍗🍗🍗

&#x200B;

Edit 1: Clarifying Logarithmic Analysis Below VaR Examples with strikethrough and new text.