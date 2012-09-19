---
layout: status
title: Database replication rebuild on PRO32
date: 2012-09-19 10:07 UTC
published: true
tags: [mysql, pro32]
category: DrupalCONCEPT
severity: medium
status: resolved
---

#### ISSUE:

Database replication between the two nodes of &nbsp;DrupalCONCEPT PRO Cluster PRO32 got broken during the night. To rebuild the replication, we have to do a complete database dump while all tables are locked. This will impair the operation of all websites on PRO32 while the data dump is being stored. Start of rebuild is 23:30h.


#### TIMELINE:

* [11:09 CET] Incident opened. 
* [00:00 CET] Rebuild start.
* [00:39 CET] Rebuild successfully completed. The necessary database lock took less than a minute, so operations were impaired for only this time.
