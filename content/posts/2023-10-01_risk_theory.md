+++
title = 'Risk Management Fundamentals'
date = 2023-09-26T09:42:54+10:00
draft = false
categories = []
tags = ['risk', 'governance']
ID = '7890'
+++

![Risky Work](/images/caveman_shark2.jpg)

### Context 

Guidance for managing risk is easy to find and tends to be fairly consistent in approach.  It's largely structured around templates which are straightforward and seemingly adaptable.  But practical advice for how to put a formal risk process into practice is less obvious but extremely important.  

It is likely that a step-by-step guide for implementation is not useful because the optimal implementation will vary significantly from company to company. Variables that matter a lot include:
- how experienced the leaders in the business are with formal risk practice
- the engagement from the board or other external audit bodies
- the regulatory environment 
- the level of cross-functional dependencies (i.e. do risks I own only impact me or do they also impact others?) 
- the size of the business and the load of work for risk compliance (e.g. are there dedicated risk roles)
- the risk tolerance of the business
- the fluidity of the risks and their related treatments

Each of these variables will influence how ambitious the expectations should be for the initiative.  At one end of the scale with risk being considered formally prior to decisions being made, and at the other end, an assessment only after action has been taken as a post-hoc analysis.

It is useful to start with a formal definition of risk in this context: 
> Risk is the effect of uncertainty on the achievement of objectives

This ties risks that we care are about directly to strategy, and pushes us to consider **uncertain outcomes that would impact our ability to achieve our strategic goals**.  Or to put it inversely: if there is an action or event with an uncertain outcome which *would not* impact our plans then we don't need to track it in a formal way. 


### Operational Challenges

An initial hurdle is getting buy-in to an activity which appears to replicate existing processes for deciding what to work on.  Many professions already consider risk in a deliberate way.  Whether it's software engineering with methods of predicting time to complete a task, or how we conduct QA to find bugs.  Or Product Managers undertaking customer interviews to validate need and A/B testing features to understand how they are used.  Each of these processes (and many more) are fundamentally built around addressing *uncertain outcomes that would impact our objectives*.  

What we are trying to do at an enterprise risk level is more top-down than bottom-up.  If there is a sense that we are recreating existing processes to manage uncertainty then we've probably gone in to too much detail.  Where there is motivation for it, it is possible to have functionally specific risk registers and have these roll-up to an enterprise level one.  This also allows teams to utilise existing processes for managing uncertainty where they are well developed or to use a formal risk based approach otherwise.  


### Outcomes

A fundamental goal of a formal risk management process is to align cross-functionally the various specialised methods of considering risk such that a clear understanding can be had across the business.  The ability for executive and functional leads to consider risks using a standardised model allows them to be compared and to understand dependencies more clearly.

Further it provides the business with a tool to understand the impediments to achieving it's strategic goals, and to validate whether the efforts of the team are appropriately resourced and structured to achieve the risk mitigation goals.

It may come to light that areas of uncertainty are not getting sufficient focus, or how risks owned by one team become impediments to another teams goals.  The conversations that follow this analysis put structure behind the cut and thrust of executive engagement we should expect our leadership team to be engaged in.    

## Governance Model

In order to provide confidence that a risk process is effective it is helpful to adopt a risk governance structure which provides clarity on different roles and responsibilities. A commonly adopted model is known as 3 lines of defence (3LOD) and was published by the Institute of Internal Auditors (IIA) in 2013. 

- The first line of defence (**Line 1**) are the risk owners (or risk takers) and are responsible for identifying risks, implementing treatments and reporting on outcomes from those.
- The second line of defence (**Line 2**) provide a compliance function where they support the first line to operate according to risk management practices as defined by the company.  Line 2 should be considered the managers of the risk process design, roll-out as well as ongoing compliance of that process across the business.
- The third line of defence (**Line 3**) fulfil an audit function as an independent body providing validation that collectively lines 1 & 2 are fulfilling the risk management mandate that was agreed to.  As an example the board may agree to a business strategy and the associated approach to handling risk that is expected in pursuing that, and then audit that this is in fact being followed as a part of it's operations.

This model of *activity*, check and orchestrated by *compliance* and reviewed by *audit* is broadly applicable and effective across many business domains and will be familiar to many.

## Risk Register

And finally yes; [there are templates to be followed](https://docs.google.com/spreadsheets/d/1nBQOJBIL9k6xIsp4i7g7pbYaSnYDMMVoivaQLEErPs0/edit).  Most principally a risk register document.  It is an inventory of risks and a formally defined and well understood method to evaluate them.  It is also a location where risk treatments will be considered, tracked and the residual risk predicted.

The key features of a risk are the likelihood that it will occur, and the impact if that were to happen.  These translate into an overall classification typically being low, medium and high.  

### Risk Likelihood

Typically determining the likelihood of a risk is quite hard to do in a satisfying way.  It is a subjective assessment and undertaking it requires making a prediction about one or more future events. Often those occurrences will be rare and / or not previously experienced so hard to predict.  In order to account for this no attempt of precision is attempted and qualitative and reductive values like certain, likely, and rare are used to convey this.

### Risk Impact

The impact of a risk is easier to assess than the likelihood because we can often (but not always) translate into a quantitative measure which makes it less subjective.  The ideal measure of course being dollars (be that revenue or cost) which allows for clear benchmarking.

### Risk Classification

A risk matrix will be established where each of the possible ratings for likelihood and impact are used as axis in a matrix and given a weighting (e.g 1 - 5) and the output or classification of the risk the multiplication of these weightings.  

![Risk Matrix](/images/risk-matrix.png)

### Risk Appetite

Given the option to express a risk tolerance level I expect most executive teams would describe themselves as mid-range.  Obviously not reckless in accepting unnecessary risk but also not overly conservative as agents for growth.  There is the ability to validate and self-adjust the risk appetite through the validation of the risk classifications against willingness of the business to accept these.  If a risk is considered high, and could be treated to reduce that, but the business decides not to proceed with that, then most likely the scale for determining the likelihood and impact should be adjusted, or the matrix that determines a risk is high for the given likelihood and impact should be adjusted. 

### Treatments and mitigations

A Risk Treatment is the process to modify a risk and involves:
- Avoiding the risk by deciding not to start or continue with an activity that gives rise to the risk
- Removing the risk source
- Reducing the likelihood
- Reducing the impact
- Sharing the risk with another party
- Accepting the risk after informed consideration

It should be known what outcome we are hoping to impact by pursuing a risk treatment prior to starting that activity.  It's possible to pursue multiple treatments in parallel which independently address likelihood and impact, but it is helpful to know this up front to be able to track performance against those goals. 

Following the application of treatments the **residual risk** is the updated status of the risk item after completion.  

### Removal

And finally, when is a risk no longer a risk?  When the uncertain event has played out and the risk is no longer relevant, or the risk has been realised **into an issue**. A risk register should stand separate from issues or other known challenges the business is facing but there will be the temptation to leave these (realised) risks in as historical artefacts. 

### Finally: A question of time

Does a risk register have a start or finish date?  Or is it continuously updated?  This should be considered and influences how the register can be queried.  For example do we care to know:

- What was the status of a risk 6 months ago?  And importantly, how have we progressed since then in our treatment of the risk?  This requires maintaining an initial or point in time risk status but does allow tracking the impact of our risk treatments clearly.
- What is the risk status today?  This assumes continually (or on a defined cadence) updating the risks to reflect the current position.  

Each question requires work in order to be answered and the ROI may not be there for all cases.  One final thing to be considered deliberately.  


