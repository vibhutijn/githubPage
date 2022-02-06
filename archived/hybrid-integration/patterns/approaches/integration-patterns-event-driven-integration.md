---
layout: default
title: Event Driven Integration
parent: Integration Patterns
grand_parent: Hybrid Integration
permalink: /integration-patterns-event-driven-integration
has_toc: false
has_children: false
nav_order: 2
---

{: .no_toc}
# Event Driven 

---

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

---

## Overview

Event-driven architecture (EDA) is a common pattern that involves production, detection, consumption, and reaction to events.

| Event-Driven Architecture (EDA) Workflow |
| :-: |
| ![eda-workflow.png](../../../resources/eda-workflow.png) |

Event Driven integrations are *triggered by an event* in one system and trigger a predefined corresponding event in another. An event can be anything that happens in a particular system that you've integrated with, such as e.g. order creation in online shopping, lead creation in a CRM, a new registration received, etc.

Event driven integrations are suitable for *functional integration*. It is not a direct candidate option for syncing all data quickly and easily. 

Event driven integrations are suitable for simple point to point data transfer when certain events take place in a system and you want to trigger corresponding actions in the other system.

---

## Enabling Event Integration for Legacy Systems

There are older systems which are not enabled to accept and act on events. You can choose to write **event adaptors**. These event adaptors intercept incoming events and pass them to the backend system in the native format. They then receive response from backend systems and put an optional outgoing event too.

| EDA Adaptor |
| :-: |
| ![eda-legacy-event-adaptor.png](../../../resources/eda-legacy-event-adaptor.png) |

---

## Event Driven Data Synchronization

Data Driven integrations have a different action that triggers synchronization. This action is a *change in the data* that you have in place in either system. This can be a *new record created* or a *change in an existing record* and more. 

| EDA Integration |
| :-: |
| ![event-driven-data-integration.png](../../../resources/event-driven-data-integration.png) |

Any change in data will trigger a sync operation of the *delta in the data* to the other system(s). For example, a new entry in the order fulfillment system should trigger an update in the CRM system to reflect the customer’s order history.

Even driven data integration makes easy to achieve an enterprise-class type of integration with easy setup and maintenance.

One example of data synchronization is necessity to access data located in the on-premises data center from an application deployed in cloud. Data driven event based integration can come to rescue here. You can add a change data capture mechanism in front of the legacy datastore which can publish the change-sets of the data in order to synchronize your datastore in the cloud.

Data driven integrations are suitable for integrations with systems where you want to keep your data in sync regardless of the event that takes place.