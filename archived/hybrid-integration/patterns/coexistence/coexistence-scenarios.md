---
layout: default
title: Co-existence Scenarios
parent: Integration Patterns
grand_parent: Hybrid Integration
permalink: /coexistence-scenarios
has_toc: false
has_children: false
nav_order: 11
---

{: .no_toc}
# Co-existence Scenarios

Modernization of monolithic application to microservice based application needs monolithic & modern application to co-exist until the modernization is complete. To facilitate this co-existence, a co-existence integration layer needs to be built using various integration patterns across on-premise and cloud. 

Thus, the co-existence layer is a by-product of incremental modernization to deliver modernized functionality into production in controlled risk adverse manner.

Co-existence supports multiple patterns for the incremental modernization in both the scenarios listed below:

## Scenario 1: Current state reads from and writes to modernized data

| Current state reads from and writes to modernized data |
| :-: |
| ![current-to-modernized.png](../../../resources/current-to-modernized.png) |

- Current state datasets are decommissioned; and the data is completely moved to the modernized state with its access is guarded by the domain/data services designed around that dataset. The current state reads and updates this data residing in the target state.
- This pattern can be used when modernized data to current state data transformation complexity is minimal and performance requirements are relaxed, thereby allowing real time transformation for reading & writing to modernized data from the current state.

- **Examples** : 
	- A status code, indicator, or flag value is needed on the current state that was transformed into a new value set when loaded to the modernized data model.
	- A complex batch job, in part or is not modernized along with a given modernization roll out, but a status code or aggregated value needs to be transformed and updated on the modernized database since the current state equivalent table was decommissioned.

---

## Scenario 2: Modernized state reads and writes to current state data

| Modernized state reads and writes to current state data |
| :-: |
| ![modernized-to-current.png](../../../resources/modernized-to-current.png) |

- Modernized data needs a subset of data from the current state (e.g. master data). A functionality is moved incrementally and the modernized data needs to update a subset of data from the current state.
- This pattern supports incremental modernization roll out where modernized data and current state data can be brought together in context within the modernized application.

- **Examples** : 
	- The modernized solution needs customer data reflected in the modernized user interface that has not yet been added to the modernized data model (e.g. customer name).
	- Critical business owned applications need replica of current state key data that cannot be changed in the timeframe planned for a given modernization roll out.
