---
title: Possible DB downtime
date: 2024-08-28 14:52:00
resolved: true
resolvedWhen: 2024-08-28 15:16:00
# Possible severity levels: down, disrupted, notice
severity: distrupted
section: issue
---

**edit** this didn't go quite as smoothly as expected; seems to have recovered after around 20mins + restarting the SQL secondary

__Description__ As a part of routine maintenance we may experience some database downtime as we change a configuration setting on the DB see: T373448

__Expected Severity__ Possible short term disruption; wikis may be read only

__Impact__ Possible short term disruption

__Links__ More information can be found in [T373448](https://phabricator.wikimedia.org/T373448).
