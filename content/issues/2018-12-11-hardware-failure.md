---
section: issue
title: Resolved - hardware failure
date: 2018-12-11T14:00:00.000Z
resolved: true
resolvedWhen: 2018-12-11T14:45:00.000Z
affected:
  - corvus
  - fomalhaut
severity: disrupted
---
_Investigating_ - hardware failure, we're moving the VMs to a different machine at the moment.

_Update_ - Found log entry: `Memory #0x08 | Correctable ECC (@DIMMO6(CPU1))`, we're replacing the memory on the machine. VMs are moved to another host and are booting up.

_Update_ - Migration complete. Systems are up and running.
