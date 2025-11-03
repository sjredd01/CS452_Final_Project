# Project Summary 
The projects purpose is to give land lords and tennets an easy and convient way to submit and track maintenence requests. Tenets will be able to scan a unique QR
code for there apartment or housing unit. Then be able to submit a maintence request. When it is submitted they are giving a number that they can use to track the status 
of the maintence request. The land lord will have dashboard with the maintence requests and be able to keep track of the requests and see what was requested.

# Rough ERD Diagram

Here is a basic erd diagram of our initial idea. We will be accessing lots of strings and ints. mostly from the ticket table.

<img width="1982" height="636" alt="drawSQL-image-export-2025-11-03" src="https://github.com/user-attachments/assets/109283e6-3303-4505-b051-9fbf77bc627a" />


# Rough System Design

User -> Browser
Browser -> index.html / main.ts -> AppModule (app.routes.ts)
AppModule -> Feature Modules:
  - Auth (login, register)
  - Tickets (ticket-dashboard, ticket-component, user/admin tickets)
  - Groups (create-group, edit-group, admin-dashboard)
Feature Modules -> Feature Services (login-service, ticket-service, admin services)
Core Services -> HttpInterceptor -> Backend API (REST)

# Goals for Project

By the end of week one we hope that we have a functioning product 
By the end of week two we hope to have many of the major bugs to be fixed 
By the end of week three we hope to add more quality of life features that we come up with along the way 
by the end of week four we hope to have product that will be good enough to try to give to actual land lords and tennets.  
