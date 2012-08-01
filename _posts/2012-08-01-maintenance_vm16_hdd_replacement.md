---
layout: status
title: Maintenance window to replace HDD on vm16
date: 2012-08-01 16:02:07 +0200
published: true
tags: [maintenance, disk, vm16, power12, power13, power15, power16, m17]
category: DrupalCONCEPT
severity: medium
status: open
---

#### ISSUE:

Due to a harddisk failure we have to do maintenance on VM host vm16 on Wednesday, 2012-08-01, 23:00 to 03:00 CET to replace the faulty drive. Since the host has to be turned off to replace the drive, there will be a downtime of about 30 to 45 minutes.

This affects the following servers:

* power12.drupalconcept.net
* power13.drupalconcept.net
* power15.drupalconcept.net
* power16.drupalconcept.net
* m17.topcluster.net

#### TIMELINE:

* [16:05 CET] Maintenance window announced.
* [23:00 CET] System shutdown to replace disk.
* [2012-08-02, 00:30 CET] The system and its VMs are running with decreased performance due to the RAID rebuild.
