---
layout: default
title: Digital Integration
parent: Hybrid Integration_
# Change the parent name to hide the file, which content has been merged into the main Hybrid Integration part
permalink: /hybrid-digital-integration
has_toc: false
has_children: false
nav_order: 20
---
{: .no_toc}
# Digital Integration

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

This is a transformation journey that requires business transformation, building new architectural layers, adopting new architectural patterns, modernizing & moving existing workloads, exposing existing processes/services as APIs: 
- Engage customers anytime anywhere
- Paradigm shift from business processes to customer journeys
- Offer a seamless customer experience beyond the original line of businesses
- Become agile to respond to market and regulatory changes
- Keeping innovation at the forefront - not just in business but also in technology (bringing new ideas to market rapidly)
- Extreme automation to reduce costs

Following image gives an overview of what it takes to become digital:

| **Digital Mandates** |
| :-: |
| ![Digital Mandates](../resources/digital-mandate.PNG) |

From an architecture & technology perspective this translates to:
- Building new architectural layers and patterns (Microservices, API, EDA, AI/insights)
- Modernization to remove impediments to rapid business transformation and innovation
- Adopting new technologies and development practices
- Reducing technical debt
- Exposing processes and data to partner and developer ecosystem to accelerate innovation (in a secure way ofcourse)
- Cloud migration/development
- Ensuring IT systems are resilient and available 
- Automation of software development processes

What it means is a holistic approach is required for Digital transformation. i.e.:
- Running siloed initiatives (e.g. enhancing systems of engagement, modernizing applications) is not enough
- Just developing systems of engagement will not realize the objectives of digital transformation
- There is a need for well-defined delivery practices, architecture and standards
- Services & API are the backbone of any digital strategy. 80% of the effort is in Integration to backend systems and Process Digitisation

---

## Key Questions to Ask

It is essential to understand client's digital strategy and their progress before proposing changes or revamping their strategy. Key questions to ask here are:
- What is your modernization strategy?
- What is your cloud strategy?
- What is your API strategy?
- Are you modernizing your applications using Microservices architectural style?
- How are you handling co-existence?
- How are you doing DevOps?
- What are you doing in terms of business process transformation? How are you automating them?
- What is your integration strategy?

---

## IBM's Approach

The core of any digital transformation program is the digital integration layer as depicted in the diagram below

| **Digital Integration Layer** |
| :-: |
| ![Digital Integration Layer](../resources/digital-integration-conceptual.PNG) |

Following are the key capabilities that the digital integration layer should possess:

| **Digital Integration Layer Capabilities** |
| :-: |
| ![Digital integration layer capabilities](../resources/digital-integration-capabilities.PNG)

<br>

### Main Constituents of Digital Integration

There are 4 main constituents of digital integration:

1. Business processes/Customer journeys
2. Microservices fabric
3. API 
4. Analytics (real-time and batch)

<br>

#### Microservices Fabric

Following is a conceptual view of the Microservices platform:

| **Microservices Platform - Conceptual View** |
| :-: |
| ![Microservices platform - conceptual view](../resources/microservices-conceptual.PNG) |

Microservices need to provide multiple ways of invocation. Primarily:
1. REST endpoints - these endpoints are then exposed as API endpoints on the API Gateway (or used to create APIs)
2. EDA or Stream data processing endpoints - microservices can be chained together to develop stream data processing logic

Following picture depicts a typical Microservice development blueprint with REST :

| **Microservices Development Blueprint** |
| :-: |
| ![Microservice development blueprint](../resources/microservice-blueprint.png) |

Following picture depicts a typical way in which microservices are chained together to build stream data processing logic

| **Streaming Data Processing** |
| :-: |
| ![Streaming data processing](../resources/microservice-eda.png) |
 
<br>

### DevOps

Following picture depicts a typical CI/CD pipeline

| **DevOps - CI/CD** |
| :-: |
| ![DevOps - CI/CD](../resources/devops-cicd.png) |

---

## References
- [IBM Institute of Business Value white paper on Digital Transformation](https://www.ibm.com/downloads/cas/KWRV8QK6){:target="_blank"}
- [IBM's Smarter Business Microsite](https://www.ibm.com/in-en/smarter-business?p1=Search&p4=43700055523220409&p5=b&cm_mmc=Search_Google-_-1S_1S-_-AS_IN-_-ibm%20digital%20transformation_b&cm_mmca7=71700000068212243&cm_mmca8=kwd-296637289140&cm_mmca9=CjwKCAiAkan9BRAqEiwAP9X6Ub4zVyb4_WPv-DpOD2MUCHC4zbAuxZ-z4v3v0bWNmgUUqveMei0rzBoCYrsQAvD_BwE&cm_mmca10=446225946203&cm_mmca11=b&gclid=CjwKCAiAkan9BRAqEiwAP9X6Ub4zVyb4_WPv-DpOD2MUCHC4zbAuxZ-z4v3v0bWNmgUUqveMei0rzBoCYrsQAvD_BwE&gclsrc=aw.ds){:target="_blank"}
