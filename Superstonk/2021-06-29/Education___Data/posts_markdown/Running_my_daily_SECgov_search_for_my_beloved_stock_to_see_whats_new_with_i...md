#Title: Running my daily SEC.gov search for my beloved stock to see what's new with it and here's what came out (06-29)
#Author: Purple-Artichoke-687
#Post URL: [https://www.reddit.com/r/Superstonk/comments/oa7lj0/running_my_daily_secgov_search_for_my_beloved/](https://www.reddit.com/r/Superstonk/comments/oa7lj0/running_my_daily_secgov_search_for_my_beloved/)


The search: [https://www.sec.gov/edgar/search/#/q=gamestop&dateRange=all&startdt=2021-06-28&enddt=2021-06-29](https://www.sec.gov/edgar/search/#/q=gamestop&dateRange=all&startdt=2021-06-28&enddt=2021-06-29)

Well, nothing really interesting came out actually so I'll flag this as Education/Data instead of the usual News.

But them I ran my script to update the NPORT-P data dump for 30 apr since some new NPORT's have been submitted:

[https://docs.google.com/spreadsheets/d/1oVe2viQBOlgHKJL6qMnem3X3dReaBdgdRae05s8sZxE/edit#gid=1035308087](https://docs.google.com/spreadsheets/d/1oVe2viQBOlgHKJL6qMnem3X3dReaBdgdRae05s8sZxE/edit#gid=1035308087)

And I was astonished of the data!

![Yes, you read that right. They have more shares on loan than they hold.](https://preview.redd.it/il9sn9rw87871.png?width=1078&format=png&auto=webp&s=13c3dbd0b919843d2446abc97a51fc79bacd3b14)

Now, we really need an adult here! Did these guys just filed with the SEC that they loaned more shares than they own?

Then I went through the YTD data dump (one of the tabs in the doc) and there are cases where this happens but the differences are pretty small and might come from how the value on loan is calculated. As they don't disclose the number of shares on loan, I'm using this formula:

    sharesOnLoan = valueOnLoan/(usdValue/sharesHeld)

It worked so far, even for their previous fillings it worked.. could be an reporting error or the data is good but we need an adult.

\---

Do what you want with this info, could be nothing, could be good DD starting point for more wrinkled brain apes, I just like to search [SEC.gov](https://sec.gov/) and this is no kind of advice, this is written on the SEC website.

Will look out for new updates throughout the day and update.

Obligatory: 🚀🚀🚀

**Edit:** Updated the data dump with a column of GME weight in the fund (percent) because I found it interestingly enough that for the two investco funds with bad data, the holdings are quite unusual (8% and 6%)

**Edit2:** Did a little rabbit hole digging. This is the first filling URL: [https://www.sec.gov/Archives/edgar/data/0001209466/000175272421142046/0001752724-21-142046-index.html](https://www.sec.gov/Archives/edgar/data/0001209466/000175272421142046/0001752724-21-142046-index.html) 

We have a ticker there, XSVM. good.

So follow the CIK:

[https://www.sec.gov/cgi-bin/browse-edgar?action=getcompany&CIK=S000003025](https://www.sec.gov/cgi-bin/browse-edgar?action=getcompany&CIK=S000003025)

Check previous fillings. GME is in there correctly reported and in different percentages...

Search [etf.com](https://etf.com): [https://www.etf.com/XSVM#overview](https://www.etf.com/XSVM#overview) No mention on the GME position.

Official website: [https://www.invesco.com/us/financial-products/etfs/holdings?audienceType=Institutional&ticker=XSVM](https://www.invesco.com/us/financial-products/etfs/holdings?audienceType=Institutional&ticker=XSVM) No Mention on the GME position

Checked the web archive. Just an archive on Jan 20, 2021: [http://web.archive.org/web/20210120095023/https://www.invesco.com/us/financial-products/etfs/holdings?audienceType=Institutional&ticker=XSVM](http://web.archive.org/web/20210120095023/https://www.invesco.com/us/financial-products/etfs/holdings?audienceType=Institutional&ticker=XSVM) No mention on the GME position.