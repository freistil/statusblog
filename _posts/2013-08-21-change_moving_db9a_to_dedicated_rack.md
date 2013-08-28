---
status: resolved
title: "Change announcement: Moving db9a to dedicated rack"
severity: medium
tags: [database, change announcement]
category: Hosting
date: 2013-08-21 08:00 UTC
published: true
layout: status
---

#### ISSUE:

To reduce the impact of network issues on our database infrastructure, we are going to move the MySQL node db9a.drupalconcept.net to a server rack exclusively used by us.

We will execute this change on Tuesday 2013-08-26 between 19:00 and 21:00 UTC (21:00 - 23:00 CEST).

We do not expect any downtime since we will switch to the spare node in advance of this maintenance.

We will post updates on the change on our status blog.

#### CAUSE:

Infrastructure change to improve resilience against network issues.

#### TIMELINE:

* 2013-08-21 08:30 UTC – Announcement created.
* 2013-08-26 18:40 UTC – Initiated failover to db9b and set up db9a for new environment.
* 2013-08-26 19:00 UTC – Move started on time.
* 2013-08-26 19:25 UTC – db9a is back up at its new location in our rack. db9b will stay the active node for a while. Replication is fully working again.
* 2013-08-28 03:00 UTC – db9a is the active node again.
