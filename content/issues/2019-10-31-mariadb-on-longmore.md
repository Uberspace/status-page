---

title: MariaDB on longmore down
date: 2019-10-31 06:33:00
resolved: true
resolvedWhen: 2019-10-31 12:15:00
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

Update on 10:15:00: MariaDB is now available again, serving MyISAM tables. We are currently working on re-importing the most current state of InnoDB tablespaces.

Update on 12:15:00: Over the last two hours, all InnoDB tables have been dumped from a readonly backup MariaDB instance, putting the dumps into the production MariaDB instance. This process is now finished.
