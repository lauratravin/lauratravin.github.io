---
layout: post
title:      "Redux: Summary"
date:       2021-06-16 03:21:21 +0000
permalink:  redux_summary
---


These are the tree fundamentals principles of Redux:

A)  Store is the unique source and this is complete true.
B)  States are read-only
C)  Changes are made through actions and pure functions


A) Store

The only valid state in the application is in the Store, when a component need information, it checks the Store.

Data travels throught component in only dirrection (1-way)

B) State

The state in Redux is a unique Javascript object, simil to a tree (JSON) and contain all the information that the application needs to manage.

C) Components only read the state, when need to manipulate the use the actions. Those actions call pure functions  called Reducers.

The reducers recieve the current status of the State and a logic to process that will mutate the state.







