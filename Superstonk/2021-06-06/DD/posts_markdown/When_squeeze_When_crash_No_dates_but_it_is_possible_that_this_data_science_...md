#Title: When squeeze? When crash? No dates, but it is possible that this data science technique might give an early warning...
#Author: squirrel_of_fortune
#Post URL: [https://www.reddit.com/r/Superstonk/comments/ntou9t/when_squeeze_when_crash_no_dates_but_it_is/](https://www.reddit.com/r/Superstonk/comments/ntou9t/when_squeeze_when_crash_no_dates_but_it_is/)


**TL/DR:**

Cool math technique to predict stock market crashes looks like it might predict reverse flash crashes, i.e. squeezes, it seems to work for the Jan squeeze and VW squeeze. I will let you all know if it starts to predict again. (edited the TLDR)

**OK, why am I here?**

Originally, I was interested in using topological data analysis (TDA) to predict stock market crashes to put into an algorithmic trading bot to trade for me. I avoided joining wallstreetbets after my wife's boyfriend joked that I would end up an admin (the way to get to be an admin on WSB is apparently to YOLO all your money and lose it!). So, I started mucking around day trading stocks to learn how the stock market worked (I lost 50K paper trading options so I figured I didn't know what I was doing with options and stuck to stocks), and then like the rest of you got into GME. The point of that potted autobiography was that I wanted to use TDA on the stock market (I use it in my day job).

**Introduction**

The stock market is a complex system (obviously) and can be described with complex system theories. (I haven't really looked at this stuff for around 10 years, so this bit will be a bit vague). Complex systems can suddenly change, in the physical sciences these are called regime changes where a system changes from one regime of behavior to another. For example, if you heat up ice it will absorb heat energy for a while then there is a regime change to water (called a state change in chemistry). In the stock market these regime changes have names like 'crashes', 'flash crashes', and perhaps melt-ups and melt-downs whatever they are. (As a total aside, I think that fast algorithmic trading makes these regime changes more likely and sudden due to dampening the small fluctuations in the market, so there's less of an escape valve and new prices are discovered quickly and violently).

Topology is my new favorite bit of math. It's basically the mathematics of squashy objects, it describes how pretzels and donuts are different, but teacups and donuts are the same. In that case, it counts the number of holes in the object, and asks the question, if the objects were made out of playdoh, could you manipulate a donut into a tea-cup (without tearing it or making new holes).

Anyway, all you need to know is that topology measures patterns in the data. And the method of using topology to look for these patterns is called topological data analysis or TDA. There is underlying patterns in the price and volume data that can be used to give an early warning of crashes and the like.

There has been some recent work on using TDA to predict stock market crashes. These papers are mega new, and this is new thing, lots of them are dated from 2020.

Final thing you need to know, the things we look for are called topological features, and they are calculated from the shapes of objects (in this case, stonks). It may help to tell you that datapoints can describe points in space, and thus data series can be described as having shape properties. Here we use something called landscape distance and something called a Betti distance. We measure these distances and look for changes in them, and changes in the underlying distances suggest something is about to happen. According to the papers, that something is a crash.

**Questions**

**Question 1. Can I use this to predict the top of the squeeze?**

**Question 2. Can an examination of the GME and AMC topological features reveal any strangeness that might be extra evidence of stock manipulation?**

I think at this point, it's best that you look at the pictures. Pay attention to the red circles indicating a crash probability over 30%

**GME data**

