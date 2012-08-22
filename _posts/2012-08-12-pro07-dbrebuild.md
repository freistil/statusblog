---
layout: status
title: Database rebuild on cluster pro07
date: 2012-08-12 21:20:03 
published: true
tags: database,mysql
category: DrupalCONCEPT
severity: low
status: resolved
---

#### ISSUE:

Earlier today, the MySQL database on the active node on the **DrupalCONCEPT cluster pro07** became corrupted by a software crash. By doing a failover to the standby node, we were able to continue operation of the cluster.

To restore redundancy, we need to rebuild the database on the damaged cluster node. This is done by creating a consistent database export from the production node and import it on the other one. During the export process, the active database is locked temporarily which can render some websites on pro07 inresponsive. We estimate a downtime of 30 minutes, **starting at 21:30:00 UTC**.


#### CAUSE:

Database crash.


#### TIMELINE:

* [2012-08-12 21:20 UTC] Incident opened. 
* [2012-08-12 21:43 UTC] The database export has finished successfully.
* [2012-08-13 15:26 UTC] The standby database has been rebuilt and is now catching up with its production node.
* [2012-08-13 16:30 UTC] The standby database now is synchronous to the production instance again. Incident closed.
