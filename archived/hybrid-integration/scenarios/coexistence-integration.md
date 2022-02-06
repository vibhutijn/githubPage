---
layout: default
title: Co-existence Integration
parent: Integration Scenarios
grand_parent: Hybrid Integration
permalink: /coexistence-integration
has_toc: false
has_children: false
nav_order: 4
---
{: .no_toc}
# Co-existence Integration

Organizations rely on core applications that maintain system-of-record (SOR) data on the legacy systems like mainframes and ERP systems. The transactional and batch applications running on these systems have organically evolved over time, reflecting the accumulated changes in a business and its requirements.   

Given the importance and history of these applications, apply a high degree of due diligence needs to be done for their modernization and evolution. Businesses are often risk-averse and avoid modifying their aging business-critical applications. So to mitigate these risks, business aligned modernization is done incrementally and iteratively. 

| Incremental Modernization |
| :-: |
| ![](../images/incremental-modernization.png)

Coexistence is a by-product of incremental modernization to deliver modernized functionality into production in controlled risk adverse manner. This is a transient layer, which bridge legacy and modernized states and responsible for owning the complexities and gaps for smoothly conversating these two states.  

| Co-existence Integration |
| :-: |
| ![enter image description here](../images/coexistance-integration-latest.png)

Please find below considerations for co-existence integration layer:

 - **Data**: As Data is fragmented and distributed across the legacy core and modernized core, there is high need of data consistency across these two components for example if there is any changes on modernized data, this needs to be replicated or synchronized or reconciled between two cores or vice versa.

 - **Data Mapping and Transformation**: As business functionalities started moving from legacy to modernized core, for conversation between legacy and modernized systems, coexistence integration services would need the data/interface mapping and transformation for moving data from one system to another as well as legacy system component changes can be minimized or avoided.
  
 - **End to End Transaction Management**: Business functionalities are distributed on legacy and modernized core. Co-existence layer needs to two cores to make the end to end transaction complete and successful. For example, transactions originated on modernized core needs to talk to legacy functions to get it completed or vice versa.
	 
 - **Non-Functional considerations**: Co-existence layer should address the non–functional aspects in alignment with modernized as well as legacy core. These non-functional aspects like performance, security, availability. For example:
	 - Data latency and performance while conversating legacy and modernize for various transactions
	 - Availability of this solution to avoid the impact on functional data flow between two systems

 - **End to End Security**: As Business functionalities started modernizing which evolves the need of end to end security aspects to be looked closely. For example:
	 - New integration touch points which required to be secured
	 - Consistent Identity provider solution across two cores 
	 - Varied Authentication and authorization solution across two states
	 - Data needs to be secured in flight or at rest 

 - **End to End Operation Management**: As end to end solution, spread across legacy and modernized cores, should provided end to end operational support through  integrated technical and business support solution with the help of co-existence layer. 

 - **Interception between current/legacy or modernized core**: In incremental modernization journey, business functionalities/sub-functionalities can be distributed and available on both legacy and modernized cores, incremental functionality switchover required, traffic/workload to be distributed between two system. 

 - **End to End Functional Flow Testing**: In progressive and iterative modernization journey, when incremental business functionalities are designed and modernized while other functionalities are already alive on the legacy. Functional flows or business processes are required to be end to end tested to ensure the expected outcomes in different modernization phases without any breakage. 
 
 - **Deployment Techniques**: Consider incremental modernization use cases deployment aspects, such as: 
	 - Does functionality switch of from legacy and switch on other side fully?
	 - Does functionality require to be incrementally available or specific workload routed on modernized state and keep incremented the load for same?

 - **Cost and budget**: As this is transient layer and will not be required once legacy core is fully transformed, so cost is one of major consideration while planning and design this layer in any modernization journey.


 





