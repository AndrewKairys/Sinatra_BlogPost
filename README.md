# Sinatra Project Calorie Tracker
This project features a RESTful MVC Framework with simple users and and meals with CRUD functionality.

Below I have a brief walkthrough of the Web App ![here](http://)




The process was straightforward in that I had a goal for a user to be able to track how many calories they consumed throughout the day. They would store their meal information: name, and calories. Upon a user being added to the database there is a form input field that ties into a daily_calories column in my sqlite3 database. I was then able to use erb to expose the user's daily_calories, then subtract the the total value of the column calories on the meals table. I used the ActiveRecord::Calculations methods pluck and sum to accomplish this. I also implemented a delete route that handles the Delete All button on my meals page tby destroying each meal object through the has_many/belongs_to relationship that was set up in the models of my framework. 
