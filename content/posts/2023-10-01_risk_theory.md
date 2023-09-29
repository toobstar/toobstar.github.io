+++
title = 'Risk Management Fundamentals'
date = 2023-09-26T09:42:54+10:00
draft = true
categories = []
tags = ['risk', 'governance']
+++

### Context and why we do it

Templates for managing risk are quite easy to find and tend to be fairly similar to each other.  Practical guidance for how to put a risk methodology into practice are less easy to find.  One challenge is getting buy-in to a process which seemingly replicates existing processes for deciding what to work on.

Firstly a formal definition of risk for this context: 
> Risk is the effect of uncertainty on the achievement of objectives

This ties risks that we care are about directly to strategy, and pushes us to consider uncertain outcomes that would impact our ability to achieve our strategic goals.  Or to put it inversely: if there is an action or event with an uncertain outcome which *would not* impact our plans then we don't need to track it in a formal way. 

Secondly in general terms all professionls already consider risk in a deliberate way.  Whether it's software engineering with:
- methods of predicting time to complete a task
- QA processes to find bugs

Or Product Managers undertaking: 
- customer interviews to validate need
- A/B testing features to understand how they are used  

Each of these processes (and many more) are fundamentally built around addressing an *uncertain outcome that would impact our objectives*.  

### The output of this exercise

The fundamental point of a formal risk management process is to align cross-functionally the various specialised methods of considering risk such that a clear understanding can be had on risks across a business.  The ability for executive and functional leads to consider risks across the business using a standardised model allows them to be compared and to understand  dependencies more clearly across the business.

Further it provides the business with a tool to understand the impediments to achieving it's strategic goals, and to validate whether the efforts of the team are appropriated resources and structured achieve the risk mitigation goals. 

To clarify: a formal risk management process is not intended to replace existing methods of managing uncertainty that exist across the business.  An outcome which is duplicating existing work tracking systems should be viewed with caution as the likelihood this can be maintained effectively is poor. 

## Risk Governance Model

In order to provide confidence that a risk process is effective it is helpful to adopt a risk governance structure which provides clarity on different roles and responsibilities. A commonly adopted model is known as 3 lines of defence (3LOD) and was published by the Institute of Internal Auditors (IIA) in 2013. 

- The first line of defence (**Line 1**) are the risk owners (or risk takers) and are responsible for identifying risks, implementing treatments and reporting on outcomes from those.
- The second line of defence (**Line 2**) provide a compliance function where they support the first line to operate according to risk management practices as defined by the company.
- The third line of defence (**Line 3**) fulfil an audit function as an independent body providing validation that collectively lines 1 & 2 are fulfilling the risk management mandate of the  

This model of *activity* orchestrated by *compliance* and checked by *audit* is broadly applicable and effective across many business domains and will be familiar to many.

## Risk Register

A risk register is an inventory of risks and a formally defined and well understood method to evaluate them.  It is also a place where risk treatments will be considered and tracked.

The key features of a risk are the likelihood that it will occur, and the impact if that were to happen.  

### Risk Likelihood

Typically determining the likelihood of a risk is quite hard to do in a satisfying way.  It is a subjective assessment and undertaking it requires making a prediction about one or more future events. Often those occurrences will be rare and / or not previously experienced so hard to predict.  In order to account for this no attempt of precision is attempted and qualitative and reductive values like certain, likely, and rare are used to convey this.

### Risk Impact

The impact of a risk is easier to assess than the likelihood because we can often (but not always) translate into a quantitative measure which makes it less subjective.  The ideal measure of course being dollars (be that revenue or cost) which allows for clear benchmarking.

### Risk Classification

A risk matrix will be established where each of the possible ratings for likelihood and impact are used as axis in a matrix and given a weighting (e.g 1 - 5) and the output or classification of the risk the multiplication of these weightings.  

![Risk Matrix](/images/risk-matrix.png)

### Risk Appetite

Given the option to express a risk tolerance level I expect most executive teams would describe themselves as mid-range.  Obviously not reckless in accepting unnecessary risk but also not overly conservative as agents for growth.  There is the ability to validate and self-adjust the risk appetite through the validation of the risk classifications against willingness of the business to accept these.  If a risk is considered high, and could be treated to reduce that, but the business decides not to proceed with that, then most likely the scale for determining the likelihood and impact should be adjusted, or the matrix that determines a risk is high for the given likelihood and impact should be adjusted. 

### Risk Treatment

A Risk Treatment is the process to modify a risk and involves:
- Avoiding the risk by deciding not to start or continue with an activity that gives rise to the risk
- Removing the risk source
- Changing the likelihood
- Changing the impact
- Sharing the risk with another party
- Accepting the risk after informed consideration

Following the application of treatments the **residual risk** is the updated status of the risk  item after the fact.  

And finally, when is a risk no longer a risk?  When the uncertain event has played out and the risk is no longer relevant, or the risk has been realised into **an issue**. A risk register should stand separate from issues or other known challenges the business is facing. 

