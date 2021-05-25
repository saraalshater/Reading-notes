# HTML Links 
Types of links:
● Links from one website to another

● Links from one page to another on the same website

● Links from one part of a web page to another part of the
same page

● Links that open in a new browser window

● Links that start up your email program and address a new
email to someone

## How to write links ?

writing links using the tag `<a>`

##  LinkS syntax

`<a href:"https://facebook.com">link to facebook</a>`

- The text between the opening
`<a> `tag and closing `</a>` tag
is known as link text. Where
possible, your link text should
explain where visitors will be
taken if they click on it (rather
than just saying "click here"). 


## Linking to other pages in the same site

- If all the pages of the site are in
the same folder, then the value
of the href attribute is just the
name of the file. which called ***relative URL***

`<ul>`

`<li><a href="index.html">Home</a></li>`

 `<li><a href="about-us.html">About</a></li>`

 `<li><a href="movies.html">Movies</a></li>`

 `<li><a href="contact.html">Contact</a></li>`

`</ul>`


## Email links 

To create a link to Email you use the `<a>`
element. However, this time the
value of the href attribute starts
with ***mailto***: and is followed by
the email address you want the
email to be sent to.

`<a href="mailto:jon@example.org">Email Jon</a>`


## Open links to a new window

If you want a link to open in a
new window, you can use the
***target*** attribute on the opening
`<a>` tag. The value of this
attribute should be **_blank**.


`<a href="http://www.imdb.com" target="_blank"> Internet Movie Database</a> `



##  Link to a specific part of a different page
If you want to link to a specific
part of a different page (whether
on your own site or a different
website) you can use a similar
technique.



As long as the page you are
linking to has **id** attributes that
identify specific parts of the
page, you can simply add the
same syntax to the end of the
link for that page.


`<li><a href="#Bio">Biography</a></li>`

 `<li id="Bio">My name is Sara. I am 24, I am intrested in arts </li>`

 # Css Layout

 - CSS treats each HTML element as if it is in its
own box. This box will either be a ***block-level***
box or an ***inline box.***

- ***Block-level***: boxes start on a new line and act as the main building blocks of any layout
- ***Inline boxes***: flow between surrounding text.
- ***containing or parent element***: If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

## Positioning 
***Normal flow*** Every block-level element
appears on a new line, causing
each item to appear lower down
the page than the previous one.
Even if you specify the width
of the boxes and there is space
for two elements to sit side-byside, they will not appear next
to each other. This is the default
behavior (unless you tell the
browser to do something else).


***Relative Positioning***
This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
bottom, or left of where it
would have been placed. This
does not affect the position of
surrounding elements; they stay
in the position they would be in
in normal flow.

***Absolute positioning***
This positions the element
in relation to its containing
element. It is taken out of
normal flow, meaning that it
does not affect the position
of any surrounding elements
(as they simply ignore the
space it would have taken up).
Absolutely positioned elements
move as users scroll up and
down the page


***Fixed Positioning***
This is a form of absolute
positioning that positions
the element in relation to the
browser window, as opposed
to the containing element.
Elements with fixed positioning
do not affect the position of
surrounding elements and they
do not move when the user
scrolls up or down the page


***Floating Elements***
Floating an element allows
you to take that element out
of normal flow and position
it to the far left or right of a
containing box. The floated
element becomes a block-level
element around which other
content can flow.



#  Javascript functions, methods, and objects








# Dictinory 

- Root folder: The top-level The root folder
contains all of the other files and
folders for a website. 

- 




