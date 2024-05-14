---
title: QueryService updates are blocked
date: 2024-03-27 11:00:00
resolved: true
resolvedWhen: 2024-04-02 13:58:00
# Possible severity levels: down, disrupted, notice
severity: disrupted
section: issue
---

*Update* - This incident has been resolved.

__Description__ The QueryService updater is currently not processing any updates as it's unable to process the topmost item in the queue.
This item makes the updater stall with maxed out CPU, preventing any progress from happeing.

__Expected Severity__ High for QueryService users

__Impact__ All wikis

__Links__ More information can be found in [T361551](https://phabricator.wikimedia.org/T361551).

