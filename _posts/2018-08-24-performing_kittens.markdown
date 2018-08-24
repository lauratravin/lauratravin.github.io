---
layout: post
title:      "PERFORMING KITTENS"
date:       2018-08-24 00:34:10 -0400
permalink:  performing_kittens
---


Hello! I decided to show you how I created my ruby final project about kittens, I wil try to make it easy to undertand, not too much technicism and quick reading.

No kitten was harmed during the process and please remenber to adopt or save a kitten no matter her/his breed.

Since I am a visual designer I want to explain my project with images for make it more fun and easier.

The site I scrapped is  [here](http://www.vetstreet.com/cats/breeds) .

The main page contains 50 different breeds, that means I have 51 webpage to scrap at the end.


![image1](http://www.redhikari.com/clients/learnco/Project1.jpg)


 I managed my model in this way. Just tree basics classes. 
 
*  The scraper:  this guy have the terrific work of giving me the data usigng his friends NOKOGIRI and OPEN-URI formaly called gems.
*  The Breed:  Breed is the class who let me to intanciate  breed objects, save their name and web site initally. In a second phase (called method), she allow me to get the  breed characteristics, this attributes, getter and setter are created dinamically.
*  The CLI:  and for last but not least important CLI (Command Line Interface) class,  I think CLI has the hardest work here: deal with the "USER". 


![image2](http://www.redhikari.com/clients/learnco/Project2.jpg)

And my CLI has this behavier.

![image3](http://www.redhikari.com/clients/learnco/Project3.jpg)


The first approach was to get all the data scrapping them at the beginning.  Once I have the info it is to move throught the menu. But... yes there is a but...it takes some time to open 51 webpages for ruby. 
It is not like you start the program and go to buy a coffee and then it will show the data when you return, but (again) 
their is a naughty delay that is not a very USER - friendly.

![image4](http://www.redhikari.com/clients/learnco/Project4.jpg)

For solve this, a second approach was done, some code changed and now they Breeds characteritic are being upload according to user's behavier. 

![image5](http://www.redhikari.com/clients/learnco/Project5.jpg)



With this solution, I have 50% of chances of  user choosing a report (option 3 and 4) for fist time meaning that I will have the same naughty delay because I need to open 51 webpages to generate this information.

But suppossing the user choose between 1 or 2 option first, these options would be filling and completing the class Breed. If after the user choose option  3 or 4 from the menu,  less websites are required to be open.

You can find my code [here]https://github.com/lauratravin/CLIFP-Kitty/)  here and see how I implemented this.






