---
layout: default
title: Key Aspects
parent: Hybrid Integration_
# Change the parent name to hide the file, which content has been merged into the main Hybrid Integration part
permalink: /key-aspects
has_toc: false
has_children: false
nav_order: 1
---
{: .no_toc}
# Key Considerations of Hybrid Integration 

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

While working in the multicloud and Hybrid cloud integration, each cloud provider or non-cloud provider has similar challenges around how to surface or extract the data and  appetize and expose the data to other cloud or no cloud destination with the help of consistent integration solution.  

| Hybrid or Multicloud Challenges |
| :-: |
| ![Hybrid or Multicloud challenges](./images/multicloud-challenges.png) |

This aims to provide similar and consistent integration solution across Hybrid or Multicloud, provide better business collaboration and experience, and reducing cost for the customer.  

Please find below key considerations for Hybrid and Multicloud scenarios.

### Scope of Management  

This is one of major consideration which means "how much do you want to manage yourself (both in terms of apps and integration)”:
 1. Self Managed Pets (centralized/big bang) self managed deployment on on-premise
 2. Platform managed Cattles (lightweight) deployment on private cloud
 3. Fully managed PaaS / SaaS on private/public cloud. 


###  Network and Security (Identity and Access Control)

Each cloud provider / non-cloud provider has their own network and security solution. Considerations to deal such challenges as below:
 1. Choosing / bridging domains 
 2. Private, Partner, Public  
 3. Handling distributed IAM solution in hybrid / multicloud

### Data Sovereignty / Privacy  

Customer requirements around data sovereignty and privacy in hybrid / multicloud. Few considerations to deal such requirements as depicted below:
 1. Encryption
 2. Archiving /Deletion
 3. Legislative Information domains

 
### Ownership Boundaries

Basic considerations around application / solution boundaries.
 1. Application boundaries - How do applications sit within clouds and do they span clouds?
 2. Application between Clouds or within Clouds: if an application is partially migrated to cloud, how this is going to be managed? 
 3. Different boundaries at each level: between customer and vendor, then between groups within customer at each level
    - Infrastructure level 	
    - Platform level 	
    - Software level

### Portability 

This helps enable the hybrid and multicloud deployment. This is important consideration as depicted below:
 1. Cloud native principles
 2. Orchestrated containerization
 3. Image based deploy 
 4. Write once deploy to any cloud (cloud agnostic)
 5. Distributed deployment

 
### Asynchronous Transport Backbone  

This is going to important aspects to integrate hybrid / multicloud to address latency, performance and high throughput applications using asynchronous cloud messaging while synchronous connectivity and batch integration still valid in appropriate scenarios/use case. Few considerations for asynchronous messaging/transport.
 1. Messaging vs Events
 2. Event Replication
 3. When/Where to aggregate
 
### Latency

This is going to be one important consideration when application or data are located in different data centers/region on hybrid / multicloud, can bring latency in integration solution. This needs considerations as below:
 1. Data location
 2. Data replication close to consumer  
 3. Distance / Bandwidth
 4. Caching / Local data optimization 
 5. Reducing layering, but keeping isolation and abstraction 
   
 
### SaaS Integration  

With hybrid / multicloud adoption, customer are started moving from self managed enterprise solution to cloud managed SaaS solution, which required below considerations for integration solution:
 1. Cloud App Connectivity
 1. Business data aware Connectors
 1. Out of the Box Integration Patterns

### Monitoring and Operations  

With hybrid / multicloud adoption, customers' workload are distributed across cloud / non-cloud destinations, which required integrated monitoring and operation-based solution. Here are few considerations as below:
 1. Viewing and diagnosing across boundaries
 2. Collation and aggregation of logs across and end-to-end solution

### Migration and Modernization  

This aspects required to understand with respect to application refactoring/modernization to move on, and/or between clouds. Following considerations for integration solution associated with impacted applications:
 1. Co-location and isolations of integrations with its applications
 2. Lightweight integration services
 3. Lift and shift or refactor

### Decentralization

In distributed hybrid / multicloud environment, integration solution required to be distributed and decentralize to solve the below problems:
 1. Federated management of runtimes and gateways
 2. Simplifying cloud to ground hybrid solutions
 3. Solutions spanning multiple clouds

### Need of  Integration Platform as a Service (iPaaS)

Currently customers are using Enterprise Service Bus, enterprise messaging middleware, batch or ETL solutions to solve the enterprise wide integration problems. This is not going to solve integration problems in hybrid / multicloud environment. This arise the need of below considerations:
 1. Diverse integration capabilities 
 2. Cloud readiness integration platform
 3. Simplified self-provisioning of integration capabilities 
 4. Simplified governance of integration services 
 5. Low code and no code tooling for new line of business users 
 6. Cloud services applications development and execution 


