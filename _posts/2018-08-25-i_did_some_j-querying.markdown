---
layout: post
title:      "I did some j-Querying"
date:       2018-08-25 23:05:11 -0400
permalink:  i_did_some_j-querying
---


To spruce up my Ruby on Rails Project, Babylonia, I have added some new functionalities using j-Query front end and an Active Model Serialization JSON Backend. The three new functionalities include:

- The daily logs index JSON API.
 This renders all baby's dailylogs on the baby's show page. The baby show page doesn’t automatically show all the baby log details. You will need to click a button ‘More Logs’ to view all of the logs. If the button is clicked the second time, the logs collapses. I have added a json api in the backend that takes baby id and uses that to pull all of the babies logs, renders json in the daily logs controller and uses JQuery to display the information on the baby show page. 
   
	 
 
- The baby’s show API
When a mom or caregiver has many babies, to view each baby's profile, each owner will have to always go back to their profile page and click on the baby's name. With this new feature, each owner is able to view each babies profile from the  baby's show page by just clicking a ‘Next Baby’ button. First, I created a method to extract all babies belonging to either the a mom or caregiver depending on who is logged in. This array of babies is then used to define which baby to show after the Next baby button is clicked.
 
- The New baby profile form
This renders the details of a new baby created on submit without refreshing the Mom's show page.  When mom fills the new baby form, she will get information about this new baby after submitting the form. The responses from the form are transformed into JSON responses which is then converted to a Javascript Prototype Object. The result is then appended to the DOM using a function added to the prototype which displays a sucess statement and some of the baby's information.


Those are the new features that have been added in this Jquery project. The hope is to continue to add new features as I continue to build my skills.


