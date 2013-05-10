---
status: open
title: Mail cluster downtime for storage migration
severity: medium
tags: [mail,storage]
category: Hosting
date: 2013-05-10 10:03 UTC
published: true
layout: status
---

#### ISSUE:

Over recent weeks, we had multiple customers sending support requests because of inconsistent mailbox content and even lost emails. We've tracked the cause down to an incompatibility between the IMAP server and our storage cluster. 

To prevent these problems for the future, we've decided to do an emergency data migration (~300 GB of email) to another storage solution. 

To avoid any risk to data consistency, we need to shut down our email cluster during the migration, which will take place

  **from Friday, 2013-05-10 18:00 UTC (20:00 CEST), to Saturday, 2013-05-11 05:00 UTC (07:00 CEST)**

During this time, access to mailboxes will not be possible. Incoming email will be delivered as soon as the mail cluster goes back online.

We apologize for the short notice. Because email is a very important communications tool for our customers, we decided to act fast.


#### CAUSE:

Email storage issues.


#### TIMELINE:

* 2013-05-10 10:03 UTC -- Incident opened. 

*We are working on this issue and will add more details here as soon as possible.*
