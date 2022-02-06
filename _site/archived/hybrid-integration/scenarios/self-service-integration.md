---
layout: default
title: Self-Service Integration
parent: Integration Scenarios
grand_parent: Hybrid Integration
permalink: /self-service-integration
has_toc: false
has_children: false
nav_order: 6
---
{: .no_toc}
# Self-Service Integration

<br>

Integration is no longer preserve of a central dedicated team of integration specialists. Different people in more diverse role are now involved in performing integration, and there is a significant shift towards the lines of business solving their own integration challenges.  

| User Community |
| :-: |
| ![](../images/hybrid-user-community.png) |

Self-service integration tools allow shadow or non-Integration specialist to connect apps and services in an intuitive and step-by-step experience without much experience and training. 

| Self-service Integration |i
| :-: |
| ![](../images/self-service-integration.png)

Please find below considerations for self-service integration:

 - There has to be low code / no-code based integration tooling available, which can be simply used to connect app and data without much experience and training.
 
 - Application Adapters/connectors should be able to connect with native Integration layer of new applications/SORs. The connectors should leverage one or more of the hybrid patterns (API, Event Driven) considering API Management tools & services, MQ, Event Stream based on candidate system/application.
   
 - Consider app/data Integration (protocol, data format, data mapping) & transformation to address polygot technologies and SORs.Ensure that data from new applications are supported by XForm (ETL/ELT process) adopted by the self-service integration platform.
 
 - The platform and its connectors should support protocols like JSON, RPC, HTTP, HTTPS, SOAP.
 
 - A lightweight data integration layer should be used to enable / enrich connectors for seamless integration with external systems and their diverse data types.
 
 - The major components of self service integration platform – UI, Connectors, workflow orchestration engine and data integration shall be built using Microservice pattern.
 
 - Use lightweight technologies like Springboot, Node.js, Angular. This will help with faster spin-up of containerized microservices built with docker optimization approach(fast build time, smaller image size, etc).
   
 - Ensure integrators are able to visualize a personalized dashboard of their individual integration journey.

 - The Deployment of platform components/features(e.g. Templates, Connectors, UI changes, workflows) should be GitOps enabled.
   
 - The platform should be able to scale dynamically based on number of integrators, no. of applications to be integrated and load volumetric. The containerization of platform components and following of 12 factor principle during design/build time is key  to scalable, resilient integration system 
 
 - The integration patterns must ensure that data in transit are
   encrypted and securely transferred

