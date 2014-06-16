---
layout: post
title:  "Lean Software Development"
date:   2014-06-15 22:04:30
categories: Lean
comments: true
---


Applying lean industrial practices to Software Development


How to apply lean manufacturing principles / ideas to Software Development.

Applying Toyotas set based decision making principles or ideas to software design.

Traditional engineering (software and others) stresses analysis and early design decision making so down stream activities can proceed.

Set-based development stresses keeping multiple design options open in order to have as much as information as possible, not only about a particular piece or the design, but also about the integration of all pieces. Set-based development helps optimize the whole rather than the pieces. Simple design and refactoring serve similar purposes for software developers - pushing off certain design decisions in to the future when more information is available.

Set-based development therefore provides a parallel that adds credibility to agile practices but also shows how to extend those practices.

Lean software development applies a wealth of information about applying lean techniques from industrial setting to software development.

Wait for the requirements than to build up the application in anticipation of the requirements yet the ideal is to deliver the application immediately when the requirements are ready.

First Principle : Eliminate Waste

In the late 1940s all the car manufacturing companies used to follow the mass production strategy. Mass production was the cheapest way to make cars which is making the same kind of car in large quantities.

In this era Toyota set out to manufacture cars for Japan market for cheaper price. Japan market at this time not large enough to use the Mass production strategy so the question was “ how could Toyota make cars in small quantities but keep them as inexpensive as mass-produced cars?”

To solve this problem Toyota Production system emerged to form the basis of a whole new way of thinking about manufacturing, logistics and eventually product development. At the heart of this thinking was fundamental lean principle : Eliminate Waste.

In this principle anything that does not create value for a customer is considered as waste.
A part that is sitting around waiting to be used is waste.
Making something that is not immediately used is waste.
Motion is waste.
Transportation is waste.
Waiting is waste.
Any extra processing steps are waste.
Defects are waste.

Following are the different wastes that have beeb identified in manufacturing processes and we can see how those can be related to software development. Later we can see more info about these wastes in details and how we can avoid them.




Partially Done Work

Partially done software development has a tendency to be obsolete, and it gets in the way of any other development work that we do.

Problems with Partially Done Software Development

Since it is not in production you have no idea whether it will eventually work in production.
You might have the business requirements ,  design documents and pile of code which is well covered with unit tests and may be with functional tests too, but you really don’t know if it solves the business problem until it is in production.

What if the system never gets in to production? There is bit investment to write off.

Minimizing the partially done software development is a risk-reduction as well as waste-reduction strategy.


Extra Processes

Paper work or documentation's seriously is that all really necessary.
It consumes resources
slows down reps one times.
hides quality problems.
gets lost.
degrades and becomes obsolete.
no one cares to read adds no value.

Does customer really finds this paper work or documentation more valuable? Some of the projects requires paper work or documentation as the required deliverable but does not mean that it adds value.

If at all for a project if it is required you should follow the below.
Keep to short
Keep it high level.
Do it off line.

There are exceptions to these there might be some safety critical systems which are frequently regulated and often required to have written requirements, traceable to code, in this case instead of preparing bunch of documents about the requirements which can be used to evaluate the functionality of the delivered application it would be better if requirements are written in a table-driven or template driven format which can be understood by both users and developers.

A good test to check if we need paperwork or not is to check if any one is eagerly waiting to use them for coding, testing and writing training manuals then these probably add value.

Always try to eliminate the documentation work and see if it can be communicate in any other efficient way for example writing acceptance tests instead of writing requirements. In general delay documentation details of a feature until the iteration in which they are implemented.

Extra features

How would an extra feature come in to an application and how does it becomes as a waste?

Business owners might think that this feature might be good just incase if it is needed in future.
Developers might like to add a cool technical feature which is not needed but just wanted to see how it works.

All these sounds good and harmless , but all these a serious waste. Why ? Every bit of code is to be minted by life time which means it should be completed , tested and integrated every time a change is made.

Every bit of code adds the complexity to the system and might be potential failure point.

There is great possibility that all this extra might become obsolete before its used.

Resist the temptation , If the code / feature is not needed now putting it in to the system is a waste.


Task Switching

Assigning resources to multiple projects is a source of waste.
Every time developers switch between tasks, a significant switching time is incurred as they get their thoughts incurred and get in the flow of new task.

Belonging to multiple teams means more interruption and more task switching.This task switching time is waste.

The fastest way to complete two projects that use the same resources is to do one at a time.

TO DO :: Example of Task Switching

Waiting

Biggest waste in s/w development is to wait for things to happen.

Delays are common on software development processes, and it seems counterintuitive to think of these delays as waste.

Some of the delays

Delays in starting project.
Delays in staffing.
Delays due to excessive requirements documentation.
Delays in reviews and approvals.
Delays in testing.
Delays in deployment.

How would delay effects customer? Delays keeps customer from realizing value as quickly as possible.

When a critical customer need arrives in your development organization, the speed with which you can respond is directly related to the systematic delays in your development cycle.

Motion

When a developer has a question, how much motion does it take to find out an answer?

Are people at hand to help with a technical problem or to address any business questions?

Development is an activity that requires great concentration, so walking down the hall take a lot more time than you might think.Developer might even took some time to reestablish the focus as it took to get the question answered.

It is for this reason the agile software development practices generally recommend that the team work in a single room every one has access to every on in the team at any time of development.

It may only relate to people, often even the artifacts move around.

Digram about move.

The biggest waste of in all document hands off is that documentation don't cant really contain all information that the next person needs.

Defects

The amount of waste caused by a defect is the product of the defect impact and the time it goes undetected.

A critical defect that is detected in three minutes has less impact than the minor defect which is undiscovered for months.

To reduce this waste find the defects as early as possible. Test immediately integrate often and release to production as soon as possible.

Management Activities

Project tracking and control systems also do not add value, and further, they may be an indication of too much work in the system.

Authorization systems that are set up to review and approve changes to requirements often add significant delays as opposed to adding value to the customer.

Consider Project Prioritization and work release system. If the work release system is good we don't need much of project prioritization.

Revisit this section

Value stream  mapping






