---
layout: post
title:      "How to use Sinatra  Flash Gem"
date:       2021-03-12 20:25:25 -0500
permalink:  how_to_use_sinatra_flash_gem
---



As was told to user gem 'rack-flash3' to user messages but after fighting and lack of information I never could make this gem works. Thankfuly to Mr. Google I found Sinatra Flash Gem. 

There are plenty of page and forums about and it lets you send messages to the erb pages and can be easily implemented.

Here is my cook recipe for use the gem just for quick messages

Configuration:

1.- You need the gem in you gem field. Just add gem 'sinatra-flash'

2.-Run bundle install, gemfile.loc will be generated.

3.-You need to work with sessions, add enable :sessions to you main Application controller file.

4. Require 'sinatra/flash' in the same file.

5. Additionally, if you are using Sinatra::Base add this line: register Sinatra::Flash

6. You can use a message in a validation for example like here:

![img1](http://lauratravin.info/randomfiles/NYC-vaccine1.jpg)
					
7. In the erb view you will add something like this:

      <%if flash[:message] %>
                 <%= flash[:message] %> 
     <% end %>				
		 
8. You can add styles to the message. !
9. 
10. 
	 


