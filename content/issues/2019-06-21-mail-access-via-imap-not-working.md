---
section: issue
title: Mail access via IMAP not working
date: 2019-06-20T22:20:47.194Z
resolved: true
resolvedWhen: 2019-06-21T07:33:47.217Z
affected:
  - uberspace6
severity: disrupted
---
_Investigating_ - We are investigating a potential issue that is causing IMAP not to work. Other services maybe affected too. We are sorry for any inconvenience this may cause you. This incident post will be updated once we have more information.

_Resolved_ - We recently changed the way how we deploy software built by ourselves from our build host to our Uberspace 6 production hosts, now being based on rsyncd. We didn't realize that rsyncd maps file ownership by numeric UIDs by default - contrary to rsync which maps ownership by usernames by default. This finally resulted in some files having wrong ownership, including the Dovecot password checking component, which broke on a about a quarter of Uberspace 6 hosts. Our monitoring tests for IMAP availability, but doesn't specifically test for working login functionality, resulting in a longer time period until we discovered them being broken by user reports.
