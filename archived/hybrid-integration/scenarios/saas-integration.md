---
layout: default
title: SaaS Integration
parent: Integration Scenarios
grand_parent: Hybrid Integration
permalink: /saas-integration
has_toc: false
has_children: false
nav_order: 3
---
{: .no_toc}
# Integration with SaaS

An organization's shift to public/private cloud is a significant and disruptive event that showcase, customers has started moving their workload from on-premise to cloud as System of Records (SOR) / Software as a Service (SaaS) / Modernized applications for optimization and flexibility.   

So, what is SaaS, and what good does it do?

It’s a method of software delivery where applications are hosted remotely by a vendor or service provider and are made available to customers over a network. Simply put, users rent the software instead of purchasing it. Most SaaS providers offer a usage-based subscription that can be purchased on a monthly or yearly basis, such as Salesforces (CRM ), SAP S/4 HANA, ServiceNow, Workday, etc .

As a cloud adoption use case, when there is a decision to decommission an older legacy application, replacing it major SaaS application, a ripple effect occurs impacting all applications that interacts with the legacy application.   

| Saas Integration |
| :-: |
| ![](../images/saas-integration.png) |

Please find below considerations for integration with SaaS applications:

 1. Integration Bus will not be sufficient or capable of mediating cloud originating integrations services request without use of gateway capability. 
 2. Integration architecture/solution need to be refactored or extended further .For example, web services interacting with legacy application earlier, may need to be extended to include the REST APIs to support the formats required by SaaS applications.
 3. Such integration solution might require SaaS application cloud connectors to support the different integration styles and business data formats.
 4. Such solution provide the low/no-code integration tooling for business/shadow integrator.
 5. Such Integration scenario need to address the on-premise and cloud based security (IAM) requirements.
 6. Such solution can address the data migrations between SaaS and on-premise applications.
 7. Using ETL or FTP to Synchronize application data is not secure enough between a datacenter and cloud application. Such requirements leads to cloud-optimized data integration software.
 8. For reliable integrations between Data center and SaaS application, arise the need of reliable messaging and improved error handling. 
 9. Shift from high speed LAN to fast broadband connectivity between on-premise and Cloud or multi-Cloud to provide low latency integrations.  

Enterprise need to add new integrations capabilities like Integration Platform as a Service (iPaaS) / Integration Software as a Service (iSaaS) to address cloud to ground application integration with the help of prebuilt SaaS connectors and highly performance data synchronization / replication capabilities as cloud ready application integration stack. 

