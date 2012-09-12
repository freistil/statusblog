---
layout: status
title: 
date: 2012-09-12 09:40 UTC
published: true
tags: email,
category: Hosting
severity: medium
status: open
---

#### ISSUE:

To further enhance the performance of our email cluster, we are going to move all email data from the email cluster to a dedicated storage cluster. This maintenance procedure will start on Thursday, 2012-09-13, at 21:00 UTC.

To migrate the high volume of email data with as short of a downtime as possible, we are already synchronizing the mail cluster with the storage cluster. The first data transfer took about 27 hours. The final synchronization will take about 2,5 hours. Since this process requires us to switch off email operation, we expect a downtime of our email cluster from 21:00 to 00:00 UTC.


#### CAUSE:

Data migration.


#### TIMELINE:

* [2012-09-12 09:40 CET] Incident opened. 

*We will add more details here as soon as possible.*
