
#Stockbook
### jjd5870_cse5335_project2
It is a web application that keeps track of users and their posts. A person can post as well as play a role of admin. The role of admin can also be limited to particular users with few changes in code. It has 3 pages. the first page is login page. The second page is for adding, updating, deleting and viewing all posts (stocks). The third page is Site administration. It reccords the number of users, number of times they logged in and number of stocks. It is also able to download all the data that it records according to need of user. It shows 20 stocks per page.
 


 A [link](https://jjd5870-cse5335-2.herokuapp.com/)
 It is advisable to run it on ubuntu/linux. The graphics in Windows might not work properly but the functionality is working.
 One can sign up or use login details as: username: user7 password:123456
 
 
##Server Framework
I have used Ruby on Rails for server side programming. I am new to web development so all frameworks were equally unknown to me. I am a python programmer and I found similarity in coding of Ruby and Python so I chose it. It is also one of the fatsest framework. I have used PostgreSQL for storing data on server side. I found PostgreSQL similar to MySQL and a bit easier too.


##Client Framework
I have used javascript, JQuery and AJAX to maintain client-side. The reason to use it was that many resources were available online for it. I have used AJAX to handle the search requests from client and retrieve the data from server.
AJAX calls are based on RESTful APi, the page does not nedd to be refreshed to add and show new items.

##Aspects

###Hard Aspect
It has very complex structure. It is hard to understand the flow of data in the framework. Once we are clear with the flow of parameters in the framework, it becomes easy to make an app.
I have used gem rails_admin which is very useful and makes lots of work easier.

###Easy Aspect
It is very compact so changing the code or updating the application was easier to check. The method of scaffolding is very easy way to jump start an application for a single database model.

##Other Components
I have loaded several gem files such as  
gem gmap4rails - It is used for google maps api  
gem geocoder - It is used for google maps too but for conversion of cities to points and vice versa    
gem rails_12factor - It is used to use all the features on heroku    

##Reference
stuk.io videos on youtube were extremly helpful.
Stackoverflow

##Steps on Ubuntu to deploy app

Run command "bundle install" in your project folder.  

Install the Heroku Toolbelt  
Download and install the Heroku Toolbelt or learn more about the Heroku Command Line Interface.  
If you haven't already, log in to your Heroku account and follow the prompts to create a new SSH public key.  
$ heroku login

Clone the repository  
Use Git to clone jjd5870-cse-5335's source code to your local machine.  
$ heroku git:clone -a jjd5870-cse-5335  
$ cd jjd5870-cse-5335  

Deploy your changes  
Make some changes to the code you just cloned and deploy them to Heroku using Git.  
$ git add .  
$ git commit -am "make it better"  
$ git push heroku master  

You might need to use command- heroku run rake db:migrate 
