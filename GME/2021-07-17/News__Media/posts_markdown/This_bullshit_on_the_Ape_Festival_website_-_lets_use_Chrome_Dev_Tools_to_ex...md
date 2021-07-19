# Title: This bullshit on the Ape Festival website - let's use Chrome Dev Tools to explore some bullshit.
# Author: spozzy
# Post URL: [https://www.reddit.com/r/GME/comments/olxx95/this_bullshit_on_the_ape_festival_website_lets/](https://www.reddit.com/r/GME/comments/olxx95/this_bullshit_on_the_ape_festival_website_lets/)


Ape Festival and its organizers can go to hell, but I just wanted to highlight some off the bullshit tactics around the Ape Festival website.

I've been on this AF website for about an hour now, and it is incessantly telling me about all of the other people who have bought festival tickets...

![Nobody bought shit 31 minutes ago. Fuck you.](https://preview.redd.it/9z6oe9mmfpb71.png?width=1596&format=png&auto=webp&s=9d69da9dd00459d579567d90851d0ef907343dcc)

See the popup in the bottom left corner? It appears every few seconds. This is a marketing strategy to elicit feelings of FOMO so that everyone buys.

I traced the code, and the Ape Festival animals are running [this plugin](https://apps.shopify.com/recent-sales-popup-notifications-1/reviews?page=2), which describes itself as "social proof, sales popup urgency, stock countdown timer, FOMO."

Remember when I said I was on the site for more than an hour? The stock for all items have been listed as "sold out" -- all tickets, all sizes. See below for ticket types (you can verify sizes are sold out when you click into them, but I'm not going to post 20 screenshots):

&#x200B;

![No, nobody bought shit 37 minutes ago either. Fuck you.](https://preview.redd.it/o9srpvzmgpb71.png?width=917&format=png&auto=webp&s=40f54fba6c182ae906129ded88c2f985b314962e)

So riddle me this:

1) How are there popups showing up that say a package was purchased in the last 31-37 minutes? (I purposely included that in the screenshot above)

2) How is my browser receiving this "live data" if my chrome developer tools (right side) is not showing any network activity being sent to my browser?

Just beware. The website was not created innocently. It is all being driven to manipulate apes. You all already know this, but I just wanted to provide a perspective from looking at their code, and tracing the network. Fuck these guys and see you all on the moon, where we will all celebrate together in spirit.