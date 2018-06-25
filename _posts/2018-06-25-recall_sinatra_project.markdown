---
layout: post
title:      "Recall Sinatra Project"
date:       2018-06-25 14:12:46 +0000
permalink:  recall_sinatra_project
---


Yaaay! My Sinatra project is complete. I built out an appointments tracker called recall where you can just make a list of all the appointments that you have including the date, location and details of the appointment. It’s amazing to see how much goes into actually building each of these models, views and controllers. 


I had two models, a User class and an Appointments class with two associations. The user has many appointments and each appointment belongs to a user. The user can sign up, login, view all their appointments, create a new appointment, edit an appointment and delete the appointments. Each view was also protected to ensure that only a user logged into their account can read, edit or delete appointments. 



The username and password fields on the sign up and login pages were required and they have to be unique to my database. The create appointment page also had a required title field. I also used bycrpt to ensure that passwords and authenticated and protected for each user as they sign up and login. Each view has been designed to be private to each user because of the nature of the app.

Its interesting how the little details can make or break your application and it was so much fun learning to protect views for the users.
