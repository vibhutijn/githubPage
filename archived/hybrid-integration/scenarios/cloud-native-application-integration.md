---
layout: default
title: Cloud Native Apps Integration
parent: Integration Scenarios
grand_parent: Hybrid Integration
permalink: /cloud-native-application-integration
has_toc: false
has_children: false
nav_order: 5
---
{: .no_toc}
# Cloud Native Application Integrations

This scenario focus on new application architecture such as cloud-native / microservices that companies are using to modernize your applications to enable faster innovation and drive the digital transformation by composing business applications. Microservice applications are not built in isolations. They need access to data, and they need to be made available to other applications. 
   
Here are some use cases: <br>	 
 - Microservices needs to interact with other microservices  within the application
 - Process automation using microservice based applications/cloud native applications
 - Synchronizing System of  records (SORs) with modernized applications/data store

To enable innovation at this pace, business must be able to compose new applications / modernize applications using number of integration patterns as events / event-streams based interaction and APIs based interaction.  

| Business Composition |
| :-: |
| ![Business Composition](../images/business-composition.png)  |

Key considerations/elements of cloud-native application integrations:
  
 - Modular components: Small, loosely coupled and minimal interdependencies. This enable greater agility and optimization of resources.
	   
 - Prefer stateless: Components can be re-created by starting a fresh copy of an image. This provides smooth scalability and reduces environment configuration divergence.
	 
 - Image based deployment: Lightweight file based packaging of all interdependencies into an immutable image. Enable simpler re-creation of environments. 
	
 - Lightweight runtimes: This runtime starts and stop in seconds or less, reacts instantly to workload demands.
	
 - API-led intra-app communication: APIs for communication among modular components of the application. This enables common routing and load balancing and use of polyglot of runtimes types.

 - Event driven architecture: Asynchronous patterns where runtime de-coupling and system reliability is required. This improves availability, reduces response time and helps to reduce latency issues. 
	 
 - Elastic and Cloud agnostic infrastructure: Self service, self-scaling and self healing infrastructure that runs all the workloads in the same way .

 - Continuous Integration and Continuous Delivery and Deployment(CI/CD): Automation of the building, testing and deployment of code to the different environments. 
		  
 - DevOps: Near merging of development and operations. Ensures route to live is short and feedback from production is correctly prioritized.
 
 - Agile methods: Short, business-led iterations from requirements to implementations. Keeps the direction of travel in line with business expectations. 
