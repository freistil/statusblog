---
layout: status
title: Database overload
date: 2012-06-17 11:40:22 +0200
published: true
tags: [database,be5]
category: DrupalCONCEPT
severity: high
status: resolved
---

ISSUE:
------

We are experiencing a problem with the database cluster "be5" that impacts the operation of Drupal clusters "elite5" and "elite6". 


CAUSE:
------

The DB cluster experiences bursts of write requests to the Drupal cache tables of one database.


TIMELINE:
---------

* [11:41 CET] Incident opened. 
* [14:30 CET] The problem has subsided. We're in contact with the respective customer with the goal of using Memcache. Incident closed.
