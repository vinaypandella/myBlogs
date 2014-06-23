---
layout: post
title:  "Lean Principles @ Software Development - I"
date:   2014-06-15 22:04:30
categories: Lean
comments: true
excerpt:  leandevelopment
---

Nowadays we commonly hear about agile methodology an agile practices now a days in IT industry, I always have feel that 'Agile at Scale ' is a bigger problem organizations are facing now a days when trying to adopt to agile process or agile delivery process.All agile practices works pretty well in smaller to medium sized organizations when it comes to bigger organizations/enterprises the co-ordination should happen between large no of teams which are not co-located.
Though i have worked in different organizations who follow agile and begin trained by IM [Iteration Manager ]/Agile coaches several times regarding Agile still i feel like something is missing, in search for origins of Agile i came across 'Lean Principles' and am surprised while going through the principles and came to know that all these agile principles are been adopted from Lean Principles.
If every member in the organization at every department knows about this 'Lean Principles' and been educated about these core principles from Lean ' Agile at Scale ' becomes easier.

Following are the few insights from the book Lean Software Development: An Agile Toolkit: An Agile Toolkit (Agile Software Development Series) Pearson Education , most of the material below is how the lean principles can be adopted to Software Development.

Lean software development applies a wealth of information about applying lean techniques from industrial setting to software development. Wait for the requirements than to build up the application in anticipation of the requirements yet the ideal is to deliver the application immediately when the requirements are ready.

Following are the seven principles at high level

+   Eliminate Waste
+   Amplify Learning
+   Decide as late as possible
+   Deliver as fast as possible
+   Empower the team
+   Build integrity in
+   See the whole

We will go deeper in to the first principle Eliminate Waste in the below article

First Principle : Eliminate Waste
---------------------------------

<i>Origins of Lean Thinking</i>
In the late 1940s all the car manufacturing companies used to follow the mass production strategy. Mass production was the cheapest way to make cars which is making the same kind of car in large quantities.

In this era Toyota set out to manufacture cars for Japan market for cheaper price. Japan market at this time not large enough to use the Mass production strategy so the question was “ How could Toyota make cars in small quantities but keep them as inexpensive as mass-produced cars?”

To solve this problem Toyota Production system emerged to form the basis of a whole new way of thinking about manufacturing, logistics and eventually product development. At the heart of this thinking was fundamental lean principle : Eliminate Waste.

In this principle anything that does not create value for a customer is considered as waste.
<ol>
<li>   A part that is sitting around waiting to be used is waste. </li>
<li>   Making something that is not immediately used is waste.       </li>
<li>   Motion is waste. </li>
<li>  Transportation is waste.</li>
<li>   Waiting is waste.            </li>
<li>   Any extra processing steps are waste.</li>
<li>   Defects are waste.                        </li>

</ol>

If something does not directly add value as perceived by the customer, it is waste.every step in the waterfall model other than analysis and coding is considered as waste.

Following are the different wastes that have been identified in manufacturing processes and we can see how those can be related to software development.

<table border="1">
<tr>
 <th>  Wastes of Manufacturing  </th> <th>  Wastes of Software Development  </th>
</tr>
<tr>
 <td> Inventory </td> <td> Partially Done Work </td>
</tr>
 <td> Extra Processing </td> <td> Extra Processes </td>
 </tr>
 <tr>
 <td> OverProduction </td> <td> Extra Features </td>
 </tr>
 <tr>
 <td> Transportation </td> <td> Task Switching </td>
 </tr><tr>
 <td> Waiting </td> <td> Waiting </td>
 </tr>    <tr>
 <td> Motion </td> <td> Motion </td>
 </tr>        <tr>
 <td> Defects </td> <td> Defects </td>
</tr>
</table>


Partially Done Work
-------------------

Partially done software development has a tendency to be obsolete, and it gets in the way of any other development work that we do.

Problems with Partially Done Software Development

Since it is not in production you have no idea whether it will eventually work in production.
You might have the business requirements ,  design documents and pile of code which is well covered with unit tests and may be with functional tests too, but you really don’t know if it solves the business problem until it is in production.

What if the system never gets in to production? There is bit investment to write off.

Minimizing the partially done software development is a risk-reduction as well as waste-reduction strategy.


Extra Processes
---------------

Paper work or documentation's seriously is that all really necessary.
<ol>
<li>It consumes resources</li>
<li>slows down reps one times.</li>
<li>hides quality problems.</li>
<li>gets lost.</li>
<li>degrades and becomes obsolete.</li>
<li>no one cares to read adds no value.</li>
</ol>
Does customer really finds this paper work or documentation more valuable? Some of the projects requires paper work or documentation as the required deliverable but does not mean that it adds value.

If at all for a project if it is required you should follow the below.
<ol>
<li>Keep to short</li>
<li>Keep it high level.</li>
<li>Do it off line.</li>
</ol>

There are exceptions to these there might be some safety critical systems which are frequently regulated and often required to have written requirements, traceable to code, in this case instead of preparing bunch of documents about the requirements which can be used to evaluate the functionality of the delivered application it would be better if requirements are written in a table-driven or template driven format which can be understood by both users and developers.

