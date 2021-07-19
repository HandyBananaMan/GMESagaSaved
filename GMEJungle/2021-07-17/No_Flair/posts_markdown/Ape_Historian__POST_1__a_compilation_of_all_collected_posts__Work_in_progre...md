#Title: Ape Historian | POST 1 | a compilation of all collected posts | Work in progress
# Author: Elegant-Remote6667
# Post URL: [https://www.reddit.com/r/GMEJungle/comments/ombzoz/ape_historian_post_1_a_compilation_of_all/](https://www.reddit.com/r/GMEJungle/comments/ombzoz/ape_historian_post_1_a_compilation_of_all/)


Good afternoon all wonderful apes!

As I mentioned, I have decided to document what the entire collection of DD.  This database is updated daily, and currently looks at superstonk posts and DDintoGME posts. Now that my rig is back online after a PSU failure a few days back (thankfully just a PSU failure!)

This is a very early work in progress but I am hoping that if it is useful I can build out the pipeline to include more features, better breakdowns and so on and so forth.

There are a few caveats here:

1. The data is not clean or perfect - if the url starts with e.g. / r / superstonk the author name isnt correct - I am looking into why that is and how to change that.
2. THere are crap links! a lot of them. I have done a quick job at classifying some obvious ones into memes and pic, flagging specific subs and news.
3. You can filter by created date as well as author - all the criands DDs and attobits dds are there of course
4. Comments arent currently collected for most of these
5. THERE ARE so much shitty memes and pics - those have their own category - you can see just how much shit there has been created.

&#x200B;

My plan:

* My plan for this is to flex my data skills (and hopefully learn something new): the pipeline of features is as below roughly in this order  


1. Data cleanup
2. Past Post Topic detection and future classification of topics for new posts
3. Identification of top authors / users / potential shills, based on tactics, post history, post frequency post type and so on - if sstonk had satori, its not that my plan is to singlehandedly recreate it, but I think some transparency into potential shill accounts, or low effort accounts is a fair game.
4. Comment extraction from these posts (possibly only the top 1000 due to limitations)
5. Classifcation and cleanup of the multiple news sources that have been spammed as of late across the sub.
6. Possibly adding tracking for other subs of interest (e.g. gme)

&#x200B;

I will upload a csv file to filebin today(it expires in 3 days): here is the link for anyone who wants to already have a look. The bin will always be locked so no one else can upload fud shit in there but always verify the shasum below, just in case.

&#x200B;

&#x200B;

[Filebin will always be locked](https://preview.redd.it/knt767fk0ub71.png?width=1915&format=png&auto=webp&s=22e4df50b152cf6321e60cc5d4b17aec1ec1d7ab)

URL:[https://filebin.net/eqg9n2hsi84vtctq](https://filebin.net/eqg9n2hsi84vtctq) 

If someone is aware of a better anonymous file upload service, that doesnt require registration to upload or download, **please let me know!**

TLDR-always verify files from the internet. attaching a shasum

shasum:92664947a71def53c6bdaaab06750b557f11a4d1

[shasum: 92664947a71def53c6bdaaab06750b557f11a4d1 ](https://preview.redd.it/vyzs8vvsztb71.png?width=787&format=png&auto=webp&s=b07e186a339f994f55c0bb7019cf23845c4e98af)

if anyone is interested, the schema to the file is:

&#x200B;

[I will clean up the column names into better categories once \/ if this is useful](https://preview.redd.it/h8i1z7r50ub71.png?width=480&format=png&auto=webp&s=c541baaa02a8db9a3c0f3d56539ae467fad5eb92)

I would be very open to hear opinions about this, whether this is useful, and whether it is not. 

There is no sub / mod rule at the moment for something like this , so u/pinkcatonacid, feel free to ping me / comment if you have feedback.