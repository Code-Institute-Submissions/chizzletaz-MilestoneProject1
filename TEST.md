# Testing
## User stories testing:	
### First time users:

**1. As a first time user, I want to navigate easily across the website.**  
- *Navigation:*  
    1. On desktop: adjust screen width to see if the navigation menu collapses into a hamburger icon.  
    2. Click on all the navigation links to check if it takes you to the correct page.  
    3. Click on all the buttons on the home page to check if they take you to the correct page.


**2. As a first time user I want to find information about the group and its members, so i can get to know the group better.**  
- *About Us:*  
    1. Scroll down to the ‘About Us’ section on the Home page and click on the ‘here’ button to check if it takes you to the ‘About Us’ page.  
    2. Use the navbar and click on to go to the ‘About Us’ link and check if it takes you to the ‘About Us’ page. 
    3. Scroll down to the footer and click on each of the links to the social media accounts of the group and check if they open up in a new tab and take you to the correct social media website.

**3. As a first time user I want to hear some of the recordings, to see whether I like the group’s music.**  
- *Our Music:*  
    1. Scroll down to the ‘Our Music’ section on the Home page and click on the ‘here’ button to check if it takes you to the ‘Our Music’ page.   
    2. Use the navbar and click on the ‘Our Music’ link and check if it takes you to the ‘Our Music’ page.  

- *embedded audio and video*:
    1. Check each audio and video file if they are playing.  
    2. Check if the controls are responding (play/pause).  
    3. Scroll down to the footer and check if the Youtube and Spotify icon open a new tab and take you to YouTube and Spotify respectively.

### Returning/regular users:

**4. As a user I want to follow the group, so I stay up to date with the latest news on what they do.**
- *Subscribe to newsletter:*
    1. Scroll down to the footer. 
    2. Click on the ‘Signup for our newsletter’ button. This will open a modal where the user can subscribe to the newsletter of the group.  
    3. Submit the empty form and confirm a warning appears for required fields.
    4. Submit the form with an invalid email address and confirm a warning appears to use a correct email address.
    5. Submit the form with all the correct input and check that there are no warnings and the modal closes.
- *Social media icons and links:*
    1. Click on each of the links to the social media accounts of the group and check if they open up in a new tab and take you to the correct social media website.

**As a user I want to find information on concerts, so I can see when and where they are.**
- *Our Shows:*
    1. croll down to ‘Upcoming Shows’ on the Home page and click the ‘Get Tickets’ button to check if it takes you to the ‘Our Shows’ page. 
    2. Use the navbar and click on the ‘Our Shows’ link and check if it brings you to the ‘Our Shows’ page.

**5. As a user I want to be able to buy tickets for their concerts.**
- *Our shows:*
    1. Go to the ‘Our Shows’ page (see above). 
- *Buy tickets modal and form:*
    1. Click on the ‘Buy Tickets’-button to check if the modal for buy tickets for upcoming shows pops up.
    2. Select a number of tickets and check if the select box works.

**6. As a user I want the option of buying a song or album.**  
This feature is not implemented and is tagged as a feature left to implement. (see Scope level)

### Event planners:

**7. As an event planner I want to learn more about the group and listen to some material, so I can decide whether or not to book the group for an event.**  
See user story test 2 and 3.

**8. As an event planner I want to contact the group (by email or by phone), so I can get more information or book them for an event.**  
- *Book Us button:*  
    1. On the Home page click on the ‘Book Us’ button to check if it takes you to the ‘Contact’ page.
- *Contact page:*
    1. Use the navbar and click on the ‘Contact’ link and then on the ‘Book Us’ link and check if it takes you to the ‘Book Us’ section on the ‘Contact’ page.
- *Book us form:*
    1. Submit the empty form and confirm a warning appears for required fields.
    2. Submit the form with an invalid email address and confirm a warning appears to use a correct email address.
    3. Submit the form with all the correct input and check that there are no warnings and the modal closes.

## Testing responsiveness:

### Code validation

