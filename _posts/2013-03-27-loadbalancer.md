---
status: resolved
title: Loadbalancer outage
severity: high
tags: network,loadbalancer
category: Hosting
date: 2013-03-27 00:29 UTC
published: true
layout: status
---

#### ISSUE:

We are experiencing a problem with the routing of IP subnets that impacts most of our infrastructure. 


#### CAUSE:

Not yet determined.


#### TIMELINE:

* 2013-03-27 00:29 UTC -- Incident opened. 
* 2013-03-27 00:35 UTC -- Routing of all failover subnets to our main loadbalancer is down. We've opened a support ticket with the datacenter.
* 2013-03-27 00:57 UTC -- Call to Hetzner Support. We're asked to wait for a response via email.
* 2013-03-27 01:30 UTC -- Call to Hetzner Support. We explain the severity of the outage and demand escalation of the problem. We're promised expedited handling of the issue and quick feedback on any progress.
* 2013-03-27 01:59 UTC -- Some IP addresses come back online.
* 2013-03-27 02:06 UTC -- Hetzner informs us via email that the routing has been restored completely.
* 2013-03-27 02:18 UTC -- Call to Hetzner support to inform them that only parts of the subnets are online again. The support agent asks us to give them a complete list of the affected subnets and their intended routing. 
* 2013-03-27 02:40 UTC -- We have analyzed the remaining routing problems and it seems that only a quarter of the biggest subnet has been reactivated. We inform Hetzner of our findings.
* 2013-03-27 02:54 UTC -- All remaining IP addresses are online. 

We expect to get an official statement from Hetzner about the root cause of this outage in the morning and are preparing an extensive post-mortem that we will post on our blog.
