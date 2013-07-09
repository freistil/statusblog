---
status: open
title: "Change announcement: Moving db8a to dedicated rack"
severity: medium
tags: [database, change announcement]
category: Hosting
date: 2013-07-05 15:56 UTC
published: true
layout: status
---

#### ISSUE:

To reduce the impact of network issues on our database infrastructure, we are going to move the MySQL node db8a.drupalconcept.net to a server rack exclusively used by us. 

We will execute this change on Tuesday 2013-07-09 between 19:00 and 21:00 UTC (21:00 - 23:00 CEST).

We do not expect any downtime since we will switch to the spare node in advance of this maintenance.

These are the DrupalCONCEPT clusters affected by this change:

* elite5 (all sites)
* elite6 (some sites)
* pro20
* pro35

We will inform all customers affected by this change directly and post updates on our status blog.

#### CAUSE:

Infrastructure change to improve resilience against network issues.

#### TIMELINE:

* 2013-07-05 15:30 UTC – Announcement created.
* 2013-07-09 09:45 UTC – The IP address of db8.drupalconcept.net will change. If you are using 178.63.45.89 directly now this **will not work** after the move anymore. You will have to change it afterwards. If you are using the hostname directly you will not be affected.
* 2013-07-09 20:15 UTC – The move started one hour late due to coordination problems with the datacenter. The time to finish the move will be delayed.
* 2013-07-09 21:00 UTC – The datacenter handled the move very fast and we are happy to inform you that the move and adaption of db8a to the new place has already finished. Replication is reactivated. No downtimes occured. 