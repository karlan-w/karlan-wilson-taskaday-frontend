# Project Title: Task A Day Application

## Overview

My application is a progress record application. Users can create a to-do list and use a focus timer to record their progress in completing each task. Users can reflect on the tasks completed retroactively and see their productivity in a week and month timeframe. 

### Problem

Focus timers and to-do applications rarely allow you to record your progress for your tasks or provide an understanding of your total productivity. The most common record of productivity is a binary yes, or no for task completion. This application will allow you to track the time spent on your focus tasks. 
### User Profile

Working professionals and students have the highest likelihood of utilizing the application. They are likely to find use as many of their tasks require mental focus. 

### Features

Navigation Bar: 

The navigation bar will provide easy access to the main pages of the application. It will remain simple, allowing the user to access the focus timer and the calendar. 

Data Visualization:

Users will be able to see the record of hours worked through the data record. It will be viewable on a weekly and monthly timeline. 

- The application will visualize the following: 
- Line graph of focus time for the week/month
- Average focus time 
- Average break time
- The percentage of focus time to break time is in a pie chart. 
- A count of the times the "I need a break now,"  button was selected. 

Focus Timer:

Users can utilize this timer to set focus time and associated break time. The focus time will be a countdown timer to record how long an individual has focused. Once complete, the break time countdown timer will appear letting the user know their break duration. Both will have pre-set alarms to alert the user when the countdown has completed. 

Long Break: 

Users can force a break period when needed which will be included in the calculation for break time. Instead of a countdown timer, this one will be a stopwatch and record the time spent until stopped by the user.  Once this break is over, they will return to the focus timer page with the focus timer reset. 

To-Do List 

Users can name specific tasks for the day in their to-do list. Users will be able to set focus goals for their timer based on the set duration of their focus period (focus time and break time). For example, a user may set a goal of three focus periods each of 50 minutes of focus and 10 minutes of break time. Each task will have an associated fraction value beside its name. The fraction will represent the number of tasks set (denominator) and those completed (numerator).  Each time a focus period is complete it updates the fraction and progress bar of the task.

Monthly Calendar: 

The date on the main page will default to the current date. However, users can select the current date and access the monthly calendar. Users can click into the calendar for a specific day and route to the focus timer page of the specific date selected. This will share a detailed view of the tasks created during this day, and the progress completed.

Progress Bar: 
This is a record of focus periods completed related to the goal set for the specific task created. This will be updated as the focus periods are complete. These will also change regarding the task that the user chooses to work on. 

Login Screen:
Upon entering the site, users will be prompted to log in or sign up for the application. They may choose to log in with Gmail and will be warned that their information may not be saved if they do not.

## Implementation

### Tech Stack

- Express JS  
- Axios
- Victory JS  
- SASS 
- React
- React Router  
- Passport JS 

### APIs

I will create my own API for this project. 

### Sitemap

Main Page: This page will house the navigation bar, the focus timer, and the to-do list module. 
Stats Page: The stats page will house the data visualization modules of the application.

### Mockups

See Mockup Folder 

### Data

There are a few major data points that will be used for the application. The date, the task and the time(focus time or break time) per task. Each date will have a task, each task will have an associated total focus time and break time. This will be updated to the closest minute and stored in the database for visualization purposes. All of these will be related to a specific user ID  as described by the token received when authenticated through Google. 


### Endpoints

There will be an endpoint to create, edit, delete and get the list of tasks for a particular date. There will be an endpoint to post an update of the time associated with a task to update the data record. 

### Auth

The application will integrate OAuth with Google Email. Users must have a functioning Gmail account before utilizing the application services. We will use the associated token to identify the user for CRUD purposes. 

## Roadmap

Week 1: June 10th - 16th 
- Create a git repo for the front end and back end. 
- Create database migration and seed files. 
- Create applicable routes.
- Create endpoint tasks for CRUD.  
- Test each using test data using PostMan or CURL. 

Week 2: June 17th - 23rd 
- Develop the Navbar. 
- Design main page.
- All breakpoints. 
 
Week 3: June 24th - June 29th 
- Design Stats page. All breakpoints. 

Week 4: June 30th - July 7th 
- Diving Deeper. 
- Review and test. 
- Deploy. 


## Nice-to-haves

The creation of a settings page. The user can edit the duration of the break time, focus time and the alarm that sounds when focus time is complete. 
The user can set dates and times for tasks ahead of time. They can then receive a text message at a pre-set time to remind them of the said task.