---
layout: status
title: Replication rebuild on ELITE backend be5 
status: resolved
category: DrupalCONCEPT
---
<p><strong>ISSUE:</strong> Database replication between the two nodes of &nbsp;DrupalCONCEPT ELITE backend be5a and be5b got broken during the day. To rebuild the replication, we have to do a complete database dump while all tables are locked. This will impair the operation of all websites that use databases on db5.drupalconcept.net while the data dump is being stored. Start of rebuild is 23:30h.</p>
<p><strong>CLOSE:</strong> Database replication has been restored.</p>