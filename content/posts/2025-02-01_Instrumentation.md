+++
title = 'Application Instrumentation and Observability'
date = 2025-01-21T13:52:16+11:00
draft = false
tags = ['Security', 'CIO', 'Cloud', 'SaaS', 'DevOps']
revision = 1
+++

![Visibility and Transparency](https://toobstar.github.io/images/caveman_light.jpg)

## Application Instrumentation 

Refers to the process of exposing key information about a running application for a variety of purposes such as gaining insights into behaviour for understanding usage or audit requirements.  Key areas that are informed by this include:

- Performance Monitoring: Tracking response time, latency, throughput, and resource usage
- Error Detection & Debugging: Identifying bottlenecks and errors
- Observability & Logging: Recording events and application state changes
- User Experience: Tracking interactions and responsiveness
- Security Monitoring: Detecting suspicious patterns or anomalies
 
In the early days of server management the focus was on logs and server operating system metrics.  The logs were the window into the application and the server could provide CPU, process, memory, disk-space information which completed the picture.   Whilst the number of instances was small and stable this was acceptable, but as the transition to the cloud progressed (& the volumes of logs accelerated) the suitability of this distributed model became impractical.  Standardisation around log formats and application-performance-monitoring (APM) facilitated the progression towards centralised tools to aggregate information which created the pathway to the current tool based solutions.

The modern approach is to embed code, or an agent on the server (application container) which can access environment (APM) and application information and push that to a centralised service for further analysis. The challenge which modern tooling is focussed on is doing this:
- at scale (large volumes of activity)
- in highly dynamic (container enabled) environments
- with complex distributed (micro-service) architectures
- multi-cloud hosting platforms
- merging self hosted compute with managed platform services (PaaS)

## Observability 

Out of the fog of modern application instrumentation the key tenents of observability that have emerged are metrics, logs, and tracing.

### Metrics
Gather numerical data like CPU usage, memory consumption, request rates as well as provide flexibility for teams to create their own custom metrics on the fly without direct infrastructure access.  This provides an important interface for the organisation to understand application behaviour without compromising security and governance guidelines.  These metrics should be able to be plugged into enterprise communication channels (like Slack) for ease of reach. 

### Logging 
Where practical we can abandon the unrealistic goal of an application logging all events (good and bad) as the volumes involved make this impractical, but instead focus on logging to provide a record of auditable events and exception (e.g. error) information.  In many organisations this is not practical due to the lack of control that can be exerted on the application architecture due to vendor provided services, or legacy systems or other constraints that make conformity hard to apply and hence the lowest common denominator of logging is still required. 

### Tracing
Track flows of activity through distributed systems to enable an understanding of end-to-end request flow.  This is the modern solution for much of what application logging was originally used to fulfil. 

## Trends

The outlook for instrumentation is largely tied to continuing the journey to improving signal-to-noise and providing sensible standardised 'best practice' solutions out of the box.  This is largely being enabled by AI tooling allowing autonomous decision making at scale which is perfectly suited to this particular problem.  The self-learning of good behaviour and the automated detection of anomalous bad-behaviour is well suited to currently available AI capability and is becoming part of standard offerings.  

## Key Vendors 
There are many popular tools in the space of both the managed and open-source variety.  Where volumes of activity are modest then the commercial tools are extemely good value, and where activity is large, then ROI becomes hard to justify and self-hosted solutions may make more sense. Most companies will start out with modest activity and enjoy the benefits quickly of a hosted service, but as usage grows this equation can tip, and should be continually monitored. 


####  APM (Application Performance Monitoring) Tools
- [New Relic](https://newrelic.com/)
- [Datadog](https://www.datadoghq.com/)
- [AppDynamics / Splunk](https://www.splunk.com/en_us/products/splunk-appdynamics.html)
- [Dynatrace](https://www.dynatrace.com/)

####  Logging Frameworks
- [ELK Stack (Elasticsearch, Logstash, Kibana)](https://www.elastic.co/elastic-stack)
- [Fluentd](https://www.fluentd.org/) 

####  Distributed Tracing
- [OpenTelemetry](https://opentelemetry.io/)
- [Jaeger](https://www.jaegertracing.io/)
- [Zipkin](https://zipkin.io/)

## Outlook

It's also worth noting (and goes without saying) that commercial offerings typically have a better product offering and will be easier to enable (either through consulting services or better documentation and tooling) than open-source alternatives.  As competing vendors establish dominance they will try and create standards and these may become available to open-source tooling or merge into a defactor standard across all offerings. One example of this standardisation is [Open Telemetry](https://opentelemetry.io/).  Slowly through these standards and growing interest the open source alternatives become more capable and are viable alternatives.  In parallel with this there is a growing resistance to this high cost of SaaS that enables businesses and instrumentation has occasionally found itself at the top of the table for company vendor fees and can struggle to justify that position. 

