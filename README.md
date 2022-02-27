# C Sharp - Live Project

## Introduction
This is where the intro goes.

## Overview

### User Story #1

My first user story of the Live Project was to redesign the "Register" and "Log in" buttons to function more like actual buttons. 
This story required the following for acceptance: 
- When the cursor hovers over a button, there should be no link underline applied to the text. 
- The entirety of the button should be clickable and direct user to respective page. 
- Buttons will maintain the color scheme and theme of the project.

The following is my solution for my first user story:
![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story1/US1-SNIP.png)
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


