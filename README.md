# C Sharp - Live Project

## Introduction
To cap off my studies with The Tech Academy, I spent the last two weeks of my studies in a live Internship which entailed working on an MVC web application in C# for a theatre company in Portland. The website was divided into sections that the theatre disired being: rentals, production, and a blog section. During this project I worked on a team with fellow students to create functionalities and overall improvements to the production section of the site. Our team comminucated through Discord, and used Azure DevOps for project management. Throughout the course of the project I experienced work in the front end and the back end to complete my user stories and continue the progress of developing our application. This two-week Internship provided an opportunity to get a closer look at project planning and development, and how to collaborate with a team regardless of the technology being used in a given project.

## Quick Navigation
- [User Story #1: Create and Style Register and Log in buttons](https://github.com/tbon27/CSharp-LiveProject#user-story-1)
- [User Story #2: Create an Entity Model for TheatreMember class to use with Database](https://github.com/tbon27/CSharp-LiveProject#user-story-2)
- [User Story #3: Style the Create and Edit Buttons](https://github.com/tbon27/CSharp-LiveProject#user-story-3)
- [User Story #4: Add Photo Storage and Retrieval functionality to CRUD pages](https://github.com/tbon27/CSharp-LiveProject#user-story-4)
- [User Story #5: Style the Index View with Bootstrap Cards](https://github.com/tbon27/CSharp-LiveProject#user-story-5)
- [Sprint Retrospective](https://github.com/tbon27/CSharp-LiveProject#retrospective)
## Overview

### User Story #1

My first user story of the Live Project was to redesign the Register and Log in buttons to function more like actual buttons. 
This story required the following for acceptance: 
- When the cursor hovers over a button, there should be no link underline applied to the text. 
- The entirety of the button should be clickable and direct user to respective page. 
- Buttons will maintain the color scheme and theme of the project.

The following is my solution for my first user story:
![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story1/US1-SNIP.png)

The image below shows the button features, specifically the on hover effect.
![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story1/US1-SS.png)

### User Story #2

My second user story required the creation of an entity model for the TheatreMember class, so that cast and other production members could be saved to the database.

First, I created the TheatreMember class model, and added an enum Position for the MainRole property.

![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story2/US2-SNIP.png)

Next, I created the controller and scaffolded the CRUD pages for TheatreMember.

![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story2/US2-SNIP2a.png)

Lastly, I updated the database to store cast and production members. The image below shows a populated database with cast and production members. Note: Some of the data in this image is provided from later stories in the Live Project.

![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story2/US2-SNIP3a.png)

### User Story #3

The third user story was to style the Create and Edit pages, including a hover effect and on click effects for input boxes. The images below are a comparison of the Edit page before and after. Acceptance criteria included: a single line header, buttons styled and unique between eachother, include placeholders for all input fields, and keep project styling consistent for all features.

Before:

![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story3/US3-SS2b.png)

After:

![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story3/US3-SS1b.png)

### User Story #4

For my fourth user story I added photo storage and retrieval functionality to the TheatreMember model. This allows users to upload files from their own file system; then in the controller the uploaded image is converted into a byte array (byte[]) and stored in the database. The byte[] representing the photo is able to be retrieved from the database and converted back into an image where it can be displayed on View.

First, I created a method in the TheatreMember Controller that takes in the uploaded photo and converts that photo into a byte[].

![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story4/US4-SNIP1a.png)

Next, I added new file input fields to the Create and Edit Views, so the images could be uploaded to the Controller. 

![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story4/US4-SS-CREATE.png)
![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story4/US4-SNIP4.png)

Then I used the method in the Create and Edit Controller methods to convert the uploaded image to a byte[] and assign the byte[] to the database.

![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story4/US4-SNIP-CREATE.png)
![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story4/US4-SNIP-EDIT.png)

I also created two methods that enable us to retrieve the stored byte[] from the database using TheatreMemberID to return the file of the converted photo.

![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story4/US4-othermethods.png)

Lastly, I used my method to display the photos of TheatreMember on all CRUD pages. The following are examples of the method applied to Create and Edit views.

![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story4/US4-DisplayCreate.png)
![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story4/US4-DisplayEdit.png)

### User Story #5

For my last user story of the two-week Live Project, I added Bootstrap cards to the Index View to display the Theatre Members sorted by the Production they are acting in, along with other styling upgrades to the Index including: styling the create button, creating an on-hover overlay effect on each card utilizing Font Awesome to create the edit and delete buttons that appear on the effect, and that each card is clickable and directs the user to the Theatre Member's Details page.

The following applies Bootstrap cards and displays the Theater Member image and name sorted by Production to the Index View. Create, Edit, and Delete buttons are placed and styled, while Edit and Delete buttons use CSS to appear on hover. The card is also clickable and directs the user to the Theare Memebers Details page. 
![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story5/US5-SNIP1a.png)
![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story5/US5-SNIP2a.png)
![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story5/US5-SNIP3a.png)

The final result of the Index page.
![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story5/US5-SSb.png)

This image shows the Edit and Delete buttons appearing on hover with respective styles, and image darkens slightly on hover.
![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story5/US5-SSc.png)

### Retrospective

This two-week sprint has provided working experience on an MVC web application with a team. Many of the skills learned are translatable to my future projects and collaborations.

Other notable takeaways from this project: 
- Proper Version Control practices
- Experience with Azure DevOps
- Experience utilizing AGILE/SCRUM methodologies and frameworks
