[![CI](https://github.com/outdoor-buddies/my-nextjs-application/actions/workflows/ci.yml/badge.svg)](https://github.com/outdoor-buddies/my-nextjs-application/actions/workflows/ci.yml)

# Outdoor Buddies

## Table of contents

* [Overview](#overview)
* [Deployment](#deployment)
* [User Guide](#user-guide)
  * [Landing Page](#landing-page)
  * [Sign in and sign up](#sign-in-and-sign-up)
  * [Index pages](#index-pages-announcements-hike-recommendation-groups-profiles)
  * [Home page](#home-page)
* [Developer Guide](#developer-guide)
  * [Prerequisites](#prerequisites)
  * [Clone the repository](#clone-the-repository)
  * [Database Setup](#database-setup)
  * [Running the Application](#running-the-application)
* [Development History](#development-history)
  * [Milestone 1: Mockup development](#milestone-1-mockup-development)
  * [Milestone 2: Data model development](#milestone-2-data-model-development)
  * [Milestone 3: Final touches](#milestone-3-final-touches)
* [Team](#team)

## Overview

### Project Goals

Outdoor Buddies aims to help students find others interested in hiking, running, and walking around Oahu. The application will allow users to create profiles, discover compatible groups and activities, join outdoor events, and share information about local outdoor locations.

The goal is to make outdoor activities more accessible, social, and safer by helping students connect with others who share similar interests and preferences.

## Deployment

Our application is actively being developed and is deployed via Vercel.  
[View Outdoor Buddies Live](https://my-nextjs-application-lbc3i1d4t-outdoor-buddies.vercel.app/)

## User Guide

This section provides a walkthrough of the Outdoor Buddies user interface and its capabilities.

### Landing Page

The landing page is presented to users when they visit the top-level URL to the site. This allows users to see what the mission statement of the website is to determine if they would like to utilize it. 

![](./images/landing-page.png)

### Sign in and sign up

Click on the "Login" button in the upper right corner of the navbar, then select "Sign in" to go to the following page and login. You must have been previously registered with the system to use this option:

![](./images/signin-page.png)

Alternatively, you can select "Sign up" to go to the following page and register as a new user:

![](./images/signup-page.png)

### Index pages (Announcements, Hike Recommendation, Groups, Profiles)

Outdoor Buddies provides four public pages that help users navigate the site in different ways. Users are encouraged to log in to their profiles when trying to access these different pages, and if they do log in they will be able to see what each page has to offer.

![](./images/profiles-page.png)

The Profiles page shows all the current defined Profiles and their associated Groups:

![](./images/announcements-page.png)

The announcements page offers the admins a way to interact with users through events and announcements. When a developer is signed in, they have access to a button to create an announcement that will redirect to page where they can input info to share with users whether it be events, updates or more.

An admin/developer can add and edit existing announcements in the announcements page

![](./images/announcements-page-add.png)

![](./images/announcements-page-edit.png)

![](images/hiking-recommendations-page.png)

The Hike Recommendation page shows hikes that people like to do and recommend for newcomers to Hawaii. This is to get a feel for if a certain hike is right for them:  

While it isn't shown, the search function does work and searches by name of the trail and the location.

The Groups page shows all the currently defined Groups from users on the website with their associated Profile, Interests, and Description:

![](./images/groups-page.png)

Once users are logged in, they can also create a new group if they would like, especially if they already have some friends in mind and they would like to get new people to join. On the top left, users can click the button and will be and will be redirected to a form:

![](./images/groups-page-add.png)

### Home page

After logging in, you are taken to the home page, which presents a form where you can complete and/or update your personal profile:

work in progress

## Developer Guide

If you are interested in running Outdoor Buddies locally, follow the instructions below.

### Prerequisites

Before running the application, make sure you have the following installed:

- Node.js
- npm
- PostgreSQL

### Clone the repository

Clone the application repository locally and navigate into the project directory and install required dependencies.
```
npm install
```

### Database Setup
Create a PostgreSQL database for the application.
```
createdb name-of-db
```

Copy `sample.env` and rename the copy to `.env` and update the `DATABASE_URL` to match your local PostgreSQL setup

Run database migrations using
```
npx prisma migrate dev
```

Generate the Prisma client:
```
npx prisma generate
```

Seed the database with default users and data:
```
npm run seed
```

### Running the Application

Start the development server by running:
```
npm run dev
```

If configured correct, the app will be available to view at http://localhost:3000

## Development History

### Milestone 1: Mockup development

The goal of [Milestone 1](https://github.com/orgs/outdoor-buddies/projects/1) was to create mockups of each of the pages for our Outdoor Buddies Website

### Milestone 2: Data model development

The goal of [Milestone 2](https://github.com/orgs/outdoor-buddies/projects/3) was to implement the data model: for hikes and for users/groups on the site. We also be fixed certain login issues and added basic features such as searching, adding, editing, etc.

## Milestone 3: Final touches

The goal of [Milestone 3](https://github.com/orgs/outdoor-buddies/projects/4) is to clean up the code base, implement features that we were unable to complete in Milestone 2, have some users test our app, add more entries into our tables, and maybe adjust some of the styles, including fonts, colors etc.

## Team

OutdoorBuddies is designed, implemented, and maintained by [Brycen Kano](https://brycenk05.github.io/) and [Kelly Masaki](https://kellym12.github.io/Professional-Portfolio/).  
Our [Team Contract](https://docs.google.com/document/d/11j764LAw7YHbRscZZDggGGVZIzsIFAGyGOxQO0eoB1g/edit?tab=t.0) is viewable here.
