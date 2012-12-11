---
status: open
title: Announcement of changes in webserver log handling
severity: low
tags: logfiles
category: Hosting
date: 2012-11-30 14:52 UTC
published: true
layout: status
---

#### ISSUE:

We’d like to inform you in advance of changes in how we handle webserver log files for your website(s).

Until now, our webservers write daily access logs and monthly error logs to the “logs” directory in the asset file section of your website and there has been no post-processing of these files. Over time, these log files take up quite a bit of storage space, and they especially make our backup jobs longer and bigger. To make sure we can handle the growing amount of log files in the future, we are going to introduce a log file cleanup.

On **Monday, 2012-12-10**, we will start a nightly cleanup job that will delete all log files that are older than 3 months. The log files from the 2 previous months will be compressed, and the log files from the current month will remain untouched.

If you need an extensive archive of your log files (for example for analytics purposes), please make sure to _download all log files before the date stated above_ and schedule a regular download of your log files before they get deleted by our cleanup job.

As always, if you have any questions, please contact us via our [Help Center](http://support.freistil.it)!

Your freistil IT ops team.

#### TIMELINE:

* [2012-11-30 14:52 CET] Announcement published. 

*We will add more details here as soon as possible.*
