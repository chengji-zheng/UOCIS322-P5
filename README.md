# UOCIS322 - Project 5
## Overview
Brevet time calculator with AJAX and MongoDB!
Store control times from Project 4 in a MongoDB database.

###### Aurthor: Chengji Zheng
###### E-mail: chengjiz@uoregon.edu

## Descriptions
##### 	1. Like description said, this project is a continuous of project 4. Which stores data into a database. We chose MongoDB, a NoSQL server to store data.
##### 	2. In flask_brevets.py, we will create 2 more routes to handling correspond requirements, which are submit and display, two buttons on the client side.
#####	3. The logic under the server side to handle submission is (1) Grab the correspond JSON data from client side, which is dictionary type in python. Then use flask built-in insert_one() method to insert that JSON data into the database. The last step is redirect the route to the main page.
#####	4. For the client side, we will do two things. (1) Create a new file here called it display.html to display the entire database. (2) Edit in calc.html to implement submission
##### 	5. For the submission in calc.html, we first iterate through control class using jquery.each method, then checking the two elements "start_time_field" and "close_time_field" is empty or not. If not, then package them into JSON object using getJSON.

## Progress:
#####	1. `ERR_CONNECTION_REFUSED` Issue was fixed by editing on `docker-compose.yml` and `dockerfile` and `requirements.txt` three config files
#####	2. The webpage was successfully loaded
##### 3. The display.html looks good, but just displayed the data I submitted at the first time. Maybe I need to revise it in a smarter way -- Like clear the database after the user click submit button and then get new data and display on diaplay page.

### Known Issue(s):
##### 	1. When testing on those two buttons, it reports errors -- `405 (METHOD NOT ALLOWED)` and `500 (INTERNAL SERVER ERROR)` But the display page did show the date we want.
#####   2. Might need to look up the syntax to delete data in MongoDB
#####   3. Need testcases


## Credits
Michal Young, Ram Durairajan, Steven Walton, Joe Istas.
