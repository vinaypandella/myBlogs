---
layout: post
title:  "Agile Coding"
date:   2014-06-05 22:04:30
categories: Lean Agile Coding Development Software
comments: true
excerpt:  agilecoding
---

Knowing about agile practices and having basic idea on development/programming is not sufficient for a successful agile developer.
Following are the few principles which are required to be followed by an agile developer.

+   Program Intently and Expressively
+   Communicate in Code
+   Actively Evaluate Trade-Offs
+   Code in Increments
+   Keep It Simple
+   Write Cohesive Code
+   Tell, Don’t Ask
+   Substitute by Contract

Program Intently and Expressively
---------------------------------

Choose readability over convenience, code clarity comes before performance. Always remember that code will be read many times more than it is written, so it is worth it to make life easier to those who follow.

Communicate in Code
-------------------

Choose wisely the names of the methods and variables to be expressive. Comments should not shadow the expressiveness of the code. Instead, comments about methods should convey information about the purpose (why does the method exists) plus information about the arguments, return values and exceptions.

Actively Evaluate Trade-Offs
----------------------------

There is usually not a perfect answer to the best framework or development procedure (applicable to life too). So it is far more important to be aware what do we need to solve and choose the right solution/answer for that. Consider performance, convenience, productivity, cost and time. Let the stakeholder of the code you are writing mark you the focus you have to take.

Code in Increments
------------------

Like running a marathon, do not focus on the end point. Instead, try to put closer objectives. This iteration not just let you produce more focused software components (methods, classes, modules, libraries) but also takes care of your mental healthiness by not burning you. Write code in short edit/build/test cycles.

Keep It Simple
--------------

take that necessary time and keep it simple.

Write Cohesive Code
-------------------

Cohesion is the measure of how functionally related the members of a software component are. It feels like rowing all in the same direction. Cohesion empowers you to group similar members by their functionality. Special mention to the Single Responsibility Principle when writing classes that states that a method should have only one reason to change. Keep classes focused and components small.

Tell, Don’t Ask
---------------

Tell objects to do things based on their state. This business logic of the what the object does must reside inside the object itself, instead of playing with the object state in the calling class.

Substitute by Contract
----------------------

Inheritance vs. composition. If inheritance is chosen, overriding of methods should be done accepting the parent contract (not modifying its functionality) in such a way that the derived class can be substitute by the parent class. In most of the cases that you just want to add functionality to a class, though, composition is a most preferable option.

Please visit this again am updating this with code examples and also trying to get the metrics that can be used to identify these from the code.