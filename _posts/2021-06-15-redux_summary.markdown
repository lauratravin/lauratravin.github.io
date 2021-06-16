---
layout: post
title:      "Redux: Basic and history"
date:       2021-06-15 23:21:21 -0400
permalink:  redux_summary
---


These are the tree fundamentals principles of Redux that resumme what Redux do and we should remember.

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

![img1](https://www.redhikari.com/clients/learnco/blog1.png)


**History**

It is said that Redux is a creation of Facebook, but this is partially true.  Let's do some history and try to understand why Redux exists.

So the big bang occurs and MVC model was born. In the course we use it in Sinatra and Rails Modules.

MVC is well-known for its three-layer development architecture and it divides applications into three components:

Model: Maintains the data and behavior of an application
View: Displays the model in the UI
Controller: Serves as an interface between view & model components

Whenever the controller receives the request from the user, it uses the Model & View and generates the response sending it back to the users.

So one day people at Facebook that thought the MVC was very complicated and have some free time, decided to do some changes to the MVC architecture and created Flux.

The Flux architecture is based on the following components:

Store/ Stores: Serves as a container for the app state & logic
Action: Enables data passing to the dispatcher
View: Same as the view in MVC architecture, but in the context of React components
Dispatcher – Coordinates actions & updates to stores

In the Flux architecture, the flow works like this:
User clicks --> View creates an action --> the action creates new data and sents it to dispatcher --> Dispatcher delivers the action to the correct Store (here we have more than 1) --> Sore updates state and sends update to the view.

![img1](https://www.redhikari.com/clients/learnco/blog2.png)


In 2015 these two guys, Dan Abramov & Andrew Clark had the idea that Flux could be more easy to manage and invented Redux.

Redux is a library, which implements the idea of Flux but in quite a different way. Redux architecture introduces new components like:

Reducer: Logic that decides how your data changes exist in pure functions. Application event is denoted as an Action, which is dispatched to the reducer
Centralized store: Holds a state object that denotes the state of the entire app





















