---
layout: default
title: Data Adapters
parent: Integration Patterns
grand_parent: Hybrid Integration
permalink: /integration-patterns-data-adapters
has_children: false
nav_order: 23
---

{: .no_toc}
# Data Adapters

<br>

| Data Adapters |
| :-: |
| ![data-adapter.png](../../../../resources/data-adapter.png) |

- Data Adapter Pattern is used in data consolidation scenarios to incrementally move the data traffic from legacy source / targets to strategic / modernized source / targets.
- This pattern provides flexibility to modernize both legacy data source and data target platforms independently and incrementally.
- Data Adapter is capable of consuming data from both legacy and modernized data sources, and is configurable to send all data to either legacy DB or strategic / modernized DB or both.
- During the coexistence state, the data adapter can be configured to send all data to both legacy and strategic / modernized databases.
- Upon successful data reconciliation, the Data Adapter can be configured to send data only to the modernized DB (target state), allowing the business to discontinue legacy databases and legacy application sources.

**Benefits**

- No changes to legacy and strategic / modernized data sources & targets.
- Data sources and data targets can be modernized independently and incrementally.
- Ability to reconcile data during coexistence elevates confidence with modernization.
- Ability to fallback to legacy systems, lowers business risk.
