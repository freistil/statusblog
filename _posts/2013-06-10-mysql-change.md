---
status: resolved
title: Database change on 2013-06-14
severity: medium
tags: database
category: Hosting
date: 2013-06-10 13:53 UTC
published: true
layout: status
---

#### ISSUE:

On Friday 2013-06-14 between 21:00 and 04:00 UTC, we are going to perform software upgrades on our database servers. These upgrades will include a new MySQL server version and an improved configuration. Both require a restart of the database service.

Since the expected downtime of a few seconds does not warrant a manual failover in most cases, we will only do a switch-over for our central database clusters but not the local databases of DrupalCONCEPT POWER and PRO plans.


#### CAUSE:

Software upgrade and configuration change.


#### TIMELINE:

* 2013-06-10 13:53 UTC -- Announcement created.
* 2013-06-15 02:14 UTC -- Maintenance finished.
