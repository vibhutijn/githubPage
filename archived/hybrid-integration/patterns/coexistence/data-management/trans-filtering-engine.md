---
layout: default
title: Transformation & Filtering Engine
parent: Integration Patterns
grand_parent: Hybrid Integration
permalink: /trans-filtering-engine
has_toc: false
has_children: false
nav_order: 22
---

{: .no_toc}
# Transformation & Filtering Engine

<br>

| Filtering Engine |
| :-: |
| ![filtering-engine.png](../../../../resources/filtering-engine.png) |

When an event driven integration approach is followed, there could be lot of unwanted events being raised. 

This pattern helps to reduce this noise and process only relevant events by applying transformation and filtering rules and caching processed events.
    
-   Filtering and transformation rules are used to:    
    -   Drop irrelevant events (i.e. CDC might send everything)
    -   Set event destination
-   Event cache is used to:    
    -   Filter out duplicate events
    -   Aggregate low-level events
-   Transformation engine is used to:
	- Apply event transformation logic   
	- Applying data transformation rules, splitting complex events and aggregating low level events
	- Defines destination for transformed events
