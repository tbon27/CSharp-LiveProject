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

![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story2/US2-SNIP2.png)

Lastly, I updated the database to store cast and production members. The image below shows a populated database with cast and production members. Note: Some of the data in this image is provided from later stories in the Live Project.

![This is an image](https://github.com/tbon27/CSharp-LiveProject/blob/main/images/story2/US2-SNIP3.png)
