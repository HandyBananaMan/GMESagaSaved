# Title: LAST WARNING FROM A TECHNICAL ARCHITECT
# Author: YharnamHF
# Post URL: [https://www.reddit.com/r/DDintoGME/comments/n8youe/last_warning_from_a_technical_architect/](https://www.reddit.com/r/DDintoGME/comments/n8youe/last_warning_from_a_technical_architect/)


First let me say this is not financial advise, but for certain some technical advise on RHs failure.

Working as an IT architect for various large institutions during my career and now, I can tell you....THERE IS NO FUCKING SERVER FAILURE AT THESE KIND OF COMPANIES....EVER

No single medium sized company would let you implement their system...whatever it may be... in a SPOF (Single Point Of Failure) setup in a production (live) environment. 

It is MANDATORY(!!BY REGULATION) by various IT regulatory obligations, that while handling sensitive real-time data there must be a disaster recovery plan in the form of a instant-failover once a failure occurs to the production system. This ofcourse depends on juristiction, but I can personally guarantee you the following: Not a single CTO would let their systems be implemented without said disaster recovery.

My guess would be that it is an orchestrated technical setup in their system, to initiate these downtime frames. There is no other logical or technical explanation..

TLDR;

PLASE GTFO ROBINdaHOOD