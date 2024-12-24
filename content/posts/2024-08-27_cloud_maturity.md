+++
title = 'SaaS Delivery Maturity'
date = 2024-11-27T13:43:36+10:00
draft = false
categories = []
tags = ['CIO', 'Cloud', 'SaaS', 'Service Delivery']
revision = 1
+++

![Research](https://toobstar.github.io/images/caveman_bicycle.jpg)

With modern tooling SaaS can be up and running very quickly and easily but the journey to **maturity** can be a long and winding one. My goal with this overview is to run through the operational differences between a mature and immature service and the key areas to be considered to progress through that divide. 

## Defining the S in SaaS

To start with a simple definition though, an organisation may have a readily identifiable service which is their principle offering.  Beneath the hood there may be many independent applications which operate together to enable the offering.  A modern architecture known as [micro-services](https://en.wikipedia.org/wiki/Microservices) is commonly used which results in a proliferation of services and from a maturity point of view they could be at varying points along the maturity spectrum.  Whether it makes sense to consider each micro-service independently or to consider them collectively will be context specific.  Needless to say if a collective approach is taken the system is only as strong as the weakest link so scoring progress should recognise that. 

## What are the attributes of a mature service?  

That would include the service covering off the requirements of all functions of a modern business (finance, marketing, commercial, product, engineering etc) whilst facilitating the growth and constant change a service is expected to accomodate, being dependent on unreliable and changing 3rd party services to run, in as efficient and cost effective manner as possible.  For a technical operational service owner the focus will most naturally be on deploying new releases ('the build pipeline'), performance, cost and (if we're lucky) security.  These are all critical concerns and ones the technical service manager is the principle stakeholder for, but at a holistic organisational level, there are other questions and demands the business will have of a service which it's important to also cover off. 

## Creating a roadmap whilst the journey is underway

Defining a specification for service maturity for a live system might feel like working out a roadmap for a trip whilst already underway but it's a natural approach as it can be optimally done only with an understanding of actual operational demands. It is an important step for every organisation in progressing to an operational state which can provide certainty in a highly dynamic environment.  Each organisation will have a different view on what maturity looks like and will put different weights on different elements of that map.  And of course, these operational requirements will change over time so they should be maintained on a regular basis. 

Modern cloud providers have their guidance for what well-architected services look like (such as [AWS](https://aws.amazon.com/architecture/well-architected/) or [Azure](https://learn.microsoft.com/en-us/azure/well-architected/)) and although these are useful for sure they only provide the cloud view of service maturity and not one which will generally cover off the needs of business operations. 

![roadmap](https://toobstar.github.io/images/caveman_map_car.jpeg)

## Is there a correct level of maturity?

Actually no, the progress to maturity should simply match what's appropriate for that service in that context.  Getting to maturity consumes time and money, and like any investment doing so too early can result in wasted resources. It's easy to anticipate that as a product matures from prototype to launch and then scale, we expect the delivery maturity to also progress in a similar cadence. 

## The 8 Focus Areas

What follows is my proposed starting point for that roadmap to enable the pathway to maturity.  There are 8 areas of focus and a number of elements within each that could be scored to create a heat map of progress for each service or overall for the organisation.  

1. Functional
1. Monitoring and Alerting
1. System Reliability (SRE)
1. Logging
1. Build Pipeline
1. Cost Management
1. Business Continuity (Backup and Restore)
1. Security / Compliance

Invariably progressing to maturity will require an investment of time or the utilisation of services which both cost money, and the ROI of that will vary case by case.  So my preference is to track two metrics for each item: 

- What is the current status of this item?
- What is required to progress this item forward? 


## Focus Area 1: Functional

#### Why? 
To inform people working on or with this service what its goals are in order to provide context for its operational requirements.   It is these operational requirements that allow many of the following focus areas to be scored as to whether they meet the required standard. 

| Item         | Description                                                                                      |
| ------------ | ------------------------------------------------------------------------------------------------ |
| Overview     | A description of what the service does and related context useful for understanding it |
| Architecture Diagram | A technical representation of the inner workings of the service                         |
| Interfaces   | Relevant interface points to other services whether internal, external (SaaS) or infrastructure (PaaS)         |


## Focus Area 2: Monitoring and Alerting

#### Why?
In order to have confidence the service is fulfilling its commitments there must be oversight and then action taken when that is not achieved.

| Item         | Description                                                                                      |
| ------------ | ------------------------------------------------------------------------------------------------ |
| Key pathways    | An overview of functional behaviour that is observable in the service                        |
| Passive monitor | A capability external to the service which can monitor healthy operations within the service              |
| Active monitor  | A capability external to the service that can trigger an operation that proves the service is functioning |
| KPIs / SLAs     | Operational metrics and expectations of the service                                                       |


## Focus Area 3: System Reliability Engineering (SRE)

#### Why?
This focus area probably requires the least explanation except to clarify that I have chosen to take a narrower interpretation than what [some definitions](https://en.wikipedia.org/wiki/Site_reliability_engineering) would describe.  Populated by Google, like DevOps, SRE can be a job title, an org unit, a program or initiative, or just a collection of practices or goals related to reliable service delivery.  In this narrower interpretation the specification is simply defined as follows:


| Item         | Description                                                                                      |
| ------------ | ------------------------------------------------------------------------------------------------ 
| Goals Set & Monitored | Defining and measuring reliability goals: Service Level Indicators, Objectives and agreements ([SLIs](https://en.wikipedia.org/wiki/Service_level_indicator), [SLOs](https://en.wikipedia.org/wiki/Service-level_objective), [SLAs](https://en.wikipedia.org/wiki/Service-level_agreement) and [error budgets](https://cloud.google.com/blog/products/management-tools/sre-error-budgets-and-maintenance-windows) ) |
| Availability Specification | A practical translation of the SRE goals into an actionable configuration. e.g. [failover setups such as active-active vs warm-standby vs restore-from-backup](https://docs.aws.amazon.com/whitepapers/latest/disaster-recovery-workloads-on-aws/disaster-recovery-options-in-the-cloud.html)                                                                                                                                                                |
| Load Projection       | A model of peak & regular traffic has been created as well as forward projections for changes in load profiles                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| Load Tested           | The service has been performance [load tested](https://en.wikipedia.org/wiki/Load_testing) against load projections for both [soak](https://en.wikipedia.org/wiki/Soak_testing) and peak phases                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |


## Focus Area 4: Logging

#### Why?
Application and system logs have been a [standard part of computing](https://en.wikipedia.org/wiki/Logging_(computing)) since its origin. They are a record of activity and are used for audit/compliance, investigating bugs or user behaviour, and as part of understanding current system behaviour to enable SRE.  Most commonly due to the operational characteristics of modern logging (e.g. high volumes and combining streams of data from multiple sources) and to enable improved creation of metrics and alerts logs are consumed through an instrumentation tool.  The challenge will invariably be capturing information needed to resolve a future problem without storing unnecessary content that costs money and reduces the ability of the tooling we build around those logs to work effectively. 


| Item         | Description                                                                                      |
| ------------ | ------------------------------------------------------------------------------------------------ 
| Categorisation  | Logs with different operational characteristics (retention, sensitivity, audience etc) are identified and streamed such that they can be managed appropriately |
| Retention       | Are retained per operational requirements                                                                                                                     |
| Access          | Access and ability to modify or remove is controlled                                                                                                          |
| Instrumentation | Service behaviour is exposed through smart tools to the right audience in a timely way and allows for metrics and alerts to be built dynamically              |
| Compliance      | Data governance, privacy and retention requirements are met according to applicable compliance standards                                                      |


## Focus Area 5: Build Pipeline

#### Why?
The ability to release code with minimal effort, risk and as quickly as possible is an important feature for SaaS businesses to enable growth.  By reducing the overhead of doing a release you can reduce the delta of change which justifies a release, and therefore reduce the risk of every release. And then by releasing more quickly you can deliver value sooner, get feedback more quickly and more generally facilitate agility across the business.  The processes that formalise best practice are known as continuous integration and delivery ([CI/CD](https://www.atlassian.com/continuous-delivery/principles/continuous-integration-vs-delivery-vs-deployment)). They are enabled by trust in the delta which is traditionally driven by QA-automation practices and to a lesser extent the ability to control change independent of code through [feature flag](https://en.wikipedia.org/wiki/Feature_toggle) tooling. 

![Research](https://toobstar.github.io/images/ci_cd.jpg)


| Item         | Description                                                                                      |
| ------------ | ------------------------------------------------------------------------------------------------ 
| Source Repository  | Central control of code with ability to plug-in developer productivity tooling or operational (security) analysis                                                |
| IaaC (build)       | Infrastructure as code is a key capability to facilitate scale and compliance controls through a proper lifecycle management process over traditional click-ops. |
| Release Automation | Low friction and controlled change management to allow for continuous integration and continuous delivery                                                        |


## Focus Area 6: Cost Management

#### Why?
It should go without saying that cost management is a critical element of SaaS delivery.  The ability in a modern cloud native business to adjust infrastructure settings at will provides tremendous flexibility and power to solve problems.  It also provides the ability to drive cost quickly and in unexpected ways so care must be taken to ensure the operational setup is in alignment with the business strategy that is being pursued. This can come down to a risk assessment where no (or low) risk costs significantly more than a higher risk setting and finding the right level should be done with transparency between all stakeholders in order to enable the business strategy and achieve the SRE settings that have been agreed to.  

| Item         | Description                                                                                      |
| ------------ | ------------------------------------------------------------------------------------------------ 
| Attribution         | I.T. & infrastructure services are attributed to a cost centre                                                                                                           |
| Owner               | Cost centres have owners or related stakeholders who are informed of cost positions                                                                                      |
| Modelling           | An understanding exists of fixed & variable cost drivers as related to the cost of service delivery and product development both overall and per sale (incremental cost) |
| Reporting           | Regular cost reports are presented to stakeholders in a way that aligns to the cost model and facilitates informed commercial and product-engineering decisions          |
| Budgets & Forecasts | Cost Forecasts are made for the cost centres and actual costs are tracked against budgets over time                                                                      |
| Anomaly Detection   | Spikes in cost are detected in a timely way so action can be taken to prevent unintended blowouts                                                                        |


## Focus Area 7: Business Continuity 

#### Why?
Related to SRE is the more specialised area of understanding what infrastructure and services enable SaaS delivery, developing scenarios under which they could fail, and then building out and testing plans to allow for continuity of service delivery through these scenarios. 

| Item         | Description                                                                                      |
| ------------ | ------------------------------------------------------------------------------------------------ 
| State Catalogue       | Any non-transitory state for each service that is a required input (e.g. a database) is clearly documented                                                           |
| DR Objectives defined | Recovery time objective (RTO): Acceptable duration of service downtime<br>Recovery point objective (RPO): Acceptable loss of data.                                   |
| DRP in place          | A disaster recovery plan with appropriate scenarios has been created that describes how state would be re-instantiated and the service recovered under each scenario |
| DRP tested            | The disaster recovery plan has been used or tested and there is confidence it would work as intended                                                                 |
| Backups               | Backups exist in a suitable location such that recovery is possible in the event of the disaster scenarios occurring                                                  |
| Restoration           | Backup restores have been tested to confirm they would work as intended                                                                                              |



## Focus Area 8: Security & Compliance

#### Why?
SaaS typically depends on the key-tenets of information security (Confidentiality , Integrity  and Availability) to operate well so there is a natural synergy between the two.  Building trust with customers or suppliers in order to achieve commercial goals requires ensuring security is taken seriously and is provable. For that reason companies typically adopt a certifiable and well regarded framework to achieve their security goals.  

The mantra of a modern security focussed organisation is to “shift left” on security by building awareness with the team, and taking steps to consider security from the outset of product development.  There are now many modern tools and processes which can assist to automate this which modern organisations should definitely be adopting. 

The culmination of a suite of cloud security tools when delivered as a platform (which can be quite efficient and effective from an integration point of view) is known as a Cloud Native Application Protection Platform	 (CNAPP).  


| Item         | Description                                                                                      |
| ------------ | ------------------------------------------------------------------------------------------------ 
| Secure Engineering                                 | Training and guidance on secure coding practices and issues such as OWASP                                                                                                                        |
| Static Application Security Testing (SAST)         | Analyse source code and related configuration (including infrastructure as code) to identify security vulnerabilities typically through reference to Common Vulnerabilities and Exposures (CVEs) |
| Dynamic Application Security Testing (DAST)        | Penetration testing and active validation against live services                                                                                                                                  |
| Cloud Security Posture Management (CSPM)           | Detect and prevent misconfigurations in the cloud environment that could lead to sensitive data breaches and security compliance violations. e.g. across areas such as networking & encryption   |
| Cloud Infrastructure Entitlement Management (CIEM) | Targeted Privilege and identity configuration oversight                                                                                                                                          |
| Cloud Service Network Security (CSNS)              | Services such as web-application-firewalls (WAFs) or Zero Trust Network Access (ZTNA)                                                                                                        |
| Cloud Workload Protection Platform (CWPP)                                                                                | Continuous monitoring of cloud workloads via agents or direct access. A control over running processes in our cloud infrastructure.               
| Data Loss Prevention (DLP)                                                                                               | Monitor for unsafe or inappropriate sharing, transfer, or use of sensitive data information transfer across cloud services                                                     |
| Privileged Access Management (PAM)                                                                                       | Monitoring, detecting, and preventing unauthorised privileged access to critical resources                                                    |
| Security information and event management ([SIEM](https://en.wikipedia.org/wiki/Security_information_and_event_management)) | A logging channel that collects audit or events related to security in a single pane to facilitate the detection of threats across all business operations |
