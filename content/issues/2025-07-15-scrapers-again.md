---
title: Site Intermittently down
date: 2025-07-15 12:00:00
resolved: true
resolvedWhen: 2025-09-15 19:37:00
# Possible severity levels: down, disrupted, notice
severity: disrupted
section: issue
---
__Description__ Site Intermittently down

__Expected Severity__ Severe

__Impact__ Site is stuggling and occasionally down

__Links__ More information can be found in [T399439](https://phabricator.wikimedia.org/T399439) and [T400046](https://phabricator.wikimedia.org/T400046)

__Update__ Things seems to be better but we're still seeing occasional downtime.

__Update2__ Things have improved again since Friday (2025-07-25) when we introduced even more targeted and aggressive rate limiting; we had no related alerts until Tuesday (2025-07-29). We are still seeing some impact on the DB which will occasionally be preventing users from editing and accessing the site occasionally but right now our monitoring suggests it's only happened 3 times this morning.

__Update3__ We have seen an increased impact on the DB since our last update. We have deployed [Anubis](https://github.com/TecharoHQ/anubis) to see if that helps the situation. If users experience issues due to this change, please let us know.

__Update4__ Since deploying Anubis, the bot related traffic and load on our infrastructure has reduced significantly. After monitoring for several weeks and not receiving complaints from the community, we consider this incident resolved.