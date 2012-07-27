---
layout: status
title: High load on vm16
date: 2012-07-26 00:29:46 +0200
published: true
tags: [vm16, power12, power13, power15, power16, m17]
category: DrupalCONCEPT
severity: medium
status: resolved
---

#### ISSUE:

We are experiencing a problem that impacts the operation on VM host vm16. This impacts the following servers:

* power12.drupalconcept.net
* power13.drupalconcept.net
* power15.drupalconcept.net
* power16.drupalconcept.net
* m17.topcluster.net

#### CAUSE:

Multiple simultaneous full backups starting on several of the affected servers caused the high load.
To avoid this we distribute the backups from now on.

#### TIMELINE:

* [00:30 CET] Incident opened.
* [00:35 CET] The servers are up and running again.
