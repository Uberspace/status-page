# How To Status Page

## adding incidents

Incidents are created from markdown files in the `content/issues` directory.
See the [cstate wiki](https://github.com/cstate/cstate#doing-it-from-the-git-repository)
for more information.

Boilerplate:

```yml
---

title: some title
date: 2018-10-15 18:00:00
resolved: false
resolvedWhen: 2018-10-17 19:30:00
# down, disrupted, notice
severity: notice
# see `config.yml`
affected:
    - olbers
section: issue

---

Title again

---

Description
```
