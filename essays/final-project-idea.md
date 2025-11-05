---
layout: essay
type: essay
title: "Final Project Idea"
date: 2025-11-04
published: true
labels:
  - Engineering
  - Software Engineering
  - Nextjs
---

# Overview: UH Manoa Event Scheduler

## Name of Proposers/Authors
- Sakura Takahashi  
- Jiayi Lu  
- Kacy Kuniyoshi  
- Jordan Wong  
- Alicia Luck  

## The Problem
Currently, UH Mānoa has several different event calendars with varying functionality, which are all disconnected from each other.  
For instance, Hamilton Library has its own calendar with events such as trivia night and board game night; however, these events are not advertised on the [UH Mānoa Events Calendar](https://www.hawaii.edu/calendar/manoa/2025/11/5).  

Moreover, events cannot be filtered by category, often leaving users with inefficient visualizations. This results in students having to check multiple sites to find relevant events, which leads to lower attendance.

## The Solution
We will implement a mass event scheduler. This will allow various organizations to input their events on a singular website, allowing for efficiency and ease of use.  

Users will be able to filter by:
- Event type (e.g., sports, professional, entertainment)
- Location
- Time  

The web app will be built with Next.js, Prisma, and a PostgreSQL database.   
Events will be stored in structured tables (`Event`, `User`, `Organizer`, `RSVP`) and rendered dynamically on an interactive calendar.

## Approach 
This app will create an organized platform to present UH Mānoa–specific events in a unified student interface, with three role options.  

The app will include three roles:
1. **Users:** Students log in with their UH email, set event and location preferences, and view customized recommendations.  
2. **Organizers:** Event planners can upload and manage events related to their department, hall, or organization.  
3. **Admins:** Oversee organizer accounts, approve or edit events, and ensure quality control.  

Organizers will manage all event details such as:
- Time  
- Location  
- Topic  
- RSVP options  

Users will be able to include their preferences, like their favorite event and their specific residence hall. This will allow the app to show more content relevant to them and give accurate recommendations. 

---

# Use Cases

## 1. Users Searching for Events
1. User signs up with UH credentials.  
2. Navigates to the Calendar page.  
3. Selects interests and receives recommended events; irrelevant events are hidden.  
4. Toggles filters (event type, size, location).  
5. Views RSVP or interest indicators for signed-in users.  
6. RSVPs to events and receives reminder notifications.  

## 2. User Hosting an Event
1. User logs in with Organizer credentials.  
2. Navigates to Create an Event page.  
3. Fills in event details:  
   - Date, time, and location  
   - Category and summary  
   - Flyers or website links  
   - Sponsor and ticketing information  
4. Optionally provides an external calendar link to import events.  

## 3. Admin Editing the Page
1. Logs in with Admin credentials.  
2. Visits the page with admin-only edit tools visible.  
3. Documents and implements approved edits or changes.  

---

# Mockup Page Ideas
- Landing Page  
- User Home Page  
- Admin Home Page  
- Organizer Home Page  
- Event Search / Category Pages  
- Add / Delete / Edit Event Page  
- Calendar Page  
- Event Detail Page  
- Campus Map Page  
- (Optional) User Profile Page  

---

# Beyond the Basics
Additional planned features include:
- Notify students via email and SMS reminders of upcoming events that they have RSVPed for and notifying similar events that are coming up that they might be interested in..
- Map viewing showing the location of nearby events.  
- System for reviews on events, allowing RSVP students to give anonymous feedback of the event after they have attended.   
- Allow users to ‘like’ certain events that would give the program better suggestions on what kind of events a user would like to attend for personalized reccomendations.
- Engagement points for people who attend events and reward badges for users to unlock. (i.e “Athletics Fan”, “Music Jammer”, “Foodie”, etc.)
