# **B-sharp - a professional Vocal Group**
### *Code Institute Milestone Project 1* 

This project is a frontend website for the fictitious vocal group “B-sharp”.  
The main focus for the website is to get people to buy tickets for their concerts and to book the group for events.  
 
The website provides information on upcoming concerts, on the group and its members and has some media samples. It also has the option buy tickets or to book the group for events.

A live version of this website can be viewed [here](https://chizzletaz.github.io/MilestoneProject1/)   
&nbsp;  


***

# **User Experience (UX)**

## **Strategic level**  
The target audience for this website is:
- People who want to buy tickets for the concerts
- Event planners who want to book the group 
- First time/occasional users looking for more information about the group


### **User stories:**	
**First time users:**

- As a first time user, I want to navigate easily across the website.
- As a first time user, I want to find information about the group and its members, so i can get to know the group better.
- As a first time user, I want to hear some of the recordings, to see whether I like the group’s music.

**Returning/regular users:**

- As a user, I want to follow the group, so I stay up to date with the latest news on what they do.
- As a user, I want to find information on concerts, so I can see when and where they are.
- As a user, I want to be able to buy tickets for their concerts.
- As a user, I want the option of buying a song or album.

**Event planners:**

- As an event planner, I want to learn more about the group and listen to some material, so I can decide whether or not to book the group for an event.
- As an event planner, I want to contact the group (by email or by phone), so I can get more information or book them for an event.


### **Owner goals:**


- As the owners we want users to buy tickets to our concerts.
- As the owners we want people to book us.
- As the owners we want to provide information on our group and its members, so first time visitors/event planners can get to know us.
- As the owners we want to provide media samples, so people can get to know us and/or buy our music.
- We want our social links displayed, so people can follow us and we can generate a fanbase.
- As the owners we want to give updates on what we’re doing, so we stay connected with our followers.  
&nbsp;  


## **Scope level**

Combining the user needs and owner goals gives the following requirements with their respective importance and viability/feasibility displayed in a trade-off equation:

|					| importance  | viability/feasibility
| --- | :---: | :---: |
|a. provide information about the group | 4	| 5
|b. provide information about concerts	| 5	| 5
|c. option to buy tickets online | 5 |3
|d. option to book the group	| 5	| 4	
|e. providing media samples		| 4	| 3
|f. social media promotion		| 3	| 4	
|g. provide contact information		| 5	| 5
|h. provide newsletter subscription	|4		|3
|i. option to buy a song or album	|3		|1

This means that the option to buy a song or album is not implemented now. This will be a feature left to implement. 
&nbsp;

## **Structure level**

Using Interaction Design and Information Design I made the following decisions:  

I want to keep the website consistent by keeping the same page structure along all pages. This enhances the user’s single-use-learning:

- I kept the header and footer the same on each page.
- I styled the button elements the same way.

I want the website to be easy to navigate:
- A responsive navigation bar at the top. 
- The logo at the top is also the link to the home page.
- On the homepage: besides the navigation-links in the navigation-bar, you can get to the other pages by clicking directly on the repective buttons for more information. E.g. at the 'about us'-section on the main page there is a button that leads to the page that has more information on the group and its members.

I want the information to be easily visible:
- I use visual aids like icons, matching colours and images.
- I've used a alternating backgroundcolors to indicate a new section on the page.
- I'm not giving too much information at once. 

I want the user to get feedback during their visit:
- The user get’s a visual feedback during certain actions (e.g. focussing on, clicking on, hovering over buttons and links).
- The user get's a feedback when an error as occured, like an image that can't be displayed.

I’ve based the content requirements on the most likely path a first time user or event planner would take (navigation flow). That is: get to know more about the group (*About Us*) and their music (*Our Music*) and then get tickets for a show or book the group.
Therefore the order in which the websites (and links) are presented is: 
**Home - About us - Our Music - Our Shows - Contact (dropdown menu with Book us)**  
Taking the owner goals into account as well, I’ve opted for the 'Book Us' and 'Upcoming Shows'-section to be displayed first on the main page to ‘seduce’ the first time user/event planner into wanting more information. 
&nbsp;  

## **Skeleton level**
As mentioned above, the website will have 5 pages:  
Home, About us, Our Music, Our Shows and Contact.

**Home**  
has a hero image with a CTA-button to book the group. Below that there is a short overview of all the other webpages with links to the respective pages (where more information can be found).  
**About Us**  
has a section about the group itself and a section about the members:  
**Our Music**  
has some audio- and video-links of music that the group has performed.  
**Our Shows**  
has information on the upcoming shows the group has.  
**Contact**  
has a a contact form for booking or inquiries. Below there is a section with general contact information.
 

**Wireframes:**

link to [wireframes](https://github.com/chizzletaz/MilestoneProject1/blob/master/assets/documents/Wireframes%20MSP1.pdf)  

## **Surface level**
**Colors**  
In order to get a calm, neat and stylish look, I've decided to keep the colours to black, grey and white with an accent-colour of #b8860b (an orange shade).   
![colors used](assets/img/extra/color-codes.png)

**Fonts**  
For the logo I've chosen the 'Architects Daughter' typeface, because it is a handwritten typeface. This gives a more unique feeling to the logo.  
Also using text and font for the logo is an easier way to create the logo.

In order to keep the overall style and feeling of the site calm, I decided to mainly use one type of font: the Open Sans. This typeface is a sans-serif font and has an open feeling and is optimized for legibility across print, web, and mobile interfaces.  
To give some sort of variety to the text, I've use Open Sans Condensed for the headers.  

For the small text I've used 'Crimson text', a serif font.

# **Features**

**Existing Features:** 

- **Responsiveness** on all viewports, from mobile, to tablet to desktop.

- A **navigation bar** which allows users to easily navigate the website. 
On mobile screens it collapses into a ‘burger icon’ with dropdown menu to reduce taking up too much real estate.
- **Google maps** to provide the user with a location of the group. 

**Call To Action-buttons**   
- A CTA which allow users to subscribe to the newsletter of Be-Sharp.   
- A CTA which allow users to book the group.

**Modals**   
- A modal for a signup-form in the footer, which allows the user to sign up to the email-newsletter of the group.  
- A modal to buy tickets for upcoming shows.

**Icons**  
- Social media icons that link to the different social media profiles of the group. For desktop: if the user hovers over the icon, the background changes to the logo-color of the social media.  
- Icons as a visual aid for the different headings/navigation-links.

**Embedded audio/video links**  
- Embedded audio-files from Spotify for users to listen to.  
- Embedded video-files from Youtube for users to watch.

**Forms**   
- A form that allows users to get in contact with the group for booking or information, by leaving their name and email address and the reason for contacting.   
- A form that allows the user to sign up to the email newsletter of the group by leaving their name and email address. 
	 

## **Features left to implement**

- A Search bar for users to search information more quickly.  
- The option to buy a song or album.  
- A blog.  
- The option to pay directly.  
- functional buttons/forms, pending on learning Javascript.


## **Technologies used**

**languages used**  
- [HTML5](https://en.wikipedia.org/wiki/HTML) for markup  
- [CSS](https://en.wikipedia.org/wiki/CSS) for styling

**Frameworks, libraries and programmes used**   
- [Bootstrap 4.5.3](https://getbootstrap.com/) was used for precoded code-snippets, like navigation bar, modals, carousel and to help with the responsiveness of the website.  
- [Balsamiq](https://balsamiq.com/) for making the wireframes.  	
- [Git](https://git-scm.com/) was used version control.  
- [GitHub](https://github.com/) for storing and deploying the website.  
- [GitPod](https://www.gitpod.io/) for coding (IDE) the website.  
- [Atom](https://atom.io/) for trying out code (IDE), due to limited usage time on gitpod.
- [Google fonts](https://fonts.google.com/) for the fonts used in the website.  
- [Font Awesome](https://fontawesome.com/) for the icons used on the website.  
- [Hover.css](https://ianlunn.github.io/Hover/) was used for the hover effect on the navigation-links.  
- [Chrome Developer Tools](https://developers.google.com/web/tools/chrome-devtools)
was used to debug and checking/testing the website.  

## **Testing** 

## **Deployment**

To deploy this website to GitHub, I followed the these steps:

1. Go to GitHub.com and on the left side click on the repository:chizzletaz/MilestoneProject1.
2. In the repository click on the ‘Settings’-tab at the top.
3. Scroll down to ‘GitHub Pages’.
4. Under ‘Source’ you see the word ‘None’ with a dropdown menu: select ‘master branch’.
5. Click ‘Save’, this will give you a URL of the website (see above ‘Source’).

Local Clone:
1. Go to GitHub.com and on the left side click on the repository.
2. Click on the ‘Code’ button.
3. To clone using HTTPS, copy the link that is displayed.
4. Open a terminal in your preferred IDE (e.g. Atom)
5. Use  the ‘git clone’ command and add the link that you copied in step 3.  For Atom: Toggle command palette (cmd-shift-p (macOS) or shift-p (Linux/Windows) and search ‘git clone’: Add the link and 
6. A clone will be created locally.

For more info on how to clone a repository check [here](https://docs.github.com/en/free-pro-team@latest/github/creating-cloning-and-archiving-repositories/cloning-a-repository)
## **Credits**
### Code
Changing the color of the carousel-indicators:
[by Chris Gunawardena](https://stackoverflow.com/questions/46249541/change-arrow-colors-in-bootstraps-carousel) 

Creating the [dark/light-overlay](https://www.codegrepper.com/code-examples/css/how+to+make+dark+overlay+css) for carousel and hero-image

How to [embed spotify audio](https://developer.spotify.com/documentation/widgets/generate/embed/)

How to control the size of an embedded video [by ckuijjer](https://stackoverflow.com/questions/28124214/how-to-reduce-html-video-player-size-in-bootstrap)

Hover.css for the border of the navigation links on hover by [Ian Lunn](https://ianlunn.github.io/Hover/)

How to [embed Google maps](https://blog.duda.co/responsive-google-maps-for-your-website)


### Content
All content is written by myself.

### Media
**Images**  
*Portrait images*  
- portrait1 - Photo by Taylor Deas-Melesh on Unsplash  
- portrait2 - Photo by Kreated Media on Unsplash  
- Portrait3 - Photo by Payton Tuttle on Unsplash  
- portrait4 - Photo by Jurica Koletić on Unsplash

*upcoming shows images:*  
- mozart - https://wallpaperaccess.com/mozart  
- firework - Photo by Erwan Hesry on Unsplash  
- christmas - Photo by Rodion Kutsaev on Unsplash

*Microphone hero-image:*  
- Photo by Claus Grünstäudl on Unsplash

**Audio files**  
All audio files come from Spotify.   
All the copyrights belong the composers and/or the performers.  
  
- Ubi Caritas - composed by Ola Gjeilo, performed by Voces8.  
- And so it goes - arranged by Bob Chilcott, performed by The King’s Singers  
- Cerco te - performed by Petra Berger and Joshua Payne  
- Quartet (A model of decorum and tranquility) from Chess - composed by Benny Andersson and Björn Ulvaeus - performed by Elaine Paige, Tommy Körberg, Denis Quilley and Björn Skifs. 

**Video files**  
All video files come from YouTube.  
All the copyrights belong the composers and/or the performers. 
- Supercaligrafilisticaxpialidocious - composed by Richard and Robert Sherman - arranged and performed by The Newfangled Four.  
- Duetto buffo di due gatto (Cat Duet) - composed by Gioachino Rossini - performed by Chichi Enu and Adriene Ivey


## Acknowledgements:  
My mentor Antonio Rodriguez  
Tutor support at CI  
Jolanda Grutter for giving me tips on the design of my webpage.