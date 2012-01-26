---
layout: status
title: Sporadic Varnish error pages
status: resolved
category: DrupalCONCEPT
severity: medium
---
<p><strong>ISSUE:</strong> In irregular intervals, Websites show an error page delivered by the Varnish proxy cache, mentioning "error 503" and "guru meditation".</p>
<p><strong>CAUSE:</strong> This error occurs because the Apache process Varnish to which just opened a connection immediately failed with a "segmentation fault".</p>
<p>We found the cause for those crashes in the Apache module "mod_rpaf". After deactivating the module, the segmentation faults and thus the Varnish 503 error messages stopped.</p>
