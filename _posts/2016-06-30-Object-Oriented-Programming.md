---
layout: post
title: OOP
---

<h1>This is OOP!</h1>
OOP is great and allows us a tremendous amount of flexibility for having multiple systems interacting with the same data / logic. However, there is certainly a situation in which you wouldn't want to bother loading up a lot of objects.. Namely, when you are simply pulling data for tabular display.

Querying a database and getting a simple record set back that is immediately emitted to the browser usually doesn't need OOP involved. As a matter of fact you might want to sidestep OOP completely as tabular data usually involves a roll up of other information (sums of child records) and you normally don't want to pull more data from the database than what you are actually using. ie. if you are only showing the name and email you probably don't want to grab the user name as that is just wasted cycles.

Now, putting information into a DB usually involves making sure that certain business logic is followed. For example that the username follows certain rules. In those situations leveraging an OOP style keeps things a bit more encapsulated and easily transferred between systems.

So, looking at the specific example: I wouldn't bother with more than handing a datatable to a repeater when pulling data; but I would have a user class for when I'm going to create a new one or operate on that user to make sure the business rules are properly followed.
