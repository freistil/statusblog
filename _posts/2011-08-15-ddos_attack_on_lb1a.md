---
layout: status
title: DDOS attack on lb1a
status: resolved
category: DrupalCONCEPT
---
<p><strong>ISSUE:</strong> Between <em>19:49 and 19:58</em> CEST today, we've experienced a DDOS attack on a customer website we're hosting on an&nbsp;DrupalCONCEPT ELITE cluster. The load balancer in front of the Drupal web servers received about <em>10.000 HTTP requests per minute</em> but always limited the number of concurrent connections to about 4000. During this time, the Drupal frontends each delivered about <em>80 requests per second</em>. After the request wave subsided, all servers immediately resumed normal operation.</p>
<p>Unfortunately, we can't simply declare this incident an involuntary load test because a number of customer websites served by the affected load balancer were rendered unresponsive by the attack. Because of the connection limit, some of the legitimate visitors were not able to reach those websites during the attack.</p>
<p>We apologize to all affected customers for the service interruption. We'll work on ways to better protect our infrastructure and our customers' websites from these malicious attacks.</p>