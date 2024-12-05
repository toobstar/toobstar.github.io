+++
title = 'SaaS Delivery Maturity'
date = 2024-11-27T13:43:36+10:00
draft = true
categories = []
tags = ['CIO', 'Cloud', 'SaaS', 'Service Delivery']
revision = 1
+++

![Research](https://toobstar.github.io/images/caveman_bicycle.jpg)

With modern tooling SaaS can be up and running very quickly and easily but but the journey to **maturity** can be a long and winding one. 

## What are the attributes of a mature service?  

That would include the service covering off the requirements of all functions of a modern business (finance, marketing, commercial product, engineering etc) whilst facilitating the growth and constant change a service is expected to accomodate, whilst being dependent on unreliable and changing 3rd party services to run, in as efficient and cost effective manner as possible. 

## Creating a roadmap whilst the journey is underway

Defining a specification (or the roadmap for that journey) is an important step for every organisation in progressing to an operational state which can provide certainty in a highly dynamic environment.  Each organisation will have a different view on what maturity looks like and will put different weights on different elements of that map.  Modern cloud providers have their views of what well-architected services look like (such as [AWS](https://aws.amazon.com/architecture/well-architected/) or [Azure](https://learn.microsoft.com/en-us/azure/well-architected/)) and although these are useful to be sure they only provide the cloud view of service maturity and not one which will generally cover off the needs of business operations. 

What follows is my proposed starting point for that roadmap to enable the pathway to maturity.  There are 8 areas of focus and a number of elements within each that could be scored to create a heapmap of progress for each service or overall for the organisation.  Invariably progressing to maturity will require an investment of time or the utilisation of services which both cost money, and the ROI of that will vary case by case. 

## Focus Area 1: Functional

| Item         | Description                                                                                      |
| ------------ | ------------------------------------------------------------------------------------------------ |
| Overview     | An understandable description of what the service does or related context useful for managing it |
| Arch Diagram | A technical representation of the logicial inner workings of the service                         |
| Interfaces   | Relevant interface points to other services whether internal, external or infrastructure         |