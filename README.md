![MathsBuddy logo](assets/images/logo.png)

# MathsBuddy
MathsBuddy is a website that provides online learning for maths to students who wish to take the Junior Cycle exam.

## Overview

### Who is this app for?
 
MathsBuddy is a website which provides resources for students who will be taking the Junior Cycle exam in Ireland.  These students will be aged between 14 and 16 years old.  MathsBuddy is a website which will be used by students who are in high-risk families and are not entitled to online instruction from the department of education.  
 
### What does it do?
 MathsBuddy hopes to bridge the gap during the current covid-19 crisis by offering an opportunity to solidify maths concepts up to Junior Cycle level.
 
### How does it work
 
MathsBuddy gives access to tutorial videos and past exam questions, broken down by topic, for the Junior Cycle maths exam.

## Screen Mockups

## Features

### Existing Features
- None yet!
 
### Features Left to Implement
1 Site navigation

2 Show videos on each topic

       2.1 Videos stored locally

       2.2 Videos from external sources.  E.g. Youtube, Khan Academy

3 Display past exam papers for each topic   
 
## Design Decisions
### Code Quality
- Correct use of HTML 
    - Use HTML5 Semantic elements
    - Use Horizontal NavBar
- Correct use of CSS 
    - Use Flexbox for page layout
	
### Usability
- Suitability for purpose 
- Ease of use
    - A simple easy-to-use application focusing on reducing the 'cognitive load' on users.  The system is designed so that users do not have to remember large amounts of detail.
- Information Display 

### Layout and Visual Impact
- Responsive Design 
    - "Desktop First" design philosophy
    - FlexBox is used to give responsive layouts
    - Media Queries are used for each different screen size the tool will be used on.
- Performance
- Navigation 
    - Straightforward navigation enabling users to move easily from one part of the site to another.
- Image Treatment 
    - Images are compressed to reduce download times.  [tinypng.com](https://tinypng.com) and [tinyjpg.com](https://tinyjpg.com) were used to compress the  image files.
    - Multiple versions of each image are used, with smaller images used for smaller devices.  This reduces the download times for tablets and especially mobile devices.  The HTML5 <source> element is used and its *srcset* attribute is set to show the smaller image at lower screen widths.  For background images, a media query is used in CSS to set the background image to a smaller image when the screen size falls below a particular size.
- Non-image Content 

### Software Development Process
#### Version Control 
**Git** is used for version control of this project
- Git commit message prefix convention denoting the type of change made in this commit:
    - DOC: Documentation
    - FEAT: Feature
    - FIX: Bugfix
    - STYLE: Changes to CSS
- Git messages will be no longer than 50 characters long.

**GitHub** is used as the central version control repository for this project.

**Cloning versus Forking**
#### Testing 
All testing on the MathsBuddy website will be done manually.
##### **Test scripts**
Test Script 1
- Expected result
- Steps
1. Step 1
2. Step 2
- Actual result
#### Documentation  
- README.md :  Comprehensive overview of the MathsBuddy website detailing how it works, what its features are, the technologies involved and all the design decisions that were made in creating this learning resource.
- [Vision doc](documentation/MathsBuddy-Vision.docx) :  Business needs and feature list.
- WireFrames :  Wireframes for each different layout.
- Site map :  Basic site map with prioritisation and categorisation of each page.

#### Deployment 
- This project is deployed to [Github Pages](Link to follow)

## Technology Used

### Some of the technology used includes:
- [HTML5](https://dev.w3.org/html5/spec-LC/)
    - **HTML5** is used to develop the content of the MathsBuddy website.
- [CSS](https://www.w3.org/Style/CSS/Overview.en.html)
    - **CSS** is used to layout the HTML elements on each page of the MathsBuddy website.
- [FlexBox](https://www.w3.org/TR/css-flexbox-1/)
    - **FlexBox** is used to give the MathsBuddy website a simple, responsive layout.
 
## Contributing

### Getting the code up and running
1. Firstly you will need to clone this repository by running the ```git clone https://github.com/Liz-Conway/MathsBuddy.git``` command
