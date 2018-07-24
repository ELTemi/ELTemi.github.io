---
layout: post
title:      "Rails App - From Baby to Babylonia!"
date:       2018-07-24 00:59:31 -0400
permalink:  rails_app_-_from_baby_to_babylonia
---

Wow! This just keeps getting more interesting. I finished building the Babylonia App - A way for moms and caregivers to keeps tabs on their babies while they are out and while the baby is with a caregiver. I choose this idea because I have an 8month old baby and I am planning to resume work soon. I’m already getting the baby fever, lol.
The Babylonia App is a simple way of monitoring your baby when they are with any type of caregivers from nannies to daycare nursery assitants.

I have 5 models

Baby 
Mom
Caregiver
Dailylog
User


There are two sign up forms, mom sign up which takes the mom to her profile page and the caregiver sign up which also takes the caregiver to the sign up page. A mom can add a baby and choose a caregiver through her profile page. She can also view all her baby’s logs for each page. 

The caregiver is the one to create the log for each baby and can input time the baby came in, how many times the baby took a nap, changed diapers, had food, how many hours of playtime and also a general summary of the baby’s activity during each day. I also included a time out attribute.

Each baby has its own attributes when the baby was added to the mom’s profile including name, date of birth, allergies, who else is authorized to pick up the baby among others. I created a nested route between the baby and the dailylog so that you can view all the dailylogs for each baby. An example would be for baby with Id: 2, you can go directly to babies/2/dailylogs or babies/2/dailylogs/5.

Other features includes using bcrypt to secure the password and ensures the user is authenticated before successfully logging in. You can also log in through Facebook. I included a filter on the caregivers index page if you wanted to view all the caregivers with the <5 years, 5-10years and >10years. 

Upgrades for version 2
- I hope to include availability for the caregiver so that when a mom wants to choose a caregiver, she will only see caregivers that are available.
- Add some new models related to each log activity so that we can have more detailed log for a baby. An example would be, adding a range for sleep time and playtime 

I will continue to expand the features of this project as I continue to learn new things. Moving on to JavaScript!!!

You can view my app using the repo link below
git@github.com:ELTemi/babylonia.git
