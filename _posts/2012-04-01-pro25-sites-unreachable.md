---
layout: status
title: Websites on PRO25 unreachable
date: 2012-04-01 00:15:02 +0200
published: true
tags: 
category: DrupalCONCEPT
severity: medium
status: resolved
---

**ISSUE:** 

We have been notified of an incident that affects operation of server pro25a. We are analyzing the issue and will add more details here as soon as possible.

After switching to the standby machine, the websites are reachable again.

Regarding to the datacenter, the network segment pro25a is a part of has been under a network attack. The issue is resolved.

**CAUSE:** Network attacks lead to congested Apache processes because data from the cluster filesystem could not be read.

**TIMELINE:**

* 00:15 Opened incident report
* 00:30 Switched to Standby server and started analysis
* 00:45 Informed datacenter about networking problems
* 20:30 Datacenter confirms network attack and resolution of the issue.