A good test to check if we need paperwork or not is to check if any one is eagerly waiting to use them for coding, testing and writing training manuals then these probably add value.

Always try to eliminate the documentation work and see if it can be communicate in any other efficient way for example writing acceptance tests instead of writing requirements. In general delay documentation details of a feature until the iteration in which they are implemented.


Extra features
---------------

How would an extra feature come in to an application and how does it becomes as a waste?

Business owners might think that this feature might be good just in case if it is needed in future.
Developers might like to add a cool technical feature which is not needed but just wanted to see how it works.

All these sounds good and harmless , but all these a serious waste. Why ? Every bit of code is to be minted by life time which means it should be completed , tested and integrated every time a change is made.

Every bit of code adds the complexity to the system and might be potential failure point.

There is great possibility that all this extra might become obsolete before its used.

Resist the temptation , If the code / feature is not needed now putting it in to the system is a waste.


Task Switching
--------------

Assigning resources to multiple projects is a source of waste.
Every time developers switch between tasks, a significant switching time is incurred as they get their thoughts incurred and get in the flow of new task.

Belonging to multiple teams means more interruption and more task switching. This task switching time is waste.

The fastest way to complete two projects that use the same resources is to do one at a time.

Say that you have two tasks, each task task takes two days to complete.If you start working on one of them, it should get completed in two days.When it is done you can start the second task and it should get completed in two days.What if you start working on both tasks together and expect to switch between the tasks in between them?First of all neither of them will get completed in two days, but will they both get completed in four days? When you add switching time, they will probably take longer than four days near to five days.


Waiting
-------

Biggest waste in software development is to wait for things to happen.

Delays are common on software development processes, and it seems counter intuitive to think of these delays as waste.

Some of the delays

+   Delays in starting project.
+   Delays in staffing.
+   Delays due to excessive requirements documentation.
+   Delays in reviews and approvals.
+   Delays in testing.
+   Delays in deployment.

How would delay effects customer? Delays keeps customer from realizing value as quickly as possible.

When a critical customer need arrives in your development organization, the speed with which you can respond is directly related to the systematic delays in your development cycle.

Motion
------

When a developer has a question, how much motion does it take to find out an answer?

Are people at hand to help with a technical problem or to address any business questions?

Development is an activity that requires great concentration, so walking down the hall take a lot more time than you might think.Developer might even took some time to reestablish the focus as it took to get the question answered.

It is for this reason the agile software development practices generally recommend that the team work in a single room every one has access to every on in the team at any time of development.

It may only relate to people, often even the artifacts move around.

The biggest waste of in all document hands off is that documentation don't cant really contain all information that the next person needs.

Defects
-------

The amount of waste caused by a defect is the product of the defect impact and the time it goes undetected.

A critical defect that is detected in three minutes has less impact than the minor defect which is undiscovered for months.

To reduce this waste find the defects as early as possible. Test immediately integrate often and release to production as soon as possible.

Management Activities
---------------------
Management Activities do not directly add value to a product, but they do have a big impact on waste in an organization.

Project tracking and control systems also do not add value, and further, they may be an indication of too much work in the system.

Authorization systems that are set up to review and approve changes to requirements often add significant delays as opposed to adding value to the customer.

Consider Project Prioritization and work release system. If the work release system is good we don't need much of project prioritization.

Authorization systems that are setup to review and approve changes to requirements often add significant delay as opposed to adding value to customer.

Learning to see waste is an ongoing process of changing the way you think about what is really necessary.

Map your Value Stream
---------------------
Mapping your value stream is a good way to start discovering the waste in your software development process.Creating a Value Stream map is a paper and pencil exercise you can easily perform while walking around your organization.
Your goal is to draw chart of the average customer request, from arrival to completion.Working with the people involved in each activity, sketch all the process steps necessary to fill the request, as well as the average amount of time that a request spends in each step.

You might have already seen the following value map for the projects you have worked in water fall model.

![ValueStreamWaterfall]({{ site.url }}/images/ValueStreamWaterfall.png)

In the above value stream map RED is for wait time  and GREEN is activity time. The customer sign-off takes more time because customer thinks it as an higher risk since this map indicates that they dont get another chance to review and change what they need.In all other phases there are several reviews involved with client and even with external times which is adding more wait time in each and every phase.

Value stream map for agile looks like follows

![ValueStreamAgile]({{ site.url }}/images/ValueStreamAgile.png)

The initial value stream map indicates that customer sign-off might be a source of irritation as well as delay.It shows design reviews and reviews at all phases should be moved inline with development, since they are currently a great source of delay.
Finally it indicates that planning for deployment should occur earlier in the process.Since the team has decided on agile development, it will solve the problems by moving in to incremental development, gathering requirements as needed, integrating design reviews with coding and planning early for regular deployments.


Thank You for reading this will post the remaining principles soon, Try This

+   Take some time to discuss each of the seven wastes of software development.
+   Develop a value stream map for your organization. Start with an incoming request and map timeline of its progress to providing customer value.Find out how mich time is spent to add value and how much time in waiting.Identify the biggest cause of delay and try to cut delay.


