---
title: Tough week | Redis got chocked | Chrome Extension got unpublished
date: 2019-08-18 11:09:00 Z
categories:
- Product
- Pladio
tags:
- Product
- Usage
- Data
- Metrics
Key: 
---

Earlier this week, one of our developer came to know that some of the bad code was pushed to the main code of the chrome extension. That code was published to the production and to stop users from getting the bad experience, we decided to unpublish the chrome extension.

**What was the chrome extension issue**

The code which was hitting the main API was changed to hit the `localhost` in the for some testing. After successful testing, this localhost code was converted to ZIP and published to the production chrome extension.

Our chrome extension takes some time to publish because of some permissions that we require to function properly. Therefore, it goes through the manual review.

We are trying to take these permissions away as we are not making any use of them.

On Sunday, the users were not able to use any of our clients because of the following redis issue.

**Redis issue**

We are still not sure about the Redis issue. Most probably it happened because of snapshot file becoming so big that it started refusing any of the incoming requests from the main server and as the main server is dependent upon redis to work properly no response was going to our clients.

**Redis issue is fixed now but we are still waiting for the manual review in the case of chrome extension.**

## This week numbers

**Number of users gained: ** 3

We are building a small feature before moving toward full marketing and sharing it over different channels.

Thanks for reading. We will get back with the new numbers next week.

Please share Pladio with your friends.