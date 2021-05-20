---
layout: post
title:      "Create a search field with JS + Rails"
date:       2018-01-29 16:29:33 -0500
permalink:  things_that_struggle_me_the_most_about_learning_a_computer_language
---



Problem:
User enter his/her passport into the input field and click the search button, if the user exist in the back end, user' name and surname must be return.

Form details:



 ![cat_code](http://www.redhikari.com/clients/learnco/PE1.jpg)
 
 
 Since I am using classes and it is a webpage related to flights reservations, the class responsable for do the search will be the class named Passenger and the search will be done in the class method(static) searchPassengerByPassport.
 
 The class that posses the control of the modal and the form is Flight. She will show the modal and all the form elements includen search event.
 
In this code below, I obtain the search button and add an event listener. When the user clicks,  I obtenin the passport number, convert it into upper case and send it to the class Passenger to do the dirty work.

 ![cat_code](http://www.redhikari.com/clients/learnco/PE2.jpg)
 
 The class methot searchPassengerByPassport will reciebe the passport number in the variable term.
 
 This method will user the window method name fecth to request to the back to search for this specific passenger.
 
For the search I am going to use the tradition url that it's uses to get the list of all elements in Rails name as index route: 

const passengersURL = 'http://127.0.0.1:3000/passengers'

But in this case, I am goint to change the url with the parameter I want to search like this:


 ![cat_code](http://www.redhikari.com/clients/learnco/PE3.jpg)
 
 The rest of the fetch follow the typical construction, with a function to treat the object if it is found, where I assign the name and first name to the form and if it is not found I show a message to the user on the same form.
 
 
 On the backend side, we need to modify the index route for passenger controller
 
  ![cat_code](http://www.redhikari.com/clients/learnco/PE4.jpg)
	
	In this case there is a serializer but it work with it or without.
	
	

 


 
 
 