[W3C Markup Validation Service](https://validator.w3.org/) is used to check for markup validity of the web document, so to check that there are no errors in the HTML files.
Running the code through the validation gives:
index.html: 
1. Warning for an empty heading.  
This was done to keep the height of the header the same for responsivenes, however that problem was solved in a later stage, so the heading can be removed.

2. Two warnings that the document is not mappable to XML due to two consecutive hyphens.  
The hyphens were added for better legibility, however this clashes with the commenting out syntax. The extra hyphens were removed.

3. Error: The section on line 185 lacks a heading.
Semantics expect a section to have a heading. However this is not meant as a section. Section has been changed to div.
Since this occurs on all pages, this was also changed on the other pages.

4. Error: Five messages that the alt attribute is not allowed on an < a > element.
The alt attributes were removed. Since these were in the footer, these were also removed on the other pages.

aboutus.html:
No erors or warning are shown.
ourmusic.html:
1. Error: a bad value (100%) for width on element iframe. A digit is expected, but a % is used. 
This is done to display the audio file correctly and to keep it responsive.
I've tried to change the value to a digit, but then the width stays fixed and the audio file isn't responsive anymore.
2. Error: the frameborder attribute om the iframe element is absolete. CSS is recommended.
This attribute was provided by the Spotify embed code. I've removed the frameborder attribute and add iframe { border: none; } to style.css.
3. Error


ourshows.html:

contact.html:
After these changes no errors or warnings were found.


goal: circle border around social media icons:
.list-inline-item {
    background-color: #6c757d;
    border: 1px solid black;
    border-radius: 50%;
    height: 40px;
    width: 40px;
    padding: 7px:
    text-align: center;
issue: the icons aren't centered: ![uncentered icons](assets/img/test/icon border 1.png)
trials: put text align after border-radius: ![uncentered icons](assets/img/test/icon border 2.png)
so horizontally centered.
for vertically centered: 

solution: .list-inline-item {
    background-color: #6c757d;
    border: 1px solid #fff;
    border-radius: 50%;
    text-align: center;
    height: 40px;
    width: 40px;
    padding: 7px;
}
---------------------
goal: position footer elements to the side till viewport sm. 
below sm position footer elements on top of each other.
.list-inline {
    float: right;
    padding: 50px;
}

.footer-signup{
    float: left;
    padding: 50px;
}
issue: the elements don't wrap nicely below viewport sm. 
trial: use float-sm-right/left and remove float from  (in style.css)
on inspecting the padding is too large below 760px.
trial: change padding (of list-inline and footer-signup) to 50px auto.
Padding auto is no valid value.
solution: use margin in stead of padding, so: margin: 50px auto.
------------------

issue: the card heigths aren't equal length. 
trial: according to bootstrap you should add h-100 to the card.
This solves the equal length, but the cards are now outside of the container.
Solution: adjust text so that each card has the same amount of text-lines.
-----------------
issue: the back to top button is in the footer area. It needs to be above the footer.
trial: remove "float: right" -> the button is above the footer area, but on the left side of the page.
solution: use "margin-left: auto".
------------------
issue: I can't get the div with the text about the member next to the div with the image of the member.
solution: I forgot to add another row to make the div's sit next to each other.
-----------------
issue: after adding video with bootstrap iframe to ourmusic.html, the video takes up the whole page.
trial: wrap the video in a <div class='container> -> adjusts to max width of the container.
solution: according to c kuijjer (on https://stackoverflow.com/questions/28124214/how-to-reduce-html-video-player-size-in-bootstrap)
you can add a div and set the width or you can wrap the iframe in a bootstrap-grid. Setting a div with width looses the 
responsiveness. So I choose the bootstrap-grid.

issue2: the video isn't centered.
solution: add 2 empty columns on either side of the video-column.
-----------------
issue: the text is centered, but I want it aligned to the right. Aligned with the left side of the video.
solution: add the same bootstrap-grid to the audio and text div's.
----------------
issue: when loading ourmusic.html, the video starts playing automatically.
solution: replace iframe tag with video tag.
----------------
issue: I added a border when hover over the navlinks. 
.nav-item a:hover {
  border: 2px solid #b8860b;
}
However the navlinks and navbottom-border move when hovering, because of the added border.
solution: use hvr-reveal from hover.css. 
----------------
issue: on index.html, the carousel-text isn't responsive.
solution: I accidentally deleted the 'carousel-caption'-class. 
----------------
Issue: I want to change the color of the carousel-indicators.
trial: change the color in style-css. This doesn't work.
solution: according to Chris Gunawardena (on https://stackoverflow.com/questions/46249541/change-arrow-colors-in-bootstraps-carousel) you can use this code:
.carousel-control-next,
.carousel-control-prev,
.carousel-indicators /*, .carousel-indicators */ {
    filter: invert(100%);
}
----------------
