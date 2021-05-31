# Key Concepts in Positioning Elements

## 1. Building Blocks

CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.

## what is block level and inline elements ?


- **Block-level boxes** : ***start on a new line*** and act as the main building blocks
of any layout

Examples of block level elemnts:
`<h1> <p> <ul> <li>`


- **inline boxes** : ***flow between surrounding text***. You can
control how much space each box takes up by setting the width of the
boxes (and sometimes the height, too). To separate boxes, you can use
borders, margins, padding, and background colors.


Examples of inline elements:
`<img> <b> <i>`




## 2. Containing Elements

If one **block-level element** sits **inside** another
**block-level element** then **the outer box is**
known as the containing or **parent element.**





## Controlling the Position of Elements

- **Normal flow**
Every block-level element
appears on a new line, causing
each item to appear lower down
the page than the previous one.
Even if you specify the width
of the boxes and there is space
for two elements to sit side-byside, they will not appear next
to each other. This is the default
behavior (unless you tell the
browser to do something else).


- **Relative Positioning**
This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
bottom, or left of where it
would have been placed. **This does not affect the position of surrounding elements; they stay in the position** **they would be in in normal flow.**


- **Absolute positioning**
This **positions** the element
**in relation to its containing element.** It is taken out of
normal flow, meaning that it
does not affect the position
of any surrounding elements
(as they simply ignore the
space it would have taken up).
Absolutely positioned elements
move as users scroll up and
down the page.


- **box offset** properties to tell the browser how far from the top or bottom
and left or right it should be placed. 


- **Fixed Positioning**
This is a form of absolute
positioning that ***positions the element in relation to the browser window***, as opposed
to the containing element.
Elements with ***fixed positioning***
do not affect the position of
surrounding elements and ***they do not move when the user scrolls up or down the page***

- **Floating Elements**
Floating an element allows
you to ***take that element out of normal flow*** and position
it to the far left or right of a
containing box. **The floated element becomes a block-level element around which other content can flow.**

**When you move any element from normal flow, boxes can overlap. The ***z-index*** propertyallows you to control****which box appears on top.**




## position:relative

Relative positioning **moves** an element ***in relation to where it would have been in normal flow.***


For **example**, you can move it **10 pixels lower than it would have been in normal flow or 20% to the right.**


## position:absolute

The box is **taken out of normal flow and no longer affects the position of other elements on the page.** ***(They act like it is not there.) ***

**The box offset** properties (top
or bottom and left or right)
**specify where the element should appear in relation to its containing element.**


## position:fixed

It positions the element **in relation to the browser window.** Therefore, **when a user scrolls down the page, it stays in the exact same place.** 


## Example: ***this one placed it on the top of the page ***

`position: fixed;`

`top: 0px;`

`left: 50px;`

`padding: 10px;`

`margin: 0px;`

`width: 100%;`

`background-color: #efefef;}`



# Float **important**

The **float property** allows you
to **take an element in normal flow and place it as far to the left or right of the containing element as possible.**

***Anything else that sits inside the containing element will flow around the element that is floated.***


***When you use the float property, you should also use the width property to indicate how wide the floate element should be.***

## Using Float to Place Elements Side-by-Side ***important: (look page 371)***


## Clearing Floats

`clear`

The clear property allows you to say that ***no element (within the same containing element) should touch the left or righthand sides of a box.*** It can take the following values:

- left 
- right 
- both 
- none 

## Creating Multi-Column Layouts with Floats (look page 375)

# Screen Sizes

Resolution refers to the number of dots a screen shows per inch. Some
devices have a higher resolution than desktop computers and most
operating systems allow users to adjust the resolution of their screens.


# Page sizes 

Because screen sizes and display resolutions vary so much, web
designers often try to **create pages of around 960-1000 pixels wide**
(since most users will be able to see designs this wide on their screens)



## what is Fixed Width Layouts? 

**Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.**


## How to creat Fixed Width Layouts? 

**Look page(383)**

## what is Liquid Layouts? 

**Liquid layout designs stretch and contract as the user increases or decreases the size of their browserwindow. They tend to use percentages.**

## How to create liquid Layouts? 

**Look page(385)**



# Using grid in design 

## why its important ? 

● Creates a continuity between
different pages which may
use different designs
● Helps users predict where to
find information on various
pages
● Makes it easier to add new
content to the site in a
consistent way
● Helps people collaborate
on the design of a site in a
consistent way



## using multiple style sheet 

`@import`

there is 2 ways to create it 

1. 1: Your HTML page can link
to one style sheet and that
stylesheet can use the `@import`
rule to import other style sheets



2. In the HTML you can use a
separate `<link>` element for
each style sheet.












-------------------------------------------------------------------------------------------------


# Layout 


### Box Dimensions

**width, height**

- The most popular ways to
specify the size of a box are
to use ***pixels, percentages, or ems.***

- When you use ***percentages,***
the size of the box is relative to
the size of the ***browser window***
or, **if the box is encased within another box, it is a percentage of the size of the containing box.**

- When you use ***ems***, the size
of the **box** is based on the size
of **text within it**. Designers
have recently started to use
**percentages and ems** more for
measurements as they try to
create designs that are **flexible across devices which have different-sized screens**


## min-width max-width 

- The
**min-width** property specifies
***the smallest size a box can be displayed at when the browser window is narrow***, and the
**max-width** property indicates
***the maximum width a box can stretch to when the browser window is wide.***


## min-height, max-height

- If the box is not big enough to
hold the content, and the content
expands outside the box it can
look very messy. To control
what happens when there is not
enough space for the content of
a box, you can use the overflow
property, which is discussed on
the next page.


 ## Overflowing Content

- hidden
This property simply ***hides any extra content that does not fit in the box.***

`p { `
`    overflow : hidden;`
`}`





- scroll
This property ***adds a scrollbar to the box so that users can scroll to see the missing content.***

 `p { `
`    overflow : scroll;`
`}`



 ## Border, Margin & Padding

 - Every box has ***three available properties*** that can be adjusted to control its appearance:

 1. Border 
 2. margin 
 3. padding 



 ## border-color

 It is possible to individually
control the colors of the borders
on different sides of a box using:


border-top-color
border-right-color
border-bottom-color
border-left-color


## Padding 

The value of this property is
most often specified in **pixels**
(although it is also possible to
use **percentages or ems**). If a
percentage is used, the **padding is a percentage of the browser window** (or of the containing box if it is inside another box).

- **If a width is specified for a box, padding is added onto the width of the box**

## margin 

The margin property controls
the gap between boxes. Its value
is commonly given in **pixels**,
although you may also use
percentages or ems.


 **If the width of a box is specified then the margin is added to the width of the box.**


 ## Centering content

 - If you want to **center a box** on the **page** (or **center** it **inside the element that it sits in**), you can set the **left-margin** and **right-margin** to ***auto.***

- In order to **center a box on the page**, you need to **set a width for the box** (otherwise it will take
up the full width of the page).


## Display 

The display property allows
you to ***turn*** an **inline element**
into a **block-level element**

- **inline**
This causes a **block-level**
element to **act like** an **inline element.**

- **block**
This causes an **inline element** to
**act like** a **block-level element.**


- **inline-block**
This causes a ***block-level element** to **flow like** an **inline element**, while retaining other
features of a block-level element.

- **none**
This hides an element from the
page. In this case, the element
acts as though it is not on the
page at all (although a user could
still see the content of the box if
they used the view source option
in their browser).

## Visibility
- The **visibility** property allows
you to ***hide boxes from users but It leaves a space where the element would have been.***

- **hidden**
This hides the element.


## border-image

- The **border-image** property
***applies an image to the border of any box. It takes a background image and slices it into nine pieces.*** 


## box-shadow

The **box-shadow** property
***allows you to add a drop shadow around a box***

## border-radius

**border-radius** is the ability to
***create rounded corners on anybox.***