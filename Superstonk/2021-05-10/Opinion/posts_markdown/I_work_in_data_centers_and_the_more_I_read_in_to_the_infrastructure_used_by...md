# Title: I work in data centers and the more I read in to the infrastructure used by the stock market, the more jacked my tits get that the more jacked my tits get. It’s not “just a server reboot”.
# Author: Azote_Air
# Post URL: [https://www.reddit.com/r/Superstonk/comments/n8zzi4/i_work_in_data_centers_and_the_more_i_read_in_to/](https://www.reddit.com/r/Superstonk/comments/n8zzi4/i_work_in_data_centers_and_the_more_i_read_in_to/)


EDIT: ICYMI - there were a volume mismatches blamed on server reboots.
(X) Doubt

I’m gonna keep this short and sweet:

Outside of special sauce cloud computing software the big boys (AWS, Azure, Oracle db, etc) provide their customers, the major selling point of data centers it twofold; cost through scaling/distributed use and reliability through redundancy. The first selling point you usually read about in the marketing literature from any data center service provider is their adherence to maintaining “5 Nines” or 99.999% uptime and 99.999% availability to their customers. This engineering philosophy is maintained through a variety of channels, with the key factor behind most of them being redundancy. Yes, just like with your NAS’s RAID array for your 16TB of chicken tendy memes on 3 Seagate EXOs disks, data centers also have redundancy built in, but at more levels than just storage. 

This post already feels way too long as I type it out on my phone, so I’m gonna skip the details on modern data center topology. The likelihood of arguably one of the most important set of common service trading hosts (I can practically guarantee it’s not run on just a single server let alone a single host or network switch) requiring a reboot in the middle of the day when the service doesn’t even need to meet 5 9’s on 24-7 availability is sus AF.

If you know more about the specific topology of CTA or the exchange networks in general, please shoot this down (or offer me a job to get me out of California). I’ve got a sneaking suspicion the whole “server reboot” story is basically the same line as “sorry, the ice cream machine is broke” you hear from McDonalds.