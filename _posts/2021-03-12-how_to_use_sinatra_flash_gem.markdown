---
layout: post
title:      "How to use Sinatra  Flash Gem"
date:       2021-03-12 20:25:25 -0500
permalink:  how_to_use_sinatra_flash_gem
---



As was told to user gem 'rack-flash3' to user messages but after fighting and lack of information I never could make this gem works. Thankfuly to Mr. Google I found Sinatra Flash Gem that also works on Rails. 

There are plenty of page and forums about and it lets you send messages to the erb pages and can be easily implemented.

Here is my cook recipe for use the gem just for quick messages

Configuration:

1.- You need the gem in you gem field. Just add gem 'sinatra-flash'

2.-Run bundle install, gemfile.loc will be generated.

3.-You need to work with sessions, add enable :sessions to you main Application controller file.

4.-Require 'sinatra/flash' in the same file.

5.-Additionally, if you are using Sinatra::Base add this line: register Sinatra::Flash

6.-You can use a message in a validation for example like here:

 ![img1](http://lauratravin.info/randomfiles/NYC-vaccine1.jpg)
					
7.-In the erb view you will add something like this:

  ![img2](http://lauratravin.info/randomfiles/NYC-vaccine2.jpg)	
		 
8.-You can add styles to the message. I just add an '<span>' with color red since it is a symple application. 
  ![img3](http://lauratravin.info/randomfiles/NYC-vaccine3.jpg)	

9.-The gem comes with a helper to create styles, but as I undertood from the creator,  it does not work well on Rails.

10.-How it can be helpful from someone. 



	 


