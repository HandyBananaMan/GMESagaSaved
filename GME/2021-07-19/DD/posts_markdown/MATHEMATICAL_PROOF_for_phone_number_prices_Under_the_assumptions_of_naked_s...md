# Title: MATHEMATICAL PROOF for phone number prices. Under the assumptions of naked shorts existence. If naked shorts are 200% of float, infinity pool larger than 38% of the float makes short impossible to cover and an infinite squeeze. This was banned on Jungle!
# Author: wladeczek44
# Post URL: [https://www.reddit.com/r/GME/comments/ondeot/mathematical_proof_for_phone_number_prices_under/](https://www.reddit.com/r/GME/comments/ondeot/mathematical_proof_for_phone_number_prices_under/)


TL;DR: I made a calculation which justifies why Infinity Pool is the most dreaded expression by shills. Only part of the float in infinity pool makes short extremely hard to close, virtually impossible. number of shares, respectively:

EDIT: automod on jungle banned it, Pink let it through few hrs later. I edited it to point to this one to keep one place for discussion.
EDIT: updated wrong calculation for scenario of normal shorts closed first.
EDIT: Infinity Pool expression definition used in the title and post: it's a subset of shares owned by the shareholders which won't change the owner in a foreseeable future. The definition and the post as a whole doesn't say anything about the size of this set, this is an analysis of the potential impact of it's existence.

N - naked shorts

F - freefloat

S - normally shorted shares, 29th June on Yahoo this number is reported 18.52% of F.

T - total shares bought by retail including created from naked shorts: T = F + S + N

Assuming the level of shorting from most DDs T is much bigger than F. To close short positions HFs have to buy S + N shares.

When naked short is closed the share associated with it effectively vanishes. There are some buyers who don't want to sell at any point, and some buyers who will sell only a fraction of shares. So let's say there is a number of shares which will never be sold - infinity pool.

I - number of shares in infinity pool

T - I is the number of shares which can be bought.

In favor of shorters, let's assume for convenience that every normal short closed gives a share which can be bought again to cover another short. The optimistic scenario for shorters also assumes that they managed to close naked shorts. After closing naked shorts there are S shorts left and T - I - N shares left in circulation to buy again. Scenario of normal shorts closed first is ~~tougher for HFs~~ equivalent- discussed at the bottom. From the definition of T:

T - I - N = F + S + N - I - N = F + S - I

F + S - I must be a positive number in order to close shorts. If this number is small, like 100, shares will have to be bought S/100 times to close positions. Considering a scenario where at least part of the retail are idiots who don't know anything about existence of the sell button it get's really interesting. Say, independently of each other, en average, buyer won't sell 30% of his shares: I = 0.3*T and normal shorts S = 0.18*F. So the number of shares left to close short will be

F + 0.18*F - 0.3*T = 1.18*F - 0.30*(F+S+N) = F\*(1.18 - 0.30 - 0.18*0.30) - 0.3*N = 0.826*F - 0.3*N > 0

0.826\*F/0.3 > N

F > N/2.75

I hope this gives you an idea of how shorters are fucked. If the number of naked shorts vastly exceeds F infinite pool doesn't have to contain all the shares in circulation to make it impossible to close. And this is a weak scenario. In fact let's put I = a\*T where a is a fraction if idiots mentioned above.

F\*(1.18 - a - 0.18*a) - a*N > 0

1.18*F - 1.18*F*a - a*N > 0

1.18*F - a*(1.18\*F + N) > 0

1.18*F > a*(1.18\*F + N)

1.18*F/(1.18*F + N) > a

now there is a direct relation between N and a. In a "big" scenario where N = 2\*F. Number is arbitrary, but less than some estimates [yesterday](https://www.reddit.com/r/Superstonk/comments/omdafo/final_update_of_google_consumer_survey_n2200_at/?utm_medium=android_app&utm_source=share) (rounded from 0.371, thanks for the link u/karasuuchiha) :

0.37 > a

Even a relatively small infinity pool cause shorts impossible to close. Appendix:

If normal shorts are closed first, then shares left to cover N are ~~T - I - S = F + S + N - I - S = F + N - I~~ 

T - I because shares remain in circulation. Must be higher than N to cover.

F + S + N - I > N

F + S - I > 0

F + S - a\*(F + S + N) > 0

(F + S)/(F+S+N) > a which is ~~even more difficult.~~ equivalent.

further read - one ape here referred to an analysis by u/pjotra123 3 months ago about how pricing during the moass could look like. It's extremely wrinkled so maybe a good idea to ask the author for some smooth crayon version:

https://www.reddit.com/r/GME/comments/nsv3mz/moass_visualized_distributions_game_theory/?utm_medium=android_app&utm_source=share