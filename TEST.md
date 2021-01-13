# Testing
## Table of Contents
[User stories testing](#user-stories-testing)  
[Code Validation](#code-validation)  
[Testing across web browsers](#testing-across-web-browsers)  
[Testing Responsiveness](#testing-responsiveness)  
[Bugs and Problems](#bugs-and-problems)  
***

## User stories testing:	
### First time users:

**1. As a first time user, I want to navigate easily across the website.**  
1. The website has a responsive navigation bar that takes the user to all the other pages. On smaller screens the navigation bar collapses to a hamburger icon.  
2. The home page is an overview of the other pages, in each of the sections there are buttons that lead the user to the respective pages.  
3. At the bottom of each page there is an icon with text that, when clicked, leads to the top of the page.
4. Clicking on the logo takes the user back to the home page.


**2. As a first time user I want to find information about the group and its members, so i can get to know the group better.**  
1. The user can use the navigation bar and click on ‘About Us’ or scroll down to the ‘About Us’ section on the Home page and click on the ‘full biography’ button, which takes them to the ‘About Us’ page.
2. In the footer of each page are links to the social media accounts of the group. 
3. When users click these links, a new tab opens and lead to the respective social media website.

**3. As a first time user I want to hear some of the recordings, to see whether I like the group’s music.**  
1. Users can use the navbar and click on the ‘Our Music’ link or they can scroll down to the ‘Our Music’ section on the Home page and click on the ‘our music’ button. This takes them to the ‘Our Music’ page. 
2. On the ‘Our Music’ page are several audio and video files that the user can listen to and watch.
3. The audio and video files have controls, so the user can play or pause a file. The video files also have a volume control.
4. Two of the social media links in the footer are links to Youtube and Spotify. Here the user can listen to more music and watch more videos.

Returning/regular users:

**4. As a user I want to follow the group, so I stay up to date with the latest news on what they do.**  
1. On the bottom of each page, in the footer, the user can click on the ‘Signup for our newsletter’ button. This will open a modal where the user can subscribe to the newsletter of the group.
2. Submitting an empty form will give a warning for the required fields.
3. Submitting the form with an invalid email address will also give a warning to use a correct email address.
4. When a user submits the form with all the correct, there are no warnings and the modal closes.
5. Each page has links to the social media accounts of the group. Clicking on a link opens a new tab and takes you to the corresponding social media website.

**As a user I want to find information on concerts, so I can see when and where they are.**  
1. Users can use the navbar and click on the ‘Our Shows’ link or they can scroll down to ‘Upcoming Shows’ on the Home page and click the ‘Get Tickets’ button. 
2. This takes them to the ‘Our Shows’ page where the user can find the information about upcoming shows of the group.

**5. As a user I want to be able to buy tickets for their concerts.**  
1. The user can go to the ‘Our Shows’ page (see above) and click on the ‘Buy Tickets’-button to buy tickets for upcoming shows.
2. There they can select the number of tickets they want to buy.

**6. As a user I want the option of buying a song or album.**  

This feature is not implemented and is tagged as a feature left to implement. (see Scope level)

Event planners:

**7. As an event planner I want to learn more about the group and listen to some material, so I can decide whether or not to book the group for an event.**  

See user story test 2 and 3.

**8. As an event planner I want to contact the group (by email or by phone), so I can get more information or book them for an event.**  
1. The Home page has a clear ‘Book Us’ button that takes you to the ‘Contact’ page.
2. A user van also use the navbar and click on the ‘Contact’ link and then on the ‘Book Us’ link to go to the ‘Contact’ page.
3. There they can fill out a form for booking or inquires.
4. When the user submits the form with an invalid email address, a warning appears to use a correct email address.
5. When the form is submitted with all the correct input, there are no warnings and the modal closes.


## Code validation

[W3C Markup Validation Service](https://validator.w3.org/) is used to check for markup validity of the web document.
Running the code through the validator gives:
index.html:
1. Two warnings that the document is not mappable to XML due to two consecutive hyphens.  
The hyphens were added for better legibility, however this clashes with the commenting out syntax. The extra hyphens were removed.

2. Error: The section on line 185 lacks a heading.
Semantics expect a section to have a heading. However this is not meant as a section. Section has been changed to div.
Since this occurs on all pages, this was also changed on the other pages.

3. Error: Five messages that the 'alt' attribute is not allowed on an < a > element.
The alt attributes were removed. Since these were in the footer, these were also removed on the other pages.

aboutus.html:
No errors or warnings are shown.
ourmusic.html:
1. Four errors: a bad value (100%) for 'width' on element iframe. A digit is expected, but a % is used. 
This is done to display the audio file correctly and to keep it responsive.
I've tried to change the value to a digit, but then the width stays fixed and the audio file isn't responsive anymore.
2. Six errors: the 'frameborder' attribute om the 'iframe' element is obsolete. CSS is recommended.
This attribute was provided by the Spotify embed code. I've removed the 'rameborder' attribute and added iframe { border: none; } to style.css.
3. Four errors: the 'allowtransparency' attribute on the 'iframe' element is obsolete. CSS is recommended.
Again, this attribute was provided by the Spotify embed code. I've removed the code, this doesn't visually change the website.   
I've decided to keep it that way and not add CSS.

ourshows.html:
1. Three errors: the value of the 'for' attribure of the 'label' element must be the ID of a non-hidden form control.
I've changed the label to match the ID's.
contact.html:
1. Two errors: bad value for attribute 'type' on element 'input'.
I've accidentally added the same value of the 'for' attribute to the 'type' attribute.
2. Errors: a bad value (100%) for 'width' and 'height' on element iframe. A digit is expected, but a % is used. 
Again, this is done to display the audio file correctly and to keep it responsive (see above).

After these changes, except for the errors that I've left in deliberately in [ourmusic.html](https://github.com/chizzletaz/MilestoneProject1/blob/master/assets/img/extra/HTML_errors_ourmusic.png) and [contact.html](https://github.com/chizzletaz/MilestoneProject1/blob/master/assets/img/extra/HTML_errors_contact.png), there were [no errors](https://github.com/chizzletaz/MilestoneProject1/blob/master/assets/img/extra/HTML_validation.png) or warnings found.

[W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/) is used to check the CSS of the web document.
Running the code throught the validator by direct input gives [no errors](https://github.com/chizzletaz/MilestoneProject1/blob/master/assets/img/extra/CSS_validation.png).


## Testing across webbrowsers:  
I've tested the site on Safari, Chrome and Mozilla Firefox.  
No big issues arrose. The only small changes between websites it that they sometimes add their own styling. 
For instance on Safari, if you click/select a dropdown-link, the browser adds an extra blue border.

## Testing Responsiveness:
I've tested the site using [Chrome Dev Tools](https://github.com/chizzletaz/MilestoneProject1/blob/master/assets/img/extra/responsiveness_chrome_dev_tools.png) and [Responsinator](https://www.responsinator.com/)
There were no great issues for each of the mobiles and tablets available in Chrome Dev Tools.
On the iPhone5/SE the caroussel-indicators are at the bottom of the button, but the button can still be clicked.
On the galaxy fold (viewportwidth = 280px) the CTA is moved into the heading below. And some of the headings and the social media icons are wrapped to the line below.

I also checked each responsive breakpoint stated by [Bootstrap](https://getbootstrap.com/docs/4.3/layout/overview/#responsive-breakpoints).
At the lowest breakpoint (576px) one of the social media icons moves to the next line.
I've resolved this by adjusting the col-sm size for both:  
footers-signup: col-sm-6 -> col-sm-5. footer-social-links: col-sm-6 -> col-sm-7.

## Bugs and Problems

I have started testing with Lighthouse.  
Lighthouse is used to test issues referring to performance, accessibility, best practice and SEO (Search Engine Optimisation).  

I’ve tested every page on mobile and desktop device. Scores of 90 or more are flagged green by Lighthouse, so I’ve only looked at the scores below 90 and tried to address these issues.  

However, Lighthouse sometimes gives different values if you check the page without making any change to it. 
I also didn’t understand or was able to change some of the issues indicated by Lighthouse.  

I asked a tutor at CI about Lighthouse and they said that Lighthouse isn’t required. It’s not covered in the course and can be pretty massive in scope. So I’ve decided to drop this section from the testing part. 

However, I already made some changes to my code, which I left in.
Some of the changes are:

- Reduce the size of images I've used. 
- Adding ‘rel=“noopener”’ to all links that open in a new tab, because links to cross-origin destinations are unsafe.
- Adding a <meta> element with a descriptive link inside the <head> element of each page.

All other bugs and probems that i've encountered are already addressed in the previous sections.



