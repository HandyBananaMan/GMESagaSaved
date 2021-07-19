# Title: NO BRIGADING
# Author: redchessqueen99
# Post URL: [https://www.reddit.com/r/Superstonk/comments/o80eky/no_brigading/](https://www.reddit.com/r/Superstonk/comments/o80eky/no_brigading/)


It has become an increasingly problematic situation for r/Superstonk and our nearly 500,000 members that some individuals are repeatedly harassing other subreddits. As moderators, we have declared a zero tolerance policy for brigading and have mentioned this multiple times in our daily news posts, as well as on YouTube and Twitter, so as to reach as many of you as possible.

# Automod Change - No Subreddit Mentions

Nonetheless, the problem has persisted. Several moderators from other subs have supposedly reported this to Reddit admins, and we have now received messaging from Reddit admins about this very topic, and the following has been forcibility added to our automod code:

    #do not remove per admins
    
        title+body (regex, includes): ['\br/ ?(?!superstonk)\S+']
        action: remove
        action_reason: "links to other communities {{match}}"
    
    #do not remove per admins 
    
        title (includes): ["r/"]
        action: remove 
        action_reason: "call outs of other communities {{match}}"

Also, I have added the following words to automod for instant removal: **gme\_meltdown**, **melvincapitallove**, **wallstreetbets**, **amcstock**, **WSB**, and **AMC**. This list will be adjusted as necessary in regards to preventing discussion of other subs, in accordance with Reddit Admins.

# No Tolerance for Brigading

Brigading can include the following:

* Vote manipulation of other subs' content, either positively or negatively
* Harassing other subs' posts and comment threads with pro-r/Superstonk content
* Making posts on this subreddit about other subs and their members
* Organizing in any way to influence other subs one way or another
* Posting negative comments or posts on r/Superstonk itself
* Posting screenshots of posts from other subs

We understand that there are many issues coming from other subs. I will not name those issues because of the new Reddit automod rule that says we cannot discuss those subs. But many of us have felt defensive in this regard. I kindly ask all of you to stay focused on r/Superstonk, the stock we all love $GME, and issues of the financial world, and not those of the reddit world. As of today, you can no longer discuss other subs on this subreddit.

**We have also DISABLED CROSSPOSTING for the foreseeable future, so as to not include other subreddits in any way.**

Please note that we cannot enforce these rules off of Reddit, such as on Twitter, Discord, or YouTube, unless it is by means of our own individual accounts. However, we do discourage making this a big issue on other social media, because that could also be used against us.

# No Brigading Rule

We have also added a new rule that will be used to remove content and potentially BAN users for this behavior:

>Under NO circumstances, will brigading be tolerated on this subreddit or any other. Individuals who are discovered to be participating in this, risk being permanently banned for this reason.  
>  
>Brigading includes:  
>  
>\- organized voting on other subs  
>  
>\- harassing other subs  
>  
>\- using r/Superstonk to defame other subs  
>  
>\- sharing screenshots from other subs  
>  
>Additionally, Reddit Admins have placed an irremovable code into our automod that prevents linking other subs entirely.

If you violate this rule, you will be considered an instigator in directly attempting to take down r/Superstonk, and we will respond as intensely as can so as to prevent that circumstance.

# Additional Measures

We are currently exploring additional measures on how to comply with Reddit Admins' anti-brigading rules, and that may include increasing karma/age limits considerably as well as bringing in considerably more moderators that we trust and can rely on to properly moderate the sub. We are making these changes due to outside parties reporting us for facilitating brigading and also due to Reddit admins contacting us directly in a very concerning manner.

If you see brigading, please discourage it as intensely as you can. We do not allow this, and it is a bannable offense. We hope to comply entirely with Reddit Admins' requests, as that is the platform we are on. We need to comply with Reddit rules above all else. Thank you.

# Edit: Automod Code for Other Subs

I have also created an automod code that can be easily copy/pasted into other subreddits' automod, which will effectively block crossposts from r/Superstonk. I just tested it and it works great! If other subs are truly having issues with our members crossposting into their subs, they can use this to block us:

    ---
    
    # SUPERSTONK GTFO
    
    type: crosspost submission
    crosspost_subreddit:
        name: ["Superstonk"]
    action: remove
    message: |
        We don' like yer kind 'roun 'ere.
    
    ---

As of current, our automod and rules are updated to be strict against brigading, limiting certain words and references to other subs, and all crossposting is disabled. I am unsure personally how to prevent this further, so here is code that other subs can use to block specific words and mentions:

    ---
    
    # I DONT LIKE THE STOCK
    
    title+body (regex): ["GME", "$GME", "to the moon", "paperhand"]
    author:
        is_moderator: false
    action: remove
    message: |
        We don't like the stock, but we haven't read enough DD.
    
    ---

Hopefully now it can be evidently clear that we are making zero efforts to Brigade other subs, and are now actively bolstering their capabilities against us. I am confident r/Superstonk will nonetheless grow and continue to unearth the truths of the real market due to GameStop stock and research around it. I like the stock. I love the company. CAN'T STOP; WON'T STOP.