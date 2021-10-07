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

## Features

### Existing Features
1 Site navigation

2 Show videos on each topic

       2.1 Videos stored locally

       2.2 Videos from external sources.  E.g. Youtube, Khan Academy

3 Display past exam papers for each topic   
 
### Features to Implement in the future
- Send the 'Contact Us' form data to a backend server.
- Use a collapsible navbar in mobile versions of the site.
- Add more maths topics!

## UX

### Personas

**Emily Reilly**

![Emily](documentation/ux/emily-persona.png)

![Daniel](documentation/ux/daniel-reily-persona.png)

### Student Journey Maps

![Emily Journey Map](documentation/ux/emily-student-journey-map.png)

![Daniel Journey Map](documentation/ux/daniel-student-journey-map.png)

### User Flow

![User Flow](documentation/ux/mathsbuddy-userflow.png)


### Site Map

![MathsBuddy Site Map](documentation/ux/mathsbuddy-sitemap.png)


## Design Decisions
### Code Quality
- Correct use of HTML 
    - Use HTML5 Semantic elements
    - Use Horizontal NavBar
- Correct use of CSS 
    - Use Flexbox for page layout
	
### Usability
- Suitability for purpose
    - MathsBuddy provides resources that cover maths topics for the Junior Cycle.
    - MathsBuddy provides access to past exam questions from the maths Junior Cycle exams.
    - MathsBuddy provides resources and exam questions for both Paper 1 and Paper 2 on the Junior Cycle exam.
- Ease of use
    - A simple easy-to-use application focusing on reducing the 'cognitive load' on users.  The system is designed so that users do not have to remember large amounts of detail.
- Information Display 
    - There is a main navigation bar on every page.  This allows navigation to all the main pages (Home, Maths, About and Contact Us) from everywhere on the site.
    - For the Topics pages, as well as the main navigation bar, there is a secondary (breadcrumb) navigation that allows the student to (i) go back to the parent page (Maths), or (ii) go to the previous and next topic pages.
    - For the Exam Question pages, as well as the main navigation bar, there is a secondary (breadcrumb) navigation that allows the student to (i) go back to either of the parent pages (Maths or the topic page), or (ii) go to the previous and next exam question pages.

### Layout and Visual Impact
- Responsive Design 
    - "Desktop First" design philosophy
    - FlexBox is used to give responsive layouts
    - Media Queries are used for each different screen size the tool will be used on.
- Navigation 
    - Straightforward navigation enabling users to move easily from one part of the site to another.
    - When a student ventures onto a page which is not navigable from the main navigation bar, a secondary breadcrumb navigation bar is engaged, which allows the student to navigate all the way back to a main page.
    - The secondary breadcrumb navigation bar also allows the student to go to the next and previous pages at the same level.  I.E.  If the student is on the Number types *topic* page, he can go to the Algebra *topic* page or the Trigonometry *topic* page.  Also, if the student is on the Number types *exam questions* page, he can go to the Algebra *exam questions* page or the Trigonometry *exam questions* page.
- Image Treatment 
    - Images are compressed to reduce download times.  [tinypng.com](https://tinypng.com) and [tinyjpg.com](https://tinyjpg.com) were used to compress the  image files.
    - Multiple versions of each image are used, with smaller images used for smaller devices.  This reduces the download times for tablets and especially mobile devices.  The HTML5 <source> element is used and its *srcset* attribute is set to show the smaller image at lower screen widths.  For background images, a media query is used in CSS to set the background image to a smaller image when the screen size falls below a particular size.
- Video Treatment 
    - All videos are made available in mp4, webm and ogg formats.  Videos were converted to webm format using [wem.to](https://webm.to/video-webm), and to ogg format using [onlineconverter.com](https://www.onlineconverter.com/video-to-ogg). The HTML5 *source* element is used and its *src* attribute is set to point to the correct version. Its *type* attribute is set to tell the browser which format this src is pointing to.
    - Text is set within the *video* element. This text will be displayed if the student's browser does not support the video element.
    - The video on the home page is set to play automatically and to loop.  This is because the video is intended as a background video, its sound is muted and the colours have a low saturation so they will not distract the user.
    - All other videos are not autoplay and allow the user to control their playback.
    - Some videos are served from the MathsBuddy site.
    - Videos served from external sites are displayed within an iframe.    
- Non-image/video treatment

####Wireframes

**Home Page**
![Home page](documentation/wireframes/wireframe-main-page.png)
**Maths Page**
![Maths page](documentation/wireframes/wireframe-maths.png)
**About Page**
![About page](documentation/wireframes/wireframe-about.png)
**Contact Us Page**
![Contact Us page](documentation/wireframes/wireframe-contact-us.png)
**Topic Video Page**
![Topic page](documentation/wireframes/wireframe-maths-number-types.png)
**Topic Exam Questions Page**
![Exam question page](documentation/wireframes/wireframe-exam-questions-number-types.png)

####Screen Mockups

### Software Development Process
#### Version Control 
**Git** is used for version control of this project
- Git commit message prefix convention denoting the type of change made in this commit:
    - DOC: Documentation
    - FEAT: Feature
    - FIX: Bugfix
    - STYLE: Changes to CSS
    - ARIA: Changes to improve accessibility for the MathsBuddy website.
- Git messages will be no longer than 50 characters long.

**GitHub** is used as the central version control repository for this project.

#### Testing 
All testing on the MathsBuddy website will be done manually.
##### **Test scripts**
Test Script 1
- Expected result
- Steps
1. Step 1
2. Step 2
- Actual result

#### Known Bugs
Number types exam questions says 16 questions but it only has 4.
Image on Trigonometry topic page (5.1KB) does not have a smaller image to display on smaller screens

#### Validation
CSS was validated using [W3C CSS validator](https://jigsaw.w3.org/css-validator/validator)
![CSS Validated](documentation/validation/css-validator.png)

HTML was validated on all pages using [W3C HTML validator](https://validator.w3.org/)

Home Page

![Home page validated](documentation/validation/html-validator-home.png)

Maths Page

![Maths page validated](documentation/validation/html-validator-maths.png)

About Page

![About page validated](documentation/validation/html-validator-about.png)

Contact Us Page

![Contact page validated](documentation/validation/html-validator-contact-us.png)

Number Types video page

![Number Types page validated](documentation/validation/html-validator-number-types.png)

Algebra video Page

![Algebra page validated](documentation/validation/html-validator-algebra.png)

Co-ordinate Geometry video Page

![Co-ordinate Geometry page validated](documentation/validation/html-validator-coordinate-geometry.png)

Trigonometry video Page

![Trigonometry page validated](documentation/validation/html-validator-trigonometry.png)

Number Types exam questions Page

![Number Types exam questions page validated](documentation/validation/html-validator-number-types-exam-q.png)

Algebra exam questions Page

![Algebra exam questions page validated](documentation/validation/html-validator-algebra-exam-q.png)

Co-ordinate Geometry exam questions Page

![Co-ordinate Geometry exam questions page validated](documentation/validation/html-validator-coordinate-geometry-exam-q.png)

Trigonometry exam questions Page

![Trigonometry exam questions page validated](documentation/validation/html-validator-trigonometry-exam-q.png)

404 Error page

![404 error page validated](documentation/validation/html-validator-404.png)

#### Documentation  
- README.md :  Comprehensive overview of the MathsBuddy website detailing how it works, what its features are, the technologies involved and all the design decisions that were made in creating this learning resource.
- [Vision doc](documentation/MathsBuddy-Vision.docx) :  Business needs and feature list.

- Site map :  Basic site map with prioritisation and categorisation of each page.

#### Deployment 
- This project is deployed to [Github Pages](https://liz-conway.github.io/MathsBuddy/)

## Technology Used

### Some of the technology used includes:
- [HTML5](https://dev.w3.org/html5/spec-LC/)
    - **HTML5** is used to develop the content of the MathsBuddy website.
- [CSS](https://www.w3.org/Style/CSS/Overview.en.html)
    - **CSS** is used to layout the HTML elements on each page of the MathsBuddy website.
- [FlexBox](https://www.w3.org/TR/css-flexbox-1/)
    - **FlexBox** is used to give the MathsBuddy website a simple, responsive layout.
 
## Contributing

### Clone
1. Firstly you will need to clone this repository by running the ```git clone https://github.com/Liz-Conway/MathsBuddy.git``` command
2. After you've that you'll need to make sure that you have a package manager such as **npm**  installed
  1. You can get **npm** by installing Node from [here](https://nodejs.org/en/)
3. Make sure that you have **live-server** installed. You can install this by running the following: ```npm install -g live-server``` .  This also may require sudo on Mac/Linux
4. Once **live-server** is installed run ```live-server``` in the root directory (the one where index.html is).
5. The project will now run on [localhost](http://127.0.0.1:8080)
6. Make changes to the code and if you think it belongs in here then just submit a pull request.

### Fork
1. Log into [Github](https://github.com/)
2. Search for **MathsBuddy** and choose to go to ```Liz-Conway/MathsBuddy```.
3. Click on the *Fork* button on the top right hand side of the screen.
4. This will make a copy of **MathsBuddy** in your github account.
5. In your version of MathsBuddy click on the ```code``` button and copy the clone text.
6. Then, you will need to clone this repository by pasting the command you just copied into a terminal window on your computer and running it.  This will create a copy of MathsBuddy from your github account on your computer.
7. After you've that you'll need to make sure that you have a package manager such as **npm**  installed
  1. You can get **npm** by installing Node from [here](https://nodejs.org/en/)
8. Make sure that you have **live-server** installed. You can install this by running the following: ```npm install -g live-server```  This also may require sudo on Mac/Linux
9. Once **live-server** is installed run ```live-server``` in the root directory (the one where index.html is).
10. The project will now run on [localhost](http://127.0.0.1:8080)
11. Make changes to the code and run ```git push``` to save those changes to your github account.


### Cloning versus Forking

## Credits
