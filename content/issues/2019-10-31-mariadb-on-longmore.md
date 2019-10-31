---

title: MariaDB on longmore down
date: 2019-10-31 06:33:00
resolved: false
resolvedWhen: 2018-10-17 19:30:00
# down, disrupted, notice
severity: down
# see `config.yml`
affected:
    - longmore
section: issue

---

MariaDB on longmore down

---

Around 6:33 MariaDB on longmore has been crashed with a segmentation fault.
After being automatically restarted it initiated an auto-recovery process with an unsual long duration which is still running.
We suspect a problem with auto-recovery and are preparing for alternative ways to getting MariaDB up and running again.

We interrupted the auto-recovery process which obviously didn't show any progress or results and normally is a matter of minutes.

MariaDB is now available again, serving MyISAM tables. We are currently working on re-importing the most current state of InnoDB tablespaces.
