---
layout: status
title: Mail storage migration
date: 2012-09-12 09:40 UTC
published: true
tags: email
category: Hosting
severity: medium
status: open
---

#### ISSUE:

To further enhance the performance of our email cluster, we are going to move all email data from the email cluster to a dedicated storage cluster. This maintenance procedure will start on Thursday, 2012-09-13, at 21:00 UTC.

To migrate the high volume of email data with as short of a downtime as possible, we are already synchronizing the mail cluster with the storage cluster. The first data transfer took about 27 hours. The final synchronization will take about 2,5 hours. Since this process requires us to switch off email operation, we expect a downtime of our email cluster from 21:00 to 00:00 UTC.

*Update 2012-09-14:*  All data has been transferred successfully to the new storage system. Unfortunately, not until after activating the new storage system, we realized that there was a small error in our synchronization logic. This error did not cause any data loss but may result in email messages reappearing that had already been deleted during the synchronization process. We apologize for any inconvenience this may cause. Please let us know if you need assistance in expunging previously deleted messages via support@freistil.it.


#### CAUSE:

Data migration.


#### TIMELINE:

* [2012-09-12 09:40 UTC] Incident opened. 
* [2012-09-13 23:46 UTC] Because the synchronization process takes longer than anticipated, we need to extend the downtime. ETA: 01:00 UTC.
* [2012-09-14 01:54 UTC] The synchronization process has finished successfully and mail services are activated again. 
* [2012-09-14 01:58 UTC] Some reconnecting IMAP clients report that already expunged emails had reappeared. A quick analysis shows that emails that were removed on the old storage during synchronization were not removed on the new storage.

*We will add more details here as soon as possible.*
