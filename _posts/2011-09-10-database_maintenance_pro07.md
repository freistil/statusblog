---
layout: status
title: Database maintenance on PRO/shared cluster pro07
status: resolved
category: DrupalCONCEPT
---
<p><strong>ISSUE:</strong>&nbsp;Probably due to the system overload yesterday, database replication between DrupalCONCEPT PRO/shared cluster nodes pro07a and pro07b broke. To rebuild the replication, we have to do a complete database dump while all tables are write locked. This will impair the operation of all websites on that cluster while the data dump is being stored (estimated downtime: &nbsp;1h). We will start the rebuild today at 23:30h.</p>
<p><strong>UPDATE 0:26h (2011-09-11):</strong> The database dump has been successfully created and transferred to node pro07b.</p>
<p><strong>CLOSE:</strong> Replication is working again.</p>