---
layout: post
title:      "Rails Final project"
date:       2021-04-11 15:31:06 -0400
permalink:  rails_final_project
---


Project is about?
The project is an web application about races and the runner registration for a sport organization, in which a user (Admin) can create and manage races, user, registrations. The users (runners), can find the available races offered during the calendar year and create a registration. 
User also can set a miles goal that will be automatically updated as soon as the race's date is expired. The admin of the system should load the pace result of each runner, it should be done automatically but for the purpose of the project it is done manually.

At the moment it does not have the logic to knwo if the runner ran or not, but it is something that can be added in the future.

Process description:
* Describe the models, attributes and relationships (associations)
* Create the flow and define what information we want to show and which data with need to create that information.
* Create the migrations 
* Create the controllers
* Create the views
* Create the helpers 


![img1](https://www.redhikari.com/clients/learnco/Rails-blog-1.jpg)



![img2](https://www.redhikari.com/clients/learnco/Rails-blog-2.jpg)



**Flows**

1) Admin creates a Race.
2) User signs up, then login, add a goal for 2021 and chooses a race to run.
3) User runs the race and the race is closed. Admin update the race status checking date. Automatically, race's miles are discount from User's goals.
4) Admin adds the race result. The Admin board/index page are updated with results.


**View definition
**
![img3](https://www.redhikari.com/clients/learnco/Rails-blog-3.jpg)








