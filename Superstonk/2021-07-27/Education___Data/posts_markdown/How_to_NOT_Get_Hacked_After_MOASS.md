# Title: How to NOT Get Hacked After MOASS
# Author: interiumray
# Post URL: [https://www.reddit.com/r/Superstonk/comments/oshz3x/how_to_not_get_hacked_after_moass/](https://www.reddit.com/r/Superstonk/comments/oshz3x/how_to_not_get_hacked_after_moass/)


As many of you in the U.S know, cyber-attacks have been incredibly rampant. Normally, a regular person would have nothing to worry about when it comes to being hacked, however, after MOASS, every single person who has been a part of this is a target. I've been working in information security for a bit and by no means am I an expert, but hopefully, I can provide some insight that can prevent anyone from getting their spoils stolen.

# Most Common Forms of Attacks

![Verizon 2021 DBIR Summary \(worth a read\)](https://preview.redd.it/zf7wjoi16pd71.png?width=1966&format=png&auto=webp&s=ffb1ac0f0fdede26d6d0b5a27f7949a61716f66a)

Verizon conducted a study in 2021 about the most common patterns of attacks in both breaches and incidents. You can see above that breaches are most common through social engineering. We don't need to focus on Denial of Service and Web Application attacks because those are centered on a corporation's information being withheld or finding some [zero-day](https://en.wikipedia.org/wiki/Zero-day_(computing)) Below are some helpful definitions:

>**Incident vs. breach**  
>  
>We talk at length about incidents and breaches and we use the following definitions:  
>  
>**Incident:** A security event that compromises the integrity, confidentiality or availability of an information asset.  
>  
>**Breach:** An incident that results in the confirmed disclosure—not just potential exposure—of data to an unauthorized party.

Now, these are reports for corporations and not for individual people. In my opinion that doesn't mean they aren't applicable. Let's focus on social engineering and practices to avoid being phished for your information.

# Social Engineering/Phishing

For those who work in corporate environments, you have most likely gone through phishing tests and campaigns that keep employees vigilant about suspicious communication. For those that do not know, phishing is :

>**the practice of sending fraudulent communications that appear to come from a reputable source**. It is usually performed through email.

Phishing is incredibly easy to do and common. We've all received spam emails and Nigerian Prince emails, but those are usually created by non-native English speakers with purchased email addresses from random websites you visit and mass-produced to shit. They have no credibility or effort which is why Google can scan for and identify some spam automatically. However, sophisticated and targeted phishing emails are incredibly well done and easy to fall for. These emails are created by people who understand what system a person is likely to use and will copy and paste a source code for their email and plant their own link to entice you to click it.

I've had the pleasure of running a few phishing campaigns for my company and I can tell you what I would do if I were trying to make someone fall for my email and click my link. Remember, the goal of an attacker is to make you click a link that can grant them access to your system. Access can mean many things from malware that records keystrokes and websites visited and can piece together your password, to malware that holds your personal information for ransom or threatens to release private information.

To bring some perspective, an attacker can browse this sub for a couple of minutes and understand that a majority of us are on Fidelity. They can then either sign up for emails themselves and copy a [source code](https://en.wikipedia.org/wiki/Source_code) or find one online. Below I'll show you how easy it is to find the code. For those that don't know, a source code, in this case, is essentially the coded version of the email that includes all formatting so when pasted, the email looks professional and official.

![Through Gmail, you can click \\"Show Original\\" to open the code](https://preview.redd.it/hdcjqa608pd71.png?width=924&format=png&auto=webp&s=e82a8a01600b0b2c13705b34b4371d4e9964342c)

![Now you have access to the source code](https://preview.redd.it/aeg5vwo38pd71.png?width=1366&format=png&auto=webp&s=eaccda0517434ef1ff7a3f688f32f60838b1aa8d)

Now all I'd have to do is to paste the code, replace any links with the links that I want you to click and now I potentially have access when you fall for the email. It's a lot more complicated than this since you would need to write and implement usable malware but that's beyond my expertise and not important for this. All you need to know is to not fall for an email.

# What to Look Out For

So what should you look out for to not fall for these scams. Phishing emails that attempt to social engineer you will almost always have a sense of urgency in them. These can be emails from Fidelity saying there was an attempted log-in to your account prompting you to click their link to sign in or your local bank emailing to confirm you want to close your account. On paper, you may feel like you'd have to be a retard to fall for these, but I assure you are much more convincing when they've enticed some sort of emotion in you.

Look out for:

1. **sender address** \- if it is a well-created attack, then the sender's email may sound convincing. However, it is always safer to double-check and look up the address online, find any prior communication from that email, and compare it to any other results. If it feels fishy, then it's probably not legit.
2. **strong emotions** \- emails that have a sense of urgency or sound like they're offering you an amazing opportunity are usually phishing attempts. Preying on someone's fear that their account has been accessed or on someone's excitement that they were offered a black card membership from their bank is exactly the best way to get you to click on a link.
3. **awful timing** \- usually these emails get sent out at odd times and it can be an indicator. Although not full proof, it can be a sign that this is not a timely automated email from your trusted source.
4. there are more things to look out for. Here's an interesting article [https://www.phishing.org/10-ways-to-avoid-phishing-scams](https://www.phishing.org/10-ways-to-avoid-phishing-scams)

Overall, all they have to do is get you to click on a link. So beware of anything that looks suspicious. If it looks off, then contact the source and find out for information from there. If you get an email saying your account has had suspicious activity, call customer service through the number provided on their website. Don't click any links that you cannot verify.

I found this pretty interesting comparison of Google sign-in pages. One of them is the real google log-in, the other is a fake, and inputting your information to the fake one will send them straight to the attacker.

![Dark mode kinda fucks with the image. The left is the phishing page, right is the real one. ](https://preview.redd.it/rv01rtbpapd71.png?width=923&format=png&auto=webp&s=8d9085808604ebfae91a6c1c88a469c38fa07e8f)

# Multifactor Authentication

For the love of God, turn on multifactor authentication. I know it's annoying to have to sign in on your phone and your computer but it is designed to be secure. No one brute force hacks for passwords anymore. It takes an impossible amount of time that isn't worth anyone's effort. But if someone can phish for your credentials, multifactor (MFA) can provide another layer of security. Fidelity has the option to enable this and it works well. I also recommend not letting your accounts remember your device which will force you to log in every time you check your account. As annoying as this is, just remember how easy of a target you will be post-MOASS. Corporations have infosec teams and massive budgets allocated towards security to prevent breaches and they still get hacked for upwards of 750 million. MOASS would give each and every member here a net worth of at least double that. Most individuals don't have formal training in security, are heavily swayed by emotions, and don't have a data loss prevention solution on their emails.

&#x200B;

![Graphics might help ape get wrinkles](https://preview.redd.it/5q1fkgpsfpd71.png?width=416&format=png&auto=webp&s=89bc33b347ff5706e2983dd2c85475b310eb6a60)

MFA gives you a chance to prevent your information from falling into the wrong hands. If your broker does not support MFA (I'm looking at you Cashapp and your horrendous, god-awful, no password requiring bitchass) then transfer your account ASAP. If a company does not offer MFA then just imagine how many other security options they've skipped out on. The risk is never worth it.

Another point I forgot to mention: if you randomly get an MFA ping, DO NOT APPROVE IT. If you did not initiate an MFA to occur, aka you did not attempt to sign in, then it is most likely someone else trying to do it. Never share an MFA code with anyone other than the intended recipient. Pretend your MFA code or approval is worth millions of dollars because it theoretically could be. Guard it with your life.

# TL;DR

Don't trust anything that you receive. Be suspicious of everything. Don't click [random](https://www.thetek.com/oops-clicked-on-a-phishing-email-what-should-you-do/) [links](https://www.youtube.com/watch?v=dQw4w9WgXcQ). Always contact the source of information. Turn on multifactor authentication. Don't give your information to anyone. Or just stuff your millions under your mattress and bury it like [Escobar](http://gph.is/1T2J7jf).

**EDIT:** Bonus points if you find the Rickroll link and extra points if someone sends me Rick's banana video so I can make a fake link for someone to click on. This post has like 4 fake links that lead you somewhere else. All are safe 