# Images (406-427)

- Specifying image sizes helps
pages to load more smoothly
because the HTML and CSS
code will often load before the
images, and telling the browser
how much space to leave for an
image allows it to render the rest
of the page without waiting for
the image to download.


- Where the <img> elements
appear in the HTML, rather
than using width and height
attributes you can use these
names as values for the class
attribute: 

  - small 
  
  - medium

  - large



# Alianing img using css 

 web
page authors are increasingly
using the float property to align
images. There are two ways that
this is commonly achieved:


1. The float property is added
to the class that was created to
represent the size of the image
(such as the small class in our
example).

2.  New classes are created with
names such as align-left or
align-right to align the images
to the left or right of the page.
These class names are used in
addition to classes that indicate
the size of the image. (so its two classes to the same img)



# centering img in css 

By default, images are inline
elements. This means that they
flow within the surrounding text.
In order to center an image, ***it should be turned into a blocklevel element using the display property with a value of block.***

1.  On the **containing element**,
you can use the **text-align**
property with a value of **center.**

2. On the **image itself**, you can
use the use the **margin** property
and set the values of the **left and right** margins to **auto.**

<br>
<br>
<br>
<br>

# Background Images
<br>

`body {`

`background-image: url("images/pattern.gif");}`

<br>
<br>
<br>
<br>



# Repeating Images

<br>
<br>

The background-repeat
property can have four values: 

<br>

1. **repeat** :
The background image is
**repeated both horizontally and vertically** (the default way it
is shown if the backgroundrepeat property isn't used).
<br>

2. **repeat-x** :
The image is repeated
**horizontally** only 

`body {`

`background-image: url("images/header.gif");`

`background-repeat: repeat-x;}`

<br>

3. **repeat-y** :
The image is repeated vertically
only.
<br>


4. **no-repeat** :
The image is only shown once.
The `background-attachment`
property **specifies** whether a **background image should stay in one position** or **move as the userscrolls up and down** the page. It
can have one of two values:

  - **fixed** : The background image stays in the same position on the page.

  - **scroll** : The background image moves up and down as the user scrolls up and down the page.
<br>
<br>

`body {`

`background-image: url("images/tulip.gif");`

`background-repeat: no-repeat;`

`background-attachment: fixed;}`
<br>
<br>
<br>
<br>


# background position look page (415)
<br>
<br>

`background-position`
<br>

When an **image is not being repeated** you can use the
`background-position`
property to **specify where in the browser window the background image should be placed.**
<br>

This property usually has a ***pair of values***. The first represents
the **horizontal position** **and**the
second represents the **vertical**.

<br>

`background-position: center top;}`
<br>

If you only specify one value,
the second value will default to
**center.**

<br>
<br>
<br>
<br>

## shorthand
<br>
<br>

`background`

<br>
<br>

The `background` property acts
like a shorthand for all of the
other background properties
you have just seen, and also the
background-color property.

1. background-color

2. background-image

3. background-repeat

4. background-attachment

5. background-position

<br>
<br>

`body {`

`background: #ffffff url("images/tulip.gif")`

` no-repeat top right;}`

<br>
<br>
<br>
<br>

# image Rollovers & Sprites look page (417)

<br>
Using CSS, it is possible to create
a **link or button** that **changes to a second style** when a user **moves their mouse over it** (**known as a rollover**) and a **third** style **when** they **click on it.**

<br>
<br>
<br>
<br>

# CSS3: Gradients Important look (419)
<br>
<br>
 using `background-image`


<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>


# Practical Information (476-492)


# Search Engine Optimization (SEO)

**Search engine optimization** (or
SEO) is the practice of trying
to help your site appear nearer
the top of search engine results
when people look for the topics
that your website covers.


In order to determine who comes
first in the search results, search
engines do not only look at what
appears on your site. They also
consider how many sites link
to you (and how relevant those
links are). For this reason, SEO
is often split into two areas:
on-page techniques and off-page
techniques.



- **On-Page Techniques** : methods you can use on your web pages to improve their rating in search engines.

The main component of this is
looking at **keywords** that people
are likely to enter into a search
engine if they wanted to find
your site, and then including
these in the text and HTML code
for your site in order to help the
search engines know that your
site covers these topics.
 <br>

- **Off-Page Techniques**: Getting other sites to link to you
is just as important as on-page
techniques. Search engines help
determine how to rank your
site by looking at the number of
other sites that link to yours.


Search engines also look at the
words between the opening
`<a> tag and closing </a>` tag
in the link. If the text in the link
***contains keywords (rather than just click here or your website address) it may be considered more relevant.***
<br>
<br>


## On-Page SEO

In every page of your website there are seven key places where keywords
can appear in order to improve its findability

1. **Page Title** : It is specified in the `<title>` element which lives inside the `<head>` element.


2.  **URL / Web Address** : The name of the file is part of
the URL

3. **Headings** : If the keywords are in a heading` <hn>` element then a search engine will know that this page isall about that subject and give it greater weight than other text.

4. **Text** :  it helps to repeat the keywords in the main body of the text at least 2-3
times.

5. **Link Text** : Use keywords in the text that
create links between pages
(rather than using generic
expressions such as "click here").

6. ***Image Alt Text** :
Search engines rely on you
providing accurate descriptions
of images in the alt text.

7. **Page Descriptions** :
The description also lives inside
the `<head>` element and is
specified using a `<meta>` tag.
It should be a sentence that
describes the content of the
page.




<br>
<br>


## identify the right keywords and phrases for your site. for more look page(482)

1. Brainstorm

2. Organize 

3. Reasearch  :[adwords.google.co.uk/select/KeywordToolExternal](adwords.google.co.uk/select/KeywordToolExternal) , 

[www.wordtracker.com](www.wordtracker.com) ,

[www.keyworddiscovery.com](www.keyworddiscovery.com) .


4.  Compare

5.  Refine

6. Map



## Analytics: Learning about your Visitors (look page 438)

As soon as people start coming to your site, you can start analyzing
how they found it, what they were looking at and at what point they are
leaving.One of the best tools for doing this is a free service offered by
Google called ***Google Analytics.**



[Reading Link]()