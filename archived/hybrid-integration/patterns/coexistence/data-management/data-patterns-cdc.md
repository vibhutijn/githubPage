---
layout: default
title: Change Data Capture
parent: Integration Patterns
grand_parent: Hybrid Integration
permalink: /data-patterns-cdc
has_toc: false
has_children: false
nav_order: 21
---

{: .no_toc}
# Change Data Capture

<br>

| Change Data Capture |
| :-: |
| ![cdc.png](../../../../resources/cdc.png) |

- CDC is an approach to data integration that is based on the identification, capture and delivery of the changes made to enterprise data sources. This pattern is used to replicate legacy application's state to modernized application(s).
- CDC can be used when changes to core programs at the source state are not feasible or yet to be planned.
- It is a set of software design patterns used to determine and track the data that has changed so that action can be taken using the changed data.
- CDC could be implemented in both unidirectional and bidirectional data synchronization.
- CDC occurs often in datawarehouse environments since capturing and preserving the state of data across time is one of the core functions of a data warehouse, but CDC can be utilized in any database or data repository system.
- CDC can deliver the change logs to target databases, message queues, or an extract, transform, load (ETL) solution.
- CDC is mostly supported by out-of-the-box technical components without any changes to core programs.
