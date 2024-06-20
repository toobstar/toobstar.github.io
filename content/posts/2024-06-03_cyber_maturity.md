+++
title = 'Cybersecurity Maturity'
date = 2024-06-03T13:01:19+10:00
draft = false
categories = []
tags = ['CISO', 'Risk']
revision = 1

+++

![Research](https://toobstar.github.io/images/caveman_reading2.jpg)

In a domain with significant uncertainty and complexity such as cybersecurity a common approach taken by organisations to determine what action should be taken is to ask where they stand compared to others? Essentially *are we ahead or behind expectations for an organisation like ours*? This approach of determining norms and *staying within the lane* is a reasonable heuristic when entering a domain without subject matter experts familiar with the organisation.

A common way to determine this positioning is to consider how **mature** the organisation is across the key drivers of cybersecurity risk.  Those being:

- **People**: The behaviour and knowledge of the team 
- **Processes**: The nature of the work that the team undertakes (e.g. how complex or repeatable it is)
- **Technology**: The tools and infrastructure in place that enables them to do this work

Where the risks govern the ability of the organisation to maintain the **confidentiality**, **integrity** and **availability** ([CIA](https://en.wikipedia.org/wiki/Information_security)) of their information assets. In my analysis of cybersecurity maturity I've defined 3 broad levels of progression:

- **Level 1: Basic.** This doesn't necessarily mean no progress, but could indicate a lack of central control, formality or repeatability to solutions in place to address risks.
- **Level 2: Initial.**  Consideration has been given by an authority within the organisation, and solutions may be in place that have been developed for the purpose if risk mitigation, but they may be specific to a team or function. They may also lack formality and oversight which results in variable outcomes.
- **Level 3: Best practice.**  This indicates that research has been done to determine the optimal solution for the organisation, it has been documented, and relevant processes are being followed for implementation and oversight. Also that the solutions in place are being reconsidered on a regular basis. 

### People

|           | Level 1: Basic                                                                         | Level 2: Initial                                                      | Level 3: Best practice                                                                                                       |
| --------- | -------------------------------------------------------------------------------------- | --------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Knowledge | No formal assessment of knowledge                                                      | Self directed training                                                | Mandatory scheduled training                                                                                                 |
|           | No formal consideration has been given to key assets / risks / threats to the business | Limited understanding of key assets / risks / threats to the business | Broad understanding of key assets / risks / threats to the business                                                          |
| Attitude  | Inconsistent knowledge / fear of cyber incidents                                       | Fear of incidents but avoidance of reporting due to repercussions     | Appropriate respect for risks and trust in the organisation that reporting of incidents will be handled in a no-blame manner |



### Processes

|                        | Level 1: Basic                                                                           | Level 2: Initial                                           | Level 3: Best practice                                                                                                                         |
| ---------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Change Management      | No paper trail for changes in configuration which impact access or risk                  | Changes are documented for who / why / what                | Audits are done on who has access to what and why                                                                                              |
| Access Control         | To ensure no barriers to work maximal access (e.g. admin level) provided by default      | Access is granted when requested                           | Least privilege access                                                                                                                         |
|                        |                                                                                          |                                                            | Role based access linked to on/off boarding                                                                                                    |
| Separation of duties   | Done informally if at all                                                                | Domain specific processes are documented where appropriate | Formalised processes with oversight                                                                                                            |
| Risk                   | No formal process adopted                                                                | Domain specific processes are documented where sensitive   | Formal processes in place                                                                                                                      |
|                        |                                                                                          |                                                            | Understanding of risk taking / oversight functions (e.g. 3LOD)                                                                                 |
|                        |                                                                                          |                                                            | Openness to consider risk in new domains (e.g. gen ai)                                                                                         |
| Continuous Improvement | After incidents there is no formal process to learn in order to avoid repeat occurrences | Domain specific review are undertaken in an ad hoc manner  | Formal processes for retrospective, improvement are in place (e.g. Plan-Do-Check-Act Principle PDCA or Corrective and Preventive Actions CAPA) |


### Tools

|                      | Level 1: Basic                                                            | Level 2: Initial                                                                                        | Level 3: Best practice                                                                      |
| -------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| Identity Mgt         | Fragmented silos with no central control or oversight                     | Centralised directory management                                                                        | Automated provisioning based on role for on/off boarding                                    |
| Authentication       | No central control or oversight                                           | Password Management                                                                                     | Passwordless                                                                                |
|                      |                                                                           | MFA (SMS/email)                                                                                         | MFA (hardware/TOTP)                                                                         |
|                      |                                                                           | SSO                                                                                                     | Smart / Context Aware access with risk based control                                        |
| Device Mgt           | No central control of device or access (MDM)<br>Traditional AV / Firewall | Centrally controlled MDM with asset register (HD encryption, remote wipe, OS / application updates etc) | XDR/EDR posture management (heuristic based detection and automated remediation capability) |
| Data                 | Informal data catalogue                                                   | Data is documented                                                                                      | Documentation generation is automated and is audited to match held data                     |
|                      | Data catalogue is not maintained                                          | Documentation provides guidance on sensitivity & controls                                               | Data loss prevention (DLP)                                                                  |
|                      |                                                                           |                                                                                                         | Data disposal is automated                                                                  |
| Network              | No controls                                                               | VPN                                                                                                     | Zero-trust (ZTNA)                                                                           |
|                      |                                                                           | Firewalls & I.P. whitelisting                                                                           | Secure Web Gateway (SWG)                                                                    |
| Cloud Services       | Shadow I.T. commonplace                                                   | Supplier Assessments                                                                                    | Cloud access service broker (CASB)                                                          |
|                      |                                                                           | Central User directory                                                                                  | Centralised user provisioning (SCIM)                                                        |
|                      |                                                                           |                                                                                                         | Privileged Access Mgt (PAM)                                                                 |
| Cloud Infrastructure | Ad hoc setup                                                              | Least privilege access                                                                                  | Cloud Security Posture Management (CSPM)                                                    |
|                      | Overly permissive access                                                  | Infr as code (IAC)                                                                                      | Cloud Workload Protection Platform (CWPP)                                                   |
|                      |                                                                           | Static Application Security Testing (SAST)                                                              | Cloud Infrastructure Entitlement Management (CIEM)                                          |
|                      |                                                                           | Access Audits                                                                                           | Cloud Service Network Security (CSNS)                                                       |
|                      |                                                                           |                                                                                                         | Cloud Native Application Protection Platform (CNAPP\*)                                      |
|                      |                                                                           |                                                                                                         | Expose engineering team to security guidance ('Shift left on risk')                         |
                                                                                                                       

Each of the elements in the table above can represent significant amounts of effort to be progressed through and I anticipate expanding on each through this site. A framework for managing information-security risk such as ISO 27001 essentially encompasses a toolkit to undertake that work.  Where that longer term commitment is anticipated I would recommend going down that pathway as the structure of the program is well considered and the benefit brought through external audit is clear to see.


