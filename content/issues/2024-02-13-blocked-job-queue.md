---
title: Platform API job queue is blocked
date: 2024-02-13 13:00:00
resolved: true
resolvedWhen: 2024-02-14 13:26:00
# Possible severity levels: down, disrupted, notice
severity: disrupted
section: issue
---

*Update* - This incident has been resolved.

__Description__ It seems the default Laravel queue stopped processing items at 2024-02-12 01:54:38 due to a hanging network connection when trying to create Kubernetes jobs

__Expected Severity__ All users affected, creation of new wikis severely broken, existing wikis missing queryservice data et. al.

__Impact__ All wikis

__Links__ More information can be found in [T357426](https://phabricator.wikimedia.org/T357426).
