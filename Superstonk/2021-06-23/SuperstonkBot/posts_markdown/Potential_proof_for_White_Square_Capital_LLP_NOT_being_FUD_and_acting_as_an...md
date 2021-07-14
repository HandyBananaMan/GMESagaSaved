# Author: SuperstonkBot
# Post URL: [https://www.reddit.com/r/Superstonk/comments/o6otv9/potential_proof_for_white_square_capital_llp_not/](https://www.reddit.com/r/Superstonk/comments/o6otv9/potential_proof_for_white_square_capital_llp_not/)


Hi all.

**TLDR: I have found multiple companies (where some are offshore) which in some aspects link between Citadel, White Square Capital, a children's fund, a private Luxembourg bank which is now dissolved due to a history of corruption and other illegal involvement, Chrystal Capital and many others.**

I decided to submit this via the u/SuperstonkBot because I feel like **if** this is true, and **if** I've just exposed something big, then I don't want to be targeted by bots or people attempting to dox me etc.

For the record, I have a background in open-source intelligence as well as the cyber field within the computing sector. Public information is truly amazing.  

  
# 0x1 - The Start

If you aren't aware already, White Square Capital LLP has been recently 'dissolved' due to the fact that they shorted GME. People have been saying it is FUD, and I personally wanted to finally use my OSINT skills and dig into something GME related (as I haven't yet). I must say, the digging might have been worth it. Hopefully this information can benefit the people who form DDs, and those who have access to private sources to view any form of data **legally**.

I do have to admit that finding this information was fairly easy. Let me remind the hedge funds that us retail investors are smart, and we're not solely 'investors', some of us just invest on the side and are somewhat knowledgeable in this sector. What differentiates us however, is the fact that we are 'investors' as well as 'gamers', 'artists', 'influencers', etc. We are multiple hobbies in 1. You are only 1 in 1, and we're beating you at your own game. When the financial system is proven to be corrupt to the public, not only will you be targeted by the majority of the humans on this planet, but you will be absolutely hated to the guts on **everything**. Whether this is your social media, or your hedge funds website, or your private contractor.. anyone in regards to this situation preventing a deserved loss will fall victim. SEC are still paying whistleblowers to step forward. All these hedgefunds are f\*cked, and they know it.

