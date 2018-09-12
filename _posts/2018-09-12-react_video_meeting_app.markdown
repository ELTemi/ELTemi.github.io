---
layout: post
title:      "React Video Meeting App"
date:       2018-09-12 18:39:07 +0000
permalink:  react_video_meeting_app
---


So its the final project before the almighty graduation. I decided to push myself really hard for this project so i decided to build a video meeting app that uses the Twilio programmable video to connect people. The main purpose of my app was to help businesses organize video calls with their clients.

Stateless components including:
- Business 
- Calllogs 
- ContactForm
- Contacts
- NavBar
- VideoCall


Container components

- Call Container which contains the Video Call Component that allows you to enter a meeting name and connects you to the call
- Call History Container contains the CallLogs component and displays details of all previous meetings
- Contacts Container contains the ContactForm and Contacts components used to keep information of all the businesses contacts

Actions

- contact action fetches the contacts that have been persisted to the rails api
- fetchRooms grabs all completed meetings from the twillio/rails backend api

Reducers

- contacts reducer handles the FETCH_CONTACTS action and is transferred to the combine reducers function
- rooms reducer also deals with the FETCH_ROOMS action

The App component displays the NavBar component and all 3 containers
Lastly, index.js which displays the single App Component.

In the end, this project pushed me to work with a completely new api(Twilio) and I definitely learned a lot.


