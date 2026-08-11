[![CI](https://github.com/outdoor-buddies/my-nextjs-application/actions/workflows/ci.yml/badge.svg)](https://github.com/outdoor-buddies/my-nextjs-application/actions/workflows/ci.yml)

# Outdoor Buddies

## Table of contents

* [Overview](#overview)
* [Project](#project)
* [User Guide](#user-guide)
  * [Landing Page](#landing-page)
  * [Sign in and sign up](#sign-in-and-sign-up)
  * [Index pages](#index-pages)
    * [Announcements and Events](#announcements-and-events)
    * [Hikes](#hikes)
    * [Groups](#groups)
    * [Profiles](#profiles)
* [Developer Guide](#developer-guide)
  * [Prerequisites](#prerequisites)
  * [Clone the repository](#clone-the-repository)
  * [Database Setup](#database-setup)
  * [Running the Application](#running-the-application)
* [Community Feedback](#community-feedback)
* [Development History](#development-history)
  * [Milestone 1: Mockup development](#milestone-1-mockup-development)
  * [Milestone 2: Data model development](#milestone-2-data-model-development)
  * [Milestone 3: Final touches](#milestone-3-final-touches)
* [Team](#team)

___
## Overview

Outdoor Buddies aims to help students find others interested in hiking, running, and walking around Oahu. The application will allow users to create profiles, discover compatible groups and activities, join outdoor events, and share information about local outdoor locations.

The goal is to make outdoor activities more accessible, social, and safer by helping students connect with others who share similar interests and preferences.

### The Problem

People love taking hikes, running, and walking in Hawaii. There are many areas and paths with beautiful scenery all around Oahu. Sometimes people don’t feel comfortable hiking, running or walking by themselves, and it can be hard to find a group of people with whom to go.

### The Solution

The Outdoor Buddies App will allow students to login, create a profile marking certain preferences, view pre-existing groups or create a new one, and join with other students on the many beautiful hiking, running, and walking spots on Oahu. They can message each other within the app, post announcements for group hiking events, and create a community.

___
## Project

### Github

View the Outside Buddies Organization [here](https://github.com/outdoor-buddies)

View the Outside Buddies Development Page Repository [here](https://github.com/outdoor-buddies/outdoor-buddies.github.io)

View the Outside Buddies Project Repository [here](https://github.com/outdoor-buddies/my-nextjs-application)

### Deployment

To make Outdoor Buddies easily accessible to anyone, our application is actively being developed and is deployed via Vercel.  
[View Outdoor Buddies Live](https://my-nextjs-application-7pz8x81id-outdoor-buddies.vercel.app/)

___
## User Guide

This section provides a walkthrough of the Outdoor Buddies user interface and its capabilities.

### Landing Page

The landing page is presented to users when they visit the top-level URL to the site. This allows users to see what the mission statement of the website is to determine if they would like to utilize its services. There are also user reviews below to see if it is something they might be interested in. (in progress)

![](./images/landing-page-1.png)
![](./images/landing-page-2.png)

### Sign in and sign up

Scroll down and click on the "Sign In" Button or click on the "Login" button in the upper right corner of the Navbar, then select "Sign in" to go to the following page and login. You must have been previously registered with the system to use this option:

![](./images/signin.png)

Alternatively, you can select "Sign up" in the same locations as "Sign In" to go to the following page and register as a new user:

![](./images/signup.png)

Upon sign in/sign up, you will be redirected to the Announcements page of the website.

![](./images/announcements-events-page.png)

### Index pages

Outdoor Buddies provides four public pages that help users navigate the site in different ways. People are encouraged to sign in or sign up when trying to access these different pages, and if they do sign in they will be able to see what each page has to offer. If a user isn't signed in, they can't access these pages.

#### Announcements and Events

The Announcements page offers the admins a way to interact with users through Events and Announcements. Users can see new Events that they can join and Admins can post announcements for either upcoming events or changes to the website.

![](./images/announcements-events-page.png)

Users can hit the 'View Details' Button on any Event or Announcement to get more information about what is happening and when.

![](./images/event-details.png)

When an admin is signed in, this is what the Announcements and Events page will look like. Admins can connect with Users by sharing events, announcements, updates or more on this page.

![](./images/announcements-events-page-admin.png)

An admin can click on the 'Create Announcement' Button to create a new Event or Announcement and they will be redirected to the form below.

![](./images/add-event-form.png)

An admin can click on the 'Edit' Button to change the details of the Event or Announcement and they will be redirected to the form below. Editing applies to existing and future Announcements and Events. If an admin notices a mistake on an announcement or the date has passed. They can also click on the 'TrashCan Icon' Button to Delete the specific Event or Announcement.

![](./images/edit-event-form.png)

#### Hikes

The Hikes page shows hikes that people like to do and recommend for newcomers to Hawaii. Users who are new to Hawaii a way to get more information on the different hikes that people can do on Oahu. This is to get a feel for if a certain hike is right for them. While it isn't shown, the search function does work and searches by name, location, and description of the trail. There are also options to filter by difficulty and distance (in miles).

![](images/hike-list-page.png) 

Users can click on the name of the hike in blue and that will take them to a page with a text-blurb that gives more expanded details about the hike. Users can view more information about a hike including what to bring, what to look out for and more.

![](images/hike-details-page.png)

When an admin is signed in, this is what the Hikes page will look like. Admins can add and edit different hikes pages.

![](images/hike-list-page-admin.png)

An admin can click on the 'Create a Hike' Button to create a new Hike and they will be redirected to the form below.

![](images/add-hike-form.png)

An admin can click on the 'Edit' Button to change the details of the Hike and they will be redirected to the form below. Editing applies to existing and future Hikes. They can also click on the 'TrashCan Icon' Button to Delete the Hike (accounting for something like Stairway to Heaven, since people can't hike there anymore).

![](images/edit-hike-form.png)

#### Groups

The Groups page shows all the currently defined Groups from Users on the website with their associated image, number of members, and description. If applicable, it will also display the group's last event location as well as the date when it took place. While it isn't shown, the search function does work and searches by name and description of the group. There are also options to filter by commitment level.

![](./images/group-page.png)

Users can click on the 'Add a Group' Button to create a new group. This is especially helpful if they already have some friends in mind and they would like to get new people to join. Users can also create multiple groups. They will be redirected to the page below.

![](./images/add-group-form-empty.png)

Once it is filled out, the page should look something like this

![](./images/add-group-form-full-1.png)
![](./images/add-group-form-full-2.png)

Users can click on the 'View Details' Button to get more information on what the group is about: how many members are there, if there's a cap to how many members they will accept, and a description meant for the group to tell the world what it's about.

![](./images/group-details-page.png)

 If the User created the group themselves, then the details page will look like it does below.
 
![](./images/group-details-page-other.png)

Users can click the 'Edit Group' Button and they will be redirected to the form below that allows for editing the details of the group. They can also click on the 'TrashCan Icon' Button to Delete the specific Group.

![](./images/edit-group-form.png)

Below that is the 'Group Forum' Button which will allow users to post a question that they have for the group or a request to join the group. (Users can join more than one group if they would like, although they should understand what each group's expecations are). Below is an example of an empty forum.

![](./images/group-forum-empty-page.png)

Users can click the 'Create Post' Button to post a question on the forum. It will redirect the user to this form

![](./images/add-post-form.png)

Posting this results in the following image on the forum

![](./images/group-forum-post-page.png)

When an admin is signed in, this is what the Forum page will look like. Admins can delete different posts if they are deemed inappropriate.

![](./images/group-forum-post-admin.png)

#### Profiles

The Profiles page shows all the currently defined Profiles from Users on the website with their associated image, group name if applicable, and description. Only one profile per User. While it isn't shown, the search function does work and searches by name, status, groupname, and description of the profile.

![](./images/profile-page.png)

If the User hasn't created a profile yet, in the navbar, under the user email, Users can click on the 'View Profile' Button to create a new profile. This redirects them to the form below. Once the profile is created, the 'View Profile' Button will redirect to the same page as 'View Details'.

![](./images/add-profile-form-empty.png)

Once it is filled out, the page should look something like this

![](./images/add-profile-form-full-1.png)
![](./images/add-profile-form-full-2.png)

Users can click on the 'View Details' Button to get more information on what another user's goal is for registering on this website: a status statement for saying how one feels in the moment, a description box that can tell more, and if applicable to say if they are already in a group or not (users can join multiple groups).

![](./images/profile-details-page-other-1.png)
![](./images/profile-details-page-other-2.png)

 If the User has already created the profile themselves, then the details page will look like it does below.
 
![](./images/profile-details-page1.png)
![](./images/profile-details-page2.png)

Users can click the 'Edit Profile' Button and they will be redirected to the form below that allows for editing the details of the profile. They can also click on the 'TrashCan Icon' Button to Delete the Profile. Once the profile is deleted, 'View Profile' will again redirect to the same form used to create a profile.

![](./images/edit-profile-form-1.png)
![](./images/edit-profile-form-2.png)

___
## Developer Guide

For new developers that are joining the project and need to run Outdoor Buddies locally, this guide provides an in-depth explanation on how to download, install, and run Outdoor Buddies.

### Prerequisites

Before running the application, make sure you have the following installed:

- [Latest Node.js](https://nodejs.org/en/download) (Comes with npm)
- [Latest PostgreSQL](https://www.postgresql.org/download/)
- [Latest Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- Code Editor

#### Optional

These are reccomended to make navigation and seeing components easier

- Code Editor (Reccomended): [VSCode](https://code.visualstudio.com/Download?_exp_download=fb315fc982) (although other editors or IDES may be used)
- [Github Desktop](https://desktop.github.com/download/)
- [pgAdmin](https://www.pgadmin.org/download/)

### Clone the repository

First, clone the [Outdoor Buddies](https://github.com/outdoor-buddies/my-nextjs-application) repository locally using Github Desktop and navigate into the project directory via your editor or IDE and install required dependencies.

### Install Dependencies

```
npm install
```

You will be able to view all of the files associated with the project and edit features or even implement your own!

### Environment Setup

This project requires a .env file (I'm not sure )

NextAuth configuration
Database connection (PostgreSQL)
Prisma
Session keys
figure out how to rephrase above

Create a `.env` file ...

### Database Setup
Create a PostgreSQL database for the application.
```
createdb outside-buddies
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

If you modify the Prisma schema or want to push the schema to the database:
```
npx prisma db push
```

Seed the database with default users and data:
```
npx prisma db seed
```

### Running the Application

Start the development server by running the command:
```
npm run dev
```

If properly configured, the app will be available to view at http://localhost:3000
(You can put this link into a browser, or if using VSCode, clicking the 'open link' when hovering over the link)

### Testing (Optional)

### Playwright

Testing is done with Playwright. You can run the browser tests with the following steps.

Install Playwright:
```
npx playwright install
```

Run Playwright Tests:
```
npx playwright test
```

#### ESLint (Quality Assurance)

Run ESLint for Linting issues
```
npm run lint
```

### Directory Structure

A brief overview of the repository layout:

```
.github/               # GitHub issue templates and CI/CD workflows
checklists/            # Feature and task checklists
config/                # Static config files (e.g., event categories)
doc/                   # Documentation assets
prisma/                # Prisma schema and migrations
├── seedData/          # seed scripts
public/                # Static assets (images, icons)
├── groups/            # Group Picture Images
├── images/            # Miscellaneous Images
├── pfps/              # Profile Picture Images
├── trails/            # Trail Picture Images
src/
├── app/               # Next.js route handlers and pages
│   ├── announcements/          # Announcements and Events
│   ├── api/auth/[...nextauth]  # API routes (auth, categories, events, user)
│   ├── auth/                   # Sign in, sign up, sign out
│   ├── groups/                 # Groups
│   ├── hikes/                  # Trails
│   ├── not-authorized/         # Role-based access fallback
│   ├── profile/                # Profiles
│   ├── global.css              # Styles
│   └── page.tsx                # Landing page
├── components/        # Reusable UI components (forms, buttons, cards, navbar, footer, search)
├── lib/               # Auth options, DB actions, validation schemas
├── types/             # TypeScript declarations
├── tests/             # Playwright test files and sessions
.env                   # Environment variables to easier transition to Vercel Database
.env.local             # Local environment variables
README.md              # Project documentation
package.json           # NPM scripts and dependencies
```

### Modifying the System

Developers and contributors should ensure that all CI checks pass before merging pull requests.

#### Contribution Workflow

Typical Development Flow
* Create an Issue Branch
* Implement Changes
* Run `npm run lint` and `npx playwright test`
* Commit and push your branch
* Open a pull request
* Ensure CI passes
* Request review from team members

___
## Community Feedback

We asked 5 members of the UH Community to try to test the Outside Buddies web application on both the user and the dev end. For each community member, we hav split their answer into the categories: 'Things that I liked', 'Things that could be improved'

### UH Community Member 1: (Civil Engineering Major, very little computer experience)

**Things that I liked:**

I liked the style of the website; I also think that the functions make sense for what the app is meant to do.

**Things that could be improved:**

A feature you could consider implementing in the future is a way to see nearby users based on location? That way if someone gets lost or separated from the group, hopefully someone would be able to find them or the person that got lost would be able to find their way back.

### UH Community Member 2: (Computer Science Major, took ICS 314 before)

**Things that I liked:**

I liked the colors and general theme of the website. I think it's interesting and unique.

**Things that could be improved:**

A feature that you could consider implementing in the future is allowing users to attach their different social medias (like Instagram, TikTok, Discord, etc.) to their Profile. That way, other users would have the option to communicate on different platforms, where it could be more convinient, especially if it's a large Group.

### UH Community Member 3: (Mathematics Major, took ICS 314 before)

**Things that I liked:**

I like the logo and the colors, it's quirky. It gives a early 2000s era of internet aesthetic. I also like that the auth has been set up and that typing the url pathways doesnt allow users to access forbidden pages. Overall, I like the concept, I think it's neat.

**Things that could be improved:**

A future feature could be having a search bar algorithm where the "likeliest" search will dropdown from the search bar based on what is the most likely successive letter. Also having back buttons would make the experience a lot better.


### UH Community Member 4: (Mathematics Major, some computer experience)

**Things that I liked:**

I really like the concept and colors. It's nice to have information about the Hikes as well to give people ideas, even if they don't set up a Group within the application. It's nice that if the image link is incorrect, you have a default profile picture and image file that loads up, so that you don't have to just look at a clear error with some text.

**Things that could be improved:**

It would be nice to be able to message different users just within the Profile like a private message.

### UH Community Member 5: (Mathematics Major, little computer experience)

**Things that I liked:**

I overall liked the concept. I think that the website looks really cool. I like that I was able to write a post. I thought that was nice. Also having a Hikes List for people who are new here is a great idea, especially since there are a lot of hikes on Oahu.

**Things that could be improved:**

There could be a discussion feature underneath each hike for users to communicate their tips and tricks. Implementing a map feature for the hikes could be nice too. A friends system would also be a nice touch, where you can friend other profiles.

___
## Development History

### Milestone 1: Mockup development

The goal of [Milestone 1](https://github.com/orgs/outdoor-buddies/projects/1) was to create mockups of each of the pages for our Outdoor Buddies Website. Specifically Announcements(/Events), Hikes, Groups, and Profiles.

### Milestone 2: Data model development

The goal of [Milestone 2](https://github.com/orgs/outdoor-buddies/projects/3) was to implement the data model: for Announcements(/Events), Hikes, and for Groups and Profiles (especially connecting them to a specific User) on the site. We also fixed certain login issues, transferring to the vercel deployment database, and added basic features, such as searching, adding, editing, and deleting functions. Users can add, edit, and delete Groups and Profiles. Admins can add, edit, and delete Announcements(/Events) and Hikes.

### Milestone 3: Final touches

The goal of [Milestone 3](https://github.com/orgs/outdoor-buddies/projects/4) is to clean up the code base, implement features that we were unable to complete in Milestone 2, have some users test our app while also implementing their suggestions, add more entries into our tables, adjust some of the styles, including fonts, colors etc. We added in a dynamic search that can filter based on certain components for both Hikes and Groups. Groups also now has a Forum Page where users can post asking a group some questions or to request to join.

___
## Team

OutdoorBuddies is designed, implemented, and maintained by [Brycen Kano](https://brycenk05.github.io/) and [Kelly Masaki](https://kellym12.github.io/Professional-Portfolio/).  

Our [Team Contract](https://docs.google.com/document/d/11j764LAw7YHbRscZZDggGGVZIzsIFAGyGOxQO0eoB1g/edit?tab=t.0) is viewable here.

Our [Effort Estimation Log](https://docs.google.com/spreadsheets/d/1eeu1O1KRPOSeJ9_-fLJdqsYPwT55wFt2rFn6RpRWpBE/edit?gid=0#gid=0) is viewable here.

Our [Feedback Form](https://docs.google.com/forms/d/1s5giYVxxcc7z6MaEk2tQkjkACl2sGNaz3vUJycFOI5g/edit) for if you would like to give us any feedback.