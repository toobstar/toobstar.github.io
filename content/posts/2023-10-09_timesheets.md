+++
title = 'Timesheets'
date = 2023-10-09T12:20:44+11:00
draft = true
tags = ['timesheets', 'cost tracking', 'budgets']
revision = 1
+++

Why would any business use timesheets which are notoriously unpopular and hard to do well?  The main reasons include:
- understanding business dynamics
- to bill for time spent on an agreed task
- to understand velocity to complete a task so future work can be better planned out 
- tracking sustainable work practices and utilisation

In all cases it's important to be deliberate about whether we are tracking (1) the cost to the business (e.g. the overall cost of an employee) versus (2) some external representation of the value delivered by that person's work (e.g. an hourly rate for an employee multiplied by hours spent).  Language used to navigate this includes the effective rate, or billable hours, or utilisation of an individual but these terms all basically comes down to the same concern of navigating an internal versus external cost view. 

If the decision is made to track the cost to the business (and assuming no overtime is paid which is typical in my experience) it's simpler to consider that as a percentage of a whole day.  E.g. 25% or 50% of a day. Where the external representation is preferred then hours or minutes can be used, but this requires more work for those entering their time, which can reduce data-quality if not done properly.

Note: it's almost impossible to track both types of time spent at the same time.  A more reasonable solution is some translation as required between the two approaches. 

## Understanding Business Dynamics

![Getting Clarity](https://toobstar.github.io/images/caveman_challenge.jpg)

A business has many constraints around how it develops, sells and delivers services.  These constraints might include access to input materials, or marketing budgets, or many other things, but **for most businesses the primary cost and enabler of success are the people who are engaged to work for it**.    

In order to understand the dynamics of a business you can start with (and go quite far) simply knowing the roles of the team and the organisational structure that they sit within.  For most growing or dynamic businesses each individual will typically be working towards multiple goals and this level of precision is not sufficient to understand it adequately. 

A basic mental model for costs in a business is that some costs are fairly stable and some costs are dynamic and depend on a variable that may or may not be directly connected to revenue.  As an example for a company that processes data, large amounts of data are more expensive to process than small amounts of data all else being equal.  Or for a business where a person is required to close a sale, the cost of sales overall is variable and tied to the cost of people to fulfil this. 

The reason this distinction is important is that in order to understand the growth potential of a business these dynamics between costs and revenue are required to be understood.  It should also be obvious that outputs which depend on inputs can only scale so far as those inputs are available.  Which for the cases where the inputs are people, then those limits are more apparent (*and important*) than in other businesses. 

A standard breakdown of employee time is to split time spent between:
- general and administrative work (G&A)
- sales related activities
- cost of goods and service delivery (COGS)

It is generally expected that G&A is a relatively fixed cost, whereas sales and COGS are relatively variable.  Businesses that are dependent on people for sales and service delivery (such as consulting companies) are constrained in how much growth they can achieve, whereas business that can automate sales and service delivery have much higher growth potential.  

A general benchmark for gross profit margin for professional services businesses is around 30%.  Internet enabled *product* companies are expected to have a higher growth margin based on the level of automation and scale that can be realised.  

## Billable Time 

Some professions bill by time and an optimal time-sheeting solution for them is quite different than that of *regular* companies. From an operational point of view it is a much simpler implementation to assume that every minute of the day is accounted for and not have to complicate things further than that. 

For other companies a decision has to be made about all the various activities that are done in a day outside of *the real work* such as lunch, meetings, training or sick leave to mention just a few. Are these kept separate from regular tasks (e.g. as "admin") or built into the cost of doing business.  Unless there is a reason to be tracking *admin* tasks (which is a reasonable thing to want to do such as how much training was run across the organisation) it is simpler to just fold admin tasks into whatever the dominant tasks was for the period.  The alternative is to track it separately (which is more work) and it just get's folded into the cost of an employee anyway at the end of the day.  So unless you need to know leave taken, or how much time was spent in meetings, my recommendation is to just treat admin tasks as part of the dominant activity where possible.  It's less work up-front (meaning data quality *should* be higher) and when reporting later (with fewer adjustments to get to true cost). 

## Planning Work

Tracking time taken to complete past work is often used to forecast time to be taken for future work.  In some businesses or professions this is quite accurate whereas others are notoriously inaccurate.  For those such as software development which tend to be at the less accurate end of the scale most teams don't try and get an accurate answer.  They use agile methodologies, and story points with fibonacci scales or t-shirt sizing that deliberately limits the ability to predict the work taken to complete larger tasks. For this sort of work time-sheets are not a practical tool for predicting time to complete a future task.  Perhaps in the aggregate they are more effective but care should be taken even then.

For work which is more repeatable, with fewer unknowns, past experience can be a more useful guide for forecasting.  And particularly in the case with external stakeholders (such as customers expecting a deliverable) on a schedule the ability to forecast accurately is hugely important for a business.  This is essentially an exercise in filling the work pipeline most optimally.

## Working Sustainably

It's possible that timesheets can be used to monitor overtime or utilisation, but due to the subjective nature of task categorisation, or perceptions around commitment this can be tricky to achieve success with.  It most likely requires a minutes/hours based tracking method rather than a % of day based one (although I suppose you could indicate you worked 125% of a day).  Where possible it makes more sense to me to track this through conversations between team and manager to cut through the subjective nature of this. 

## Practical Concerns and General Tips

#### High Quality Data

Maintaining high quality data is crucial for timesheets to be of value.  The [proverbial bad apple](https://www.npr.org/2011/05/09/136017612/bad-apple-proverbs-theres-one-in-every-bunch) real does spoil the apple cart and once trust is lost it's hard to restore. There needs to be continuous focus on validating the data through visible reporting or spot checks to maintain this compliance and quality.  This feedback loop of reporting drives improved quality with the people entering time have a shared and improved understanding of how that information is used. 

#### Work with people rather than against them

Where possible if people always work on the same activity type or it's possible to infer what they are working on without their input, use that approach to try and avoid introducing errors in the data and annoying your team.  Asking people to enter time without constant oversight is doomed to failure so it should only be done where it's required and the oversight is possible. 

If you are asking people to track their time you need to report it back to them, their team, their manager and the owner of the outcome they are working towards.  This visibility is crucial to ensure a positive feedback loop that maintains high quality data. 

There needs to also be the possibility to correct previously inputted data following this visibility to ensure engagement and ongoing support. 

#### Understand regional differences

For multinational companies there needs to be an awareness of different working week durations, or regulatory concerns regarding timesheet tracking such as [working hour controls in Japan](https://www.lexology.com/library/detail.aspx?g=eff1d14b-8b13-409b-9f78-85e269d942e5). 

#### Challenges of work categorisation

It's often not known how to categorise a task or a task may evolve over time from one category to another.  I've had the experience of an activity that started as account management, subsequently became support, then evolved into product development, (which required a release to resolve), and ultimately was viewed by some as part of a sales strategy to drive renewal.  A solution to that is to track time spent on the task itself and allow for the recategorisation (or tagging) of the task type at a later date.  This increases flexibility but creates more complexity in the model which can increase the chance of overall failure to maintain data quality.

#### No task is an island

Similar to the challenges of categorisation, most modern work depends on collaboration and team work.  A good assessment of costs should account for meetings, work done in groups, training, reporting and all the other elements that make up a high-performing work environment.   Which is to say a time-sheeting output should not punish team work or helping others such that individual performance appears compromised. 

## Summary

Overall the challenges of time-sheets are many.  They require significant buy-in to get up and running and continuous effort to maintain and monitor.  Care should be taken before embarking on such an initiative and where possible consider opportunities to automate data-collection to avoid the perils of human error.

