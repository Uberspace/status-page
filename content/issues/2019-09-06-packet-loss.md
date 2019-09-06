---
section: issue
title: Packet loss
date: 2019-09-04T20:00:19.700Z
resolved: true
resolvedWhen: 2019-09-05T08:00:19.724Z
affected:
  - FRA3
severity: disrupted
---
Due to a broken switch we observed some packet loss on our network in consequence of some interfaces that had high error rates. We've replaced the connection with a new one on another port. After that the packet loss vanished but we observed other, not user facing errors. We decided to replace the whole switch with a spare part, this led to some very short downtimes of IPv4 and a little longer on IPv6. All problems are fixed now and we are at normal operation.

 We are sorry for any inconveniences this may have caused cause you.