I would like to point out that my experience within the cyber field instantly led me to believe that [https://whitesquarecapital.com/](https://whitesquarecapital.com/) was a decoy website. Reason being is that the website is low-effort, poor design, has lack of text, is unprofessional.. the list goes on. For some reason, it also has 2 "contact" buttons which don't even work. Whoever designed this website was clearly not paid enough. Or, it was intended but that only becomes true **IF** this is proven to be a decoy company that is being used for tax evasion purposes or is attempting to engage in illegal market trading tactics.  

  
# 0x2 - Reconnaissance

When you're presented with a decoy website, you're meant to perform your own format of scanning. This could be searching for endpoints (such as /home/ or /etc/) or anything that could include sensitive files on a domain. White Square Capital didn't have anything.

Another form of scanning is port-scanning. The overall result of the port-scan will allow you to see whether there are any services running on the server other than just your standard web server etc. I have completed an nmap scan, and can see that the only ports that are running on this website are 80 & 443. These are default ports for website related things. Completely nothing else running; so there is nothing majorly suspicious to document.

The second check consists of crawling the website. You click on various buttons to see if they work, and see whether they lead you to anywhere which shows you what sort of information is present and available to the public and such. Anything could **aid** your result. But, to no avail, all White Square Capital fed me was their bullshit CSS animations on the website.

Lets look up the company via public UK company records. This should lead to something, surely?

The company White Square Capital LLP was assigned company number [OC372239](https://find-and-update.company-information.service.gov.uk/company/OC372239) and is still currently labelled as 'Active'.  
If you take a look at the filing history, you'll see that we can see "Full accounts made up to 31 March 2020" which was published on 29 March 2021. If you view the **.pdf** file, and go to **page 6**, you'll see at the bottom "**Rees Pollock**" who are "Chartered Accountants" and "Statutory Auditors". Nothing abnormal -- **yet**.  

  
# 0x3 - Rees Pollock Redirect

This is ultimately where the story takes a twist and splits into 2 roads from 1. I googled "rees pollock" to see if I could find anything on them, and I could. However, when I go to [https://www.reespollock.co.uk/](https://www.reespollock.co.uk/) it's a redirect to [http://blickrothenberg.com/](http://blickrothenberg.com/) which is a tax, accounting and business advisory firm. I mean, nothing weird other than the fact that somebody who allegedly performed audits on a decoy-looking company, is now also looking like a decoy - that is ran by a big company called Blick Rothenberg. I'm trying to find a direct connection between these two other than a website redirect, but nothing yet.  

  
# 0x4 - "Off to the shore... I'll be back later."

This is the finding. This is the section which has hot info (as well as 0x5). I saw somebody on Reddit literally today using the offshore leaks website to try connect the dots with companies that could be related. I did the same, and was surprised.

So obviously, Rees Pollock sparked my interest. I decided to search for them to see if I could find any offshore companies related to Rees Pollock.. and well..

[https://offshoreleaks.icij.org/nodes/10015249](https://offshoreleaks.icij.org/nodes/10015249) = "POLLOCK HOLDINGS LTD."  
[https://offshoreleaks.icij.org/nodes/10055000](https://offshoreleaks.icij.org/nodes/10055000) = "POLLOCK S.A."

Obviously, at the moment all there is, is 2 off-shore companies with the keyword "POLLOCK" included.

BUT, what if I told you that the agent that was used for those companies has actually been dissolved since March 2018? That's right. They were [under investigation for corruption](https://citywireamericas.com/news/j-safra-sarasin-private-bank-under-investigation-in-brazil-corruption-case/a1287937), as well as [getting fined for breaches in regards to monitoring business relations.](https://www.finews.asia/finance/34254-mas-fines-bank-j-safra-sarasin-for-money-laundering-breaches-aml-cft) Interesting.. but who else happens to have that exact same agent for an offshore company? Well.. ladies and gentlemen... [Citadel Investments Group Limited](https://offshoreleaks.icij.org/nodes/10185615). I have no idea if Mossack Fonseca was a common agent to use for offshore related activities, so do correct me if it's common to see them pop up or not.  

  
# 0x5 - Additional information

This is the section which includes information that I found which I can't seem to fit in anywhere (or just to link it somehow).

Omnium LLC used to be called Citadel Solutions (September 9 2009)

Whilst performing random recon, there were individuals with LinkedIn profiles who worked at Citadel, with links to "Chrystal Capital LLP". There is also an offshore company called "Chrystal Services Limited" which happens to be registered to the exact same agent again. Mossack Fonseca. This is the only "Chrystal" key-word firm that is assigned this specific agent. Every other firm with "Chrystal" in their name does not have Mossack Fonseca as their agent.

I found an individual by the name James Douglas Innes. I am seeing appointments for Chrystal Capital Partners LLP, Chrystal Capital Property Limited, Chrystal Capital Limited, Chrystal Capital Nominees Limited, **Starlight Children's Foundation**, Peridot Acquisition Company I Limited, Peridot Acquisition Company II Limited.

I found a news article from 23 October 2016 regarding Starlight Children's Foundation. [Check the bottom](http://www.rbc.com/newsroom/news/2016/20161023-r4tk-australia_cnews.html). **Citadel**-Magnus is mentioned. In case you think this is a coincidence, Citadel-Magnus also happens to be a financial firm.

Could someone [check this](https://www.miaxequities.com/sites/default/files/alert-files/MIAX_Options_Listing_Alert_New_Class_Listings_04.2021.pdf) and let me know whether there is a link between Citadel Securities LLC and Peridot Acquisition Corp? My ape brain can't understand this data here. I just checked Google and Peridot is a "blank check company". Nice.  

  
# 0x6 - Final Thoughts

I been clicking links and digging all day with little breaks. This was very interesting. I seriously do think I have found some useful data. I also have a **strong feeling** that they are using these companies to trade stocks between themselves, as well as tax evade, and execute any other illegal market tactics. I personally think there are many more companies to unravel and expose, with much more information that could help us out to see the truth.

Please fact check everything I have included. From as far as I am aware, everything seems to check out as stated. This is **NOT** financial advice.

P.S: If anyone wants to help out, go check out the people that are registered under White Square Capital LLP and do some digging on them. Post your findings in the comments. I will see them, and include them in my future post if this does well and is actually accurate.

---

***This is not financial advice!***  
*This post was **anonymously** submitted via **[www.superstonk.net](https://www.superstonk.net/)** and reviewed by our team.
Submitted posts are unedited and published as long as they follow r/Superstonk rules.*