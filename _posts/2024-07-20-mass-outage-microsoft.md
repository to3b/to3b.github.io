---
layout: post
title:  Y2K came 24 years too late - Mass outage of Windows computers.
---

## A little bit of background



## What actually happened

A Cyber Security company called CrowdStrike who equips potentially billion of computers with antivirus software pushed an update to most if not all online Windows computers at version 7.11 or above (Windows 7 to 11+?) during the hours of Friday, July 19, 2024 04:09 UTC and Friday, July 19, 2024 05:27 UTC, the update attempted to improve their current antivirus program but instead there was a bug in the code that was pushed that ended up giving every single computer a [logic error](https://en.wikipedia.org/wiki/Logic_error) that unintentionally gave each computer a BSoD (Blue Screen of Death) and rebooted asking to be put in Recovery Mode.

## The impact of this event



## Solution (is there one?)

CrowdStrike have put out multiple statements and atleast one about a quick fix solution to the problem. They suggested that the user boots into Safe Mode on their computer and navigates to '%WINDIR%\System32\drivers\CrowdStrike' and delete the file called 'C-00000291*.sys'. I personally believe they need an actual wide spread solution because with this currect solution you need to do it to every computer individually, manually. Which if you're dealing with a setup like this: 

![Mass BSoD](https://github.com/user-attachments/assets/fe37940b-e1cd-4928-9013-892ccca6f862)

Then that is the opposite of ideal. -

Personally, I can think of a way better solution to resetting every machine back to where it used to be, I am not sure why they didn't initally suggest this but my idea is to just basically do the process they are wanting the users to do manually and just push a script to everyone that deletes the file because I believe you should have access to the internet still through safe mode, so they could just either push an update (if the program is still running) or... Have the script to delete the file avaliable on their website so that an IT Admin could potentially remote into each pc and run the script if everything is setup for that. The current solution that they have doesn't seem too viable to me, although it has been awhile and things such as flights seem to be going ahead, I don't know what system they're using though.


## Final thoughts

Effectively, CrowdStrike initiated a cyber attack on themselves with no immediate easy fix. CrowdStrike will need to go over their procedures and evaluate how this happened in the first place, who did it, why was there no prior checks before pushing the update and what barriers they need to put in place to ensure that this type of self-inflicted cyber attack doesn't happen again. The CEO of CrowdStrike put out a statement saying ""

NOTES:

They do have a remote virtual server solution to the problem.
Find CEO's statement.
Impact was that flights were effected,