![Landscape distance based data for GME](https://preview.redd.it/1b4yyh12tn371.png?width=1775&format=png&auto=webp&s=d15eb4e562ec051f2a0a04b2056e17558866173a)

![Betti distance based data for GME](https://preview.redd.it/ep6rcjp2tn371.png?width=1775&format=png&auto=webp&s=1bbf06423cbeef7b629b4bcba805000131ddb906)

**AMC data**

![Landscape data for AMC](https://preview.redd.it/3s3dpgwbsn371.png?width=1775&format=png&auto=webp&s=c99374505b01f12fe3013551b264ec27edffb802)

![Betti based data for AMC](https://preview.redd.it/m8utugvcsn371.png?width=1775&format=png&auto=webp&s=50f843c3f8c6710170b10ccda56816402abb5c22)

**Things to note:**

1. Landscape distance is more optimistic (less likely to predict a crash) than Betti distance.
2. **High probability of a 'crash' in early to mid Jan for both GME and AMC**
3. **High probability of a 'crash' in late march early April**
4. Low probability of a 'crash' at the moment. (Wen Lambo? Not yet)
5. GME and AMC look similar (I showed that they were significantly correlated in my last post [https://www.reddit.com/r/Superstonk/comments/ns8dhk/yes\_those\_patterns\_yall\_keep\_posting\_are\_real\_the/?utm\_source=share&utm\_medium=web2x&context=3](https://www.reddit.com/r/Superstonk/comments/ns8dhk/yes_those_patterns_yall_keep_posting_are_real_the/?utm_source=share&utm_medium=web2x&context=3) )
6. **That 'crash' predicted in early Jan was the first short squeeze.**

So, I think number 6 is the most important here. It seems that this technique for predicting crashes has found a reverse crash. **Is a short squeeze the opposite of a flash crash?** This technique has been successfully used to predict flash crashes.

Going back to systems theory and regime change it looks to me that this method can find reverse crashes (i.e. squeeze type things). I don't know finance, so if anyone wants to tell me the technical term for these things please do). Before the regime change (crash, squeeze) there is higher variability in the stock, and it is this that the TDA works off of. So, I think that this method can predict the possibility of a reverse crash.

Anyway, lets look at the VW/Porche squeeze.

**VW during the squeeze**

![VW landscape distance based data](https://preview.redd.it/ef3yvx7esn371.png?width=1764&format=png&auto=webp&s=a0c2eb0a4276bd503d87225dd62f6bcbd41b4cd3)

&#x200B;

![VW Betti distance data](https://preview.redd.it/92i9s38usn371.png?width=1776&format=png&auto=webp&s=71c56921322ab7b186541192bd8fb3bb4ff880de)

Look, in early 2008 there was a prediction in both graphs of a crash, the stock went up. The Betti distance predicts a crash in May-September that didn't happen. But the three data points just before the squeeze are all predicting a crash, then we get a squeeze.

I gotta be honest, I'm giving the Betti graphs for VW, AMC and GME a bit of side eye here as the VW graph has that red section that predicts nothing in the middle, and we see this pattern in the AMC and GME graphs.

Now, lets have a little look at some non-squeezing boomer stocks, and this is where it gets a little odd.

**IBM**

![IBM landscape based data](https://preview.redd.it/daqtq49gsn371.png?width=1775&format=png&auto=webp&s=17702f5dbcc5b92bc3d15805afcc7d8c49bd7522)

![IBM Betti distance data](https://preview.redd.it/be1lqe7hsn371.png?width=1775&format=png&auto=webp&s=e066861c58baba002af5380215b28fca41b208b2)

The landscape distance measure says that Big Blue has nothing to worry about, the Betti distance data is hyperventaliting that a crash in coming. (Of course, I think we all believe that a general stock market crash is incoming).

Hmmmm, so I picked a smaller stock, our favorite restaurant.

**Wendy's**

![Wendy's landscape distance data](https://preview.redd.it/garliqwisn371.png?width=1775&format=png&auto=webp&s=5d766a9cb76b486661c6615d0f3456b04a271c78)

![Wendy's Betti distance data](https://preview.redd.it/04sduf2ksn371.png?width=1787&format=png&auto=webp&s=cb914c9e5ddc07836496898a01c07f844aa2b5bb)

Yeah, Wendy's is safe. And as a smaller bricks'n'mortar company, is a better comparison for GME and AMC. So this could show that the GME and AMC behavior is odd. I should probably repeat all this with different windows (the data is smoothed), finer grained data and more stock comparisons.

**Conclusions (actually more questions)**

Well... The distance measures here obviously measure a few different things, impeding regime change, whether up or down, and impending crashes. I think that this explains IBM's data, the stock market as a whole looks a bit crashy when analysed with this technique.

There are some false positives in the method (where the method predicts a change that doesn't happen).

**Is it possible that the prediction of a regime change in April in GME and AMC that didn't happen is a result of some oddness in the stock? (Oddness like synthetic shares, very low volume coupled with large price swings, unnatural behavior perhaps?)**

**Will this method show the impending squeeze?** (stay tuned)

**And, will it show when we're at the top of the squeeze?** Looking at the VW behavior it doesn't seem so. I think it might if I had more fine-grained data (5 mins data), cos these prices are smoothed out over a few days.

I have a feeling I might end up writing an actual academic paper on this shit.

**References:**

[https://towardsdatascience.com/detecting-stock-market-crashes-with-topological-data-analysis-7d5dd98abe42](https://towardsdatascience.com/detecting-stock-market-crashes-with-topological-data-analysis-7d5dd98abe42)

[https://arxiv.org/pdf/2004.02551.pdf](https://arxiv.org/pdf/2004.02551.pdf)

behind a paywall [https://www.sciencedirect.com/science/article/pii/S0378437117309202?casa\_token=DfG\_j6zdAQ0AAAAA:91hHDLuhIGqABmnkZXyiVNgFVETL-hmDYOZJwYLVYneWrm0Vap1LAvAg6XwvSVC0mTnWi2O\_4w](https://www.sciencedirect.com/science/article/pii/S0378437117309202?casa_token=DfG_j6zdAQ0AAAAA:91hHDLuhIGqABmnkZXyiVNgFVETL-hmDYOZJwYLVYneWrm0Vap1LAvAg6XwvSVC0mTnWi2O_4w)