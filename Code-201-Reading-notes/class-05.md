# Images HTML
If you are building a site from scratch, it is good
practice to create a folder for all of the images
the site uses.

### How to add an image to you HTML page
Using the tag ***<img>***
`<img src="images/quokka.jpg" alt="A family of`
 `quokka" title="The quokka is an Australian`
 `marsupial that is similar in size to the`
 `domestic cat." />`

 ***src*** : link to the image
 ***alt*** : describtin about the image
 ***title*** : additional information


  ### height and width 

  to spicifiy image size tou can add height and width in side your tag 


  ## 3 Rules to remeber when you want to use an image 
  - Save images in the right **format** 
  - Save images at the right **size**
  - Use the correct resolution


  ### Notes about images 
  - Whenever you have many different
colors in a picture you should use a **JPEG**.
A photograph that features snow or an
overcast sky might look like it has large
areas that are just white or gray, but the
picture is usually made up of many different
colors that are subtly different.

  - use photoshop to set the right format and resuliotion and size

  - ***Transparency*** : If the transparent part of the
image has straight edges and
it is 100% transparent (that is,
not semi-opaque), you can save
the image as a GIF (with the
transparency option selected).

- ***Checking the Size of Images*** :If you are updating a website, you might need to check the size of an
existing image before creating a new one to replace it. 


  - Use ***GIF or PNG***  format
when saving images
with few colors or large
areas of the same color.



## <figure> 
Images often comes with caption so `<figure>` element to
contain images and their caption
so that the two are associated.
You can have more than one
image inside the `<figure>`
element as long as they all share
the same caption.

`<figcaption>`: The `<figcaption>` element has
been added to HTML5 in order
to allow web page authors to add
a caption to an image.

**Example**:

`<figure>`

`<img src="images/otters.jpg" alt="Photograph of`

 `two sea otters floating in water">`

`<br />`

 `<figcaption>Sea otters hold hands when they`

 `sleep so they don't drift away from each`

 `other.</figcaption>`

 `</figure>`



# CSS Colors 

Every color on a computer screen is created by mixing amounts of red,
green, and blue. To find the color you want, you can use a color picker.


## Contrast

When picking foreground and background
colors, it is important to ensure that there is
enough contrast for the text to be legible.


## Opacity, rgba

The CSS3 rgba property allows
you to specify a color, just like
you would with an RGB value,
but adds a fourth value to
indicate opacity. This value is
known as an `alpha` value and is
a number between 0.0 and 1.0
(so a value of 0.5 is 50% opacity
and 0.15 is 15% opacity). The
rgba value will only affect the
element on which it is applied
(not child elements).


## HSL Colors

**Hue**:
Hue is the colloquial idea of
color. In HSL colors, hue is often
represented as a color circle
where the angle represents the
color, although it may also be
shown as a slider with values
from 0 to 360.

**Saturation**:
Saturation is the amount of
gray in a color. Saturation is
represented as a percentage.
100% is full saturation and 0%
is a shade of gray.

**lightness**:
Lightness is the amount of
white (lightness) or black
(darkness) in a color. Lightness
is represented as a percentage.
0% lightness is black, 100%
lightness is white, and 50%
lightness is normal. Lightness
is sometimes referred to as
luminosity


# Texts 


## fonts
**Serif**
Serif fonts have extra details on
the ends of the main strokes of
the letters. These details are
known as serifs.

**Sans-Serif**
Sans-serif fonts have straight
ends to letters, and therefore
have a much cleaner design.

**Monospace**
Every letter in a monospace (or
fixed-width) font is the same
width. (Non-monospace fonts
have different widths.)


## fonts family 
The font-family property
allows you to specify the
typeface that should be used for
any text inside the element(s) to
which a CSS rule applies.

## font-size
- ***pixels**
Pixels are commonly used
because they allow web
designers very precise control
over how much space their text
takes up. The number of pixels is
followed by the letters px.

- **Percentages**
The default size of text in
browsers is 16px. So a size of
75% would be the equivalent of
12px, and 200% would be 32px.
If you create a rule to make all
text inside the `<body>` element
to be 75% of the default size (to
make it 12px), and then specify
another rule that indicates the
content of an element inside the
`<body>` element should be 75%
size, it will be 9px (75% of the
12px font size).

- **Ems**
An em is equivalent to the width
of a letter m.



## @font-face
 allows you to use
a font, even if it is not installed
on the computer of the person
browsing, by allowing you to
specify a path to a copy of the
font, which will be downloaded if
it is not on the user's machine.

- **font-family**
This specifies the name of the
font

- **src**
This specifies the path to the
font.

`@font-face {`
`font-family: 'ChunkFiveRegular';`
`src: url('fonts/chunkfive.eot');}`
`h1, h2 {`
`font-family: ChunkFiveRegular, Georgia, serif;}`



## Notes about fonts
- **When choosing a typeface, it is important to understand that a browser will usually only display it if it's  installed on that user's computer.**

- **If you design on a Mac, it is important to check what the typefaces look like on a PC because PCs can render type less smoothly. But if you design on a PC, then it should look fine on a Mac.**

- **The reason Photoshop and InDesign offer the same sizes of text s because they are setaccording to a scale ratio that was developed by European typographers in the sixteenth century.**

- **Different browsers support different formats for fonts ), so you will need to supply the font in severa**
**variations to reach all browsers. If you do not have all of these formats for your font, you can upload the **font to a website called ***FontSquirrel*** where they will convert it for you



## Styling Links

**:link**:
This allows you to set styles
for links that have not yet been
visited. 

**:visited**:
This allows you to set styles for
links that have been clicked on.

**:hover**
This is applied when a user
hovers over an element with a
pointing device such as a mouse. 

**:active**
This is applied when an element
is being activated by a user; for
example, when a button is being
pressed or a link being clicked. 


**:focus**
This is applied when an element
has focus. Any element that
you can interact with, such as a
link you can click on or any form
control can have focus.

[link](https://github.com/saraalshater/Reading-notes/blob/main/Code-201-Reading-notes/class-05.md)
