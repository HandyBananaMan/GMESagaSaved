# Author: pushinbombadils
# Post URL: [https://www.reddit.com/r/Superstonk/comments/no8cqe/important_fud_regarding_the_sudden_drop_in_online/](https://www.reddit.com/r/Superstonk/comments/no8cqe/important_fud_regarding_the_sudden_drop_in_online/)


***Edit:*** *Per recommendations from commenters, I've updated the flair to DD. I'd originally flaired as "Education/Data". Mods, if it needs to be switched back, I'm more than happy to.*

\-------------------------------------------------------------------------------

**I'm not giving you a TLDR. If you panicked over the other posts and jumped to conclusions, you need to sit down and read this one.**

There were a couple of highly upvoted posts about active users/users online suddenly dropping. The conclusion in the majority of the comments is “these are bots logging off suddenly":

* [Example 1](https://www.reddit.com/r/Superstonk/comments/no2mm0/this_sub_just_went_from_85000_users_online_to/)
* [Example 2](https://www.reddit.com/r/Superstonk/comments/no2er4/anyone_else_just_saw_the_number_of_online_users/)

Guess what? **This has been going on for a while now.** Stop what you’re doing for a moment, and breathe, read this, get some wrinkles.

&#x200B;

Important stuff before the education part:

1. **Creds:** I'm a senior level software engineer at a very, very large corporation. Part of my job is (and has always been) assisting setting up environments and configuring/setting up servers/server management software to environments that have to be up 24/7. I have been doing this job for over 8 years. I have seen some shit and done my time. I am tired.
2. “Users Online” is not the number of people **actively viewing** the sub, it's the number of **active sessions** tied to the sub (meaning that a browser/app is currently logged in and that subreddit is up in that client).
3. Yes, there are bots here. Whoopty-freaking-doo, because, guess what? The DD hasn’t changed. Buy, hold, grab a towel and *don’t flipping panic.*
4. This is not financial advice, nor is there any here.

**Ever wonder why Reddit is (almost) always up and rarely has maintenance?** It’s because they have some form of a load balancer that filters the request load between the underlying web servers so that (in general) the site stays up. Every now and again, the underlying servers have to go down for maintenance or have scheduled tasks that refresh the active memory, clear sessions, and perform updates (e.g., security patches) so that the site is still accessible even though the engine hood is open and there's black smoke billowing out.

[Actual picture of me and you, right now](https://preview.redd.it/nqdzvobn48271.jpg?width=900&format=pjpg&auto=webp&s=d26537f5db7501eb434d9b05c3c1a742cd9d4161)

**ELIAA:** When you access most sites nowadays, you’re not sending a request to a physical machine or box – you’re sending a request to a *load balancer*. This is a piece of software (think of it like a valet) that chooses how your request to the site will be directed *before it even gets processed*. The response you see in your browser is *not coming from a single location* \- it's distributed internally across multiple internal networks and there is a huge amount of stuff going on behind the scenes just so you can see Superstonk at 3 AM.

Reasons why this is good:

* Load balancers distribute the load between the underlying servers so if one server has gone down, the system stays up. This is called redundancy. It's like having multiple cash registers at a supermarket - if one goes down, you can still check out customers, *they just have to switch lanes*.
* Load balancers act as a buffer between the underlying servers and direct contact with the outside world. Think of a load balancer like your computer's firewall, except that firewall has AI that detects threats/threat patterns *and* has active management around the clock by real live server administrators (who sometimes get calls at 3 AM because servers go down or someone forgot to press F3).

Having a *distributed internal network* of servers means that when there's issues or internal maintenance, the ability to access the site doesn't change... but people sometimes see weird effects (like active users dropping, or the site being down momentarily).

**The most likely explanation:** Reddit’s server management system does “scheduled cleanup” on sessions. It drops inactive sessions (or refreshes sessions) older than X minutes or starts dropping them when a server or component has too many sessions in memory. Some form of this is standard practice across the industry - it clears up local memory and makes the site run faster as a whole. Think of it as “clearing your cookies/cache” in your browser, except Reddit is doing it on the backend with your *session* when it needs to. The effect you see is that everyone who hadn't accessed it in a while got kicked, ergo, 150k -> 20k in less than 5 minutes.

*Wrinkly Stuff: a session is a quick and easy way of keeping up with a user's state while they're logged into a system without the user ever knowing about what the session contains. Sessions can hold a lot of info, or very little, depending upon the architecture of the underlying application(s). In this case, Reddit is most likely holding your current subreddit* *in session, or current subreddits - which is important to think about... if you have multiple tabs open, which tab are you "online" for - all or one?* ***The "online users" is not a count of the number of people "actively looking" at the subreddit, it's a number used to gauge interactivity, which is calculated by reddit internally using session data, ceiling wax, and other fancy stuff.***

Even if you didn't understand much of the "wrinkly stuff" above, re-read the the bolded sentence. "Online users" is **not** the number of users that are **currently focused** on the subreddit. It includes browser sessions that left a tab open (ever leave an extra 15 tabs open?) or reddit being open in the app on your phone in the background (ever check SuperStonk every 5 minutes?).

So, yes - I'm sure there's several shills and bots in there too (hi Ken and all his friends). But, based on what I've seen posted, many of us are tuned into this from the moment we get up til the moment we go to bed. I know I am. It's very possible we could actually have 100-150k active users on a daily basis.

So, yes, we have bots. Yes, we have lots of non-subscribed visitors, but that's understandable because we're starting to get attention *and has been noted for a while*. I cannot disprove or confirm that the sudden drop in online users *isn’t* bots logging off en masse.  However....

**I can confirm that this has been reported** ***in a positive light*** **since the initial GME/Superstonk split (which I was here for), which makes me suspect this is being highlighted because of FUD.**

Posts dating back to inception:

* ["Look at the online users"](https://www.reddit.com/r/Superstonk/comments/mkkdwa/almost_70k/)
* ["More users online than GME"](https://www.reddit.com/r/Superstonk/comments/mkosn6/holy_cow_guys_you_are_amazing/)
* [**"No other sub has this many of its users online at once"**](https://www.reddit.com/r/Superstonk/comments/ms9ny5/no_other_sub_has_this_many_of_its_users_online_at/)

That last one is the most important. One month ago, we were celebrating having 66% of the sub online. Now... we're not? What changed?

There very well could have been a ton of bots logging off - my point is that it was the only answer provided, **and it is 100% not the only possible answer and is based on BIAS.** *Also - did anyone posting these even check or monitor any other subs* *outside* *of their confirmation bias circle (Superstonk/GME/W-s-b) to see if they had the same issue? (****Seriously****, if anyone has this info, it is vital to check against a non-biased dataset before jumping to conclusions)*

So, the data hasn't changed. The DD hasn't changed. **The only explanation is your emotions are getting the better of you**. One month ago we were celebrating the number of active users online and now it's being called sus. The fact that this sub is incredibly active has not changed. If you celebrated it before and now it's sus, your own FUD has affected your judgment.

Grab a towel and a tea and for the love of the gods breathe. Nothing changed in the data, but your POV did.

**It's the weekend, chill and trust the DD.**