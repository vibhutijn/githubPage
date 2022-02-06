---
layout: default
title: Saga
parent: Integration Patterns
grand_parent: Hybrid Integration
permalink: /txn-patterns-saga
has_children: false
nav_order: 31
---

{: .no_toc}
# Saga

Saga is an architectural pattern that provides an elegant approach to implement a transaction that spans multiple services and is asynchronous and reactive in nature. Each service in a Saga performs its own local transaction and publishes an event. The successive services listen to that event and perform the next local transaction. If one transaction fails for some reason, the Saga also executes compensating transactions to undo the impact of the preceding transactions.

| Saga |
| :-: |
| ![Saga Flow](../../../../resources/saga-flow.jpg) |


**Different ways to implement the Saga pattern**

There are two logical ways to implement the Saga pattern: choreography and orchestration.

**1. Choreography**

In the Saga choreography pattern, each individual microservice that is part of a process publishes an event that is picked up by the successive microservice. You must make decisions early in the microservice development lifecycle to understand if it will be part of a Saga pattern or not, since you must choose an appropriate framework that will help implement this pattern. To adopt a particular framework code, the microservice must be decorated with annotations, class initializations, or other configuration changes. In the Saga choreography pattern, the SEC (Saga Execution Coordinator) can be embedded within the microservice or in most of the scenarios is a standalone component.

**2. Orchestration**

As the name of the Saga orchestration pattern suggests, there is a single orchestrator component that is responsible for managing the overall process flow. If the process encounters an error while calling any individual microservice, then it is responsible for calling the compensating service too. The orchestrator helps model the Saga flow, but also relies on the underlying framework to call the services in a sequence and make compensating calls if any of the services fail.

For more in depth view on the saga pattern, please refer [here](https://developer.ibm.com/depmodels/microservices/articles/use-saga-to-solve-distributed-transaction-management-problems-in-a-microservices-architecture/){:target="_blank"}.
