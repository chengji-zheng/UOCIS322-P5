# UOCIS322 - Project 5
## Overview
Brevet time calculator with AJAX and MongoDB!
Store control times from Project 4 in a MongoDB database.

###### Aurthor: Chengji Zheng
###### E-mail: chengjiz@uoregon.edu

## Descriptions
##### 	1. Like description said, this project is a continuous of project 4. Which stores data into a database. We chose MongoDB, a NoSQL server to store data.
##### 	2. In flask_brevets.py, we will create 2 more routes to handling correspond requirements, which are submit and display, two buttons on the client side.
#####		3. The logic under the server side to handle submission is (1) Grab the correspond JSON data from client side, which is dictionary type in python. Then use flask built-in insert_one() method to insert that JSON data into the database. The last step is redirect the route to the main page.
#####	  4. For the client side, we will do two things. (1) Create a new file here called it display.html to display the entire database. (2) Edit in calc.html to implement submission
##### 	5. For the submission in calc.html, we first iterate through control class using jquery.each method, then checking the two elements "start_time_field" and "close_time_field" is empty or not. If not, then package them into JSON object using getJSON.

### Known Issues:
##### 1. I edited `docker-compose.yml` and not sure how it works.
##### 2. I ran `flask_brevets.py` on my local computer, and it reports errors.
##### 3. I have no idea how to write testcases to test databases.
### 4. Will figure those issues out later and do another commit.

## Credits

Michal Young, Ram Durairajan, Steven Walton, Joe Istas.
