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
----------------
issue: I want the text of the carousel centered.
trial: text-align: center -> doesn't work.
trial: margin: auto -> doesn't work.
trial: rename the carousel-caption class to concert-item and wrap everything in a div.
set the parent div to position: absolute and set position: relative for concert-item.
doesn't work. 
TO BE CONTINUED
------------------

issue: the card heigths aren't equal length. 
trial: according to bootstrap you should add h-100 to the card.
This solves the equal length, but the cards are now outside of the container.
TO BE CONTINUED
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
issue: on index.html, the carousel-text isn't aligned in the center and isn't responsive.
solution: I accidentally deleted the 'carousel-caption'-class.