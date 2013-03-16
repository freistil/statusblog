---
status: open
title: repo.freistilbox.net is unreachable
severity: medium
tags: [git]
category: Hosting
date: 2013-03-16 21:06 UTC
published: true
layout: status
---

#### ISSUE:

We are experiencing a problem that impacts the operation of server repo1.freistilbox.net. This affects freistilbox git repositories.


#### CAUSE:

The host the repository server runs on is not booting anymore after a reset.

#### TIMELINE:

* [2013-03-16 21:07 UTC] Incident opened. 
* [2013-03-16 21:30 UTC] Still unreachable. Setting up new host.
* [2013-03-16 22:38 UTC] We replaced repo1.freistilbox.net with a new host under the same hostname. All freistilbox repositories are reachable again. Since the new host has a different SSH host key, you may have to renew your entry in your local known_hosts file. The new RSA key fingerprint is `b8:c8:76:ff:e2:a2:f9:6c:73:66:d4:7e:e3:0d:48:1d`.

*We are working on this issue and will add more details here as soon as possible.*
