# Title: Post 8: I did a thing - i backed up the subs. and the comments and all the memes
# Author: Elegant-Remote6667
# Post URL: [https://www.reddit.com/r/GMEJungle/comments/owifgo/post_8_i_did_a_thing_i_backed_up_the_subs_and_the/](https://www.reddit.com/r/GMEJungle/comments/owifgo/post_8_i_did_a_thing_i_backed_up_the_subs_and_the/)


Hello,

Ape historian here.

I know ive been a way for a loong time, but i am going to make a post about what has been happening.

The first things is that the data ingestion process has now completed.

&#x200B;

![Drumroll please for the data](https://i.redd.it/y4zrrxmzxye71.gif)

We have some nice juicy progress, and nice juicy data. There is still a mountain of work to do and ~~i know this post will get downvoted to shit.~~  EDIT: wow actually the shills didnt manage to kill this one!

&#x200B;

**Point 1:**  I have all the GME subs and all the submissions. Yeah. ALL. OF THEM.

* Superstonk
* DDintoGME
* GME
* GMEJungle
* AND wallstreetbets

Why the wallstreet bets you might ask? because of point 2. The ammount of data that we have: and oh apes do we have  A LOT!

&#x200B;

![6 millies for GME, 300k for the GME sub, 9millies for superstonk. and \(still processing 44! Million for wallstreet bets!\)](https://preview.redd.it/eweg6scnzye71.png?width=254&format=png&auto=webp&s=70f9f98c5f7b344a925a915253f8150987987b4c)

so why is the chart above important?

**Point 2: Because i also downloaded all the comments for all those subs**

**Point 3:** The prelinary word classification has been done and the next steps are on the way and we have 1.4Million potential key words and phrases. that have been extracted

Now for anyone who is following, we have \~800k posts, around 60 million comments and each of those have to be classified.

Each post and comment may and does have a subset of those 1.4Million keywords in there that we need to identify.

The only problem is is that with standard approaches, checking millions of rows of text against specific keywords takes a long long time, and i have been working on figuring out how to get the processing time down from \~20-50 milliseconds per row to the microsecond scale - which funnily enough took about 3 days.

We have all seen comparison of million and billion. now here is the differnence in procesessing time if i said 20milliseconds is fast enough.

&#x200B;

&#x200B;

![processing of one \(out of multiple!\) steps at 20milliseconds per row](https://preview.redd.it/b4rl6mo31ze71.png?width=697&format=png&auto=webp&s=2107b7970cc1ccec83f2e8650829900b33dc34af)

&#x200B;

![Same dataset but now at \~20 microseconds per row processing time](https://preview.redd.it/8r3gmysb1ze71.png?width=712&format=png&auto=webp&s=013ed2a270711adde8782b56df8716a2978bfb18)

&#x200B;

But we are there now!

**Point 5: we have a definitive list of authors:** across both comments and posts, by post type, and soon by comment sentiment and comment type

&#x200B;

![total number of authors across comments and posts across all subs- as you can see we have some lurkers! Note that some of those authors have posted literally hundreds of times, so its important to be aware of that.](https://preview.redd.it/41wzjweq3ze71.png?width=270&format=png&auto=webp&s=c0bf452750f21a5eacfecdae7bf13984763b03f3)

&#x200B;

&#x200B;

My next plan of action:

the first few steps in the process have been completed. I now have more than enough data to work with.

I would be keen to hear back from you if you have specific questions.

Here is my though process for the next steps:

1. run further NLP processes to extract hedge fund names, and discussions about hedgies in general
2. complete analysis on the classified posts and comments to try to group people together - do a certain number of apes talk about a specific point - can we use this methodology to detect shills if a certain account keeps talking about "selling GME" or something like this.
3. Run sentiment analysis on the comments to identify if specific users are being overly negative or positive.
4. And any suggestions that you may have as well!