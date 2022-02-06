---
layout: default
title: Strangler Pattern
parent: Integration Patterns
grand_parent: Hybrid Integration
permalink: /txreqmgmt-patterns-strangler
has_children: false
nav_order: 41
---

{: .no_toc}
## Strangler Pattern

| Strangler Pattern |
| :-: |
| ![enter image description here](../../../../resources/strangler.png)

- While the modernization is in progress, there is a need to route the incoming requests to either current state or target state based on a pre-determined logic. Strangler pattern helps us do this. 

- Strangler component helps us to incrementally migrate a legacy system by gradually replacing specific pieces of functionality with new applications and services. As features from the legacy system are replaced, the new system eventually replaces all of the old system's features, strangling the old system and allowing you to decommission it.

- This strangler component could be a standalone component sitting outside the application or a wrapper of core programs sitting inside the current state.

- The strangler component captures requests initiated and does one of the following:
    - Streams them to the modernized side for synchronization purposes
    - Calls either current or modernized state applications
    - Calls both current and modernized state applications
    
- The strangler component could use a 'routing store' that keeps logic for request handling and it can be based on request type or/and specific field(s) values (i.e. account type or branch based).
