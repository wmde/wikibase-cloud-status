---
title: Elevated Prometheus spend
date: 2023-12-14 00:00:00
resolved: true
resolvedWhen: 2024-03-28 12:50:00
# Possible severity levels: down, disrupted, notice
severity: notice
section: issue
---

*Update* - This incident has been resolved.

We noticed very high spending on Prometheus metric ingestion, such that it's basically approaching our compute spend.
More information can be found in [T356049](https://phabricator.wikimedia.org/T356049).
This isssue has no user-facing impact.
