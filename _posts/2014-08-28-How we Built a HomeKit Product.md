---
Layout: post
Title: How we Built a HomeKit Product
Category: HomeKit
---

I'm very excited to write about all of the product design and outsourcing, but I'm also excited to talk about HomeKit and iBeacon.

As we work through product design we talk about a lot of different features we can add to a bluetooth enabled LED sign. Two that continually come up for us are iBeacon and HomeKit. 

Searching "How to join HomeKit", or "How to build a HomeKit accessory" yields very little valuable technical information. The best article I can find on how HomeKit will work technically is [this one](http://www.doubleencore.com/2014/07/ios-accessory-developers/) by Dave Smith. It confirms what I expected about the Bluetooth mechanisms. However, Dave couldn't go into any detail because of the MFi program NDA. 

**In fact, no matter where I go I have quickly learned that what I want to know is behind the Apple Confidential wall.**

I feel like there are 3 things I need to know before even starting enrollment:

1. What is required of a company to be approved to sign the License?
2. What does it mean to agree to the MFi License?
3. What would we get out of joining the program?

I don't want to waste my time enrolling only to be told I am not a good fit. As a startup and busy developer I just don't have time to spin cycles. I need quick answers. My biggest fear is that the MFi program is only for big manufacturing companies. One twitter friend even [asked](https://twitter.com/drewmck/status/496721901218455552): "don't you need, like, 20 lawyers to sign up for that?"

Would I be paying a royalty or big fat license fee? It looks like the financial terms are under Apple confidential and that no one can tell you Apple's business before you sign on the line. However, the FAQ does explain that there is no up-front fee to enroll (I'll talk about this more in the post on enrollment).

The most important thing I learned from the FAQ is that we can't know if the MFi program and HomeKit are right for our product until we agree to the MFi License. 

**I still just want a walkthrough of the process before I feel willing to dive in.**

I'd really like to see a ton of adoption of HomeKit. I'm an iOS developer and what's good for Apple tends to be good for me. It's a rough sell that startups and small companies have to wade through the dark to get going on a HomeKit enabled accessory. 

Even with [this amazing StackExchange answer](http://apple.stackexchange.com/questions/11794/can-a-hobbyist-or-individual-apply-for-apples-mfi-program) from Brad Larson I don't have what I need, and so it's probable that you don't either. I hope that by shedding light on our experience, more companies can follow.

As we go through the entire hardware experience, I will add our experiences with HomeKit and MFi. I'll be posting updates on this blog as they happen. I expect to share what we're experiencing throughout the process:

* Enrollment and Credit Check
* What agreeing to the license means to a startup
* Implementing the software required for HomeKit
* Outsourcing the manufacturing to a HomeKit approved manufacturer
* Packaging, Marketing, and Distribution of an MFi product

Let me know if you have any thoughts and questions, or anything in particular you'd like to hear about. You can follow via RSS, or Twitter. If you'd like weekly updates via email subscribe here.