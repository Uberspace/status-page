---
section: issue
title: hardware failure
date: 2018-12-11T14:00:00.000Z
resolvedWhen: 2018-12-11T14:19:18.155Z
affected:
  - corvus
  - fomalhaut
severity: disrupted
---
_Investigating_ - hardware failure, we're moving the VMs to a different machine at the moment.

_Update_ - Found log entry: `Memory #0x08 | Correctable ECC (@DIMMO6(CPU1))`, we're replacing the memory on the machine. VMs are moved to another host and are booting up.
