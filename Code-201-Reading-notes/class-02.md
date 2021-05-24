# IMPORTANT HTML TAGS
- Headings : heading tags goes decending from h1 until h6 where h1 is the biggest and h6 is the smallest


``<h1><h2><h3><h4><h5><h6>``


- Paragraph: `<p> </p>` is used to create a paragraph

- Bold : You can bold your text by wrapping it with the enclosing tag `<b> </b>`

- Italic : You can Italic your text by wrapping it with the enclosing tag `<i> </i>`

- Superscript : The `<sup> </sup>` element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power such as 2<sup>2</sup>.

- Subscript : The `<sub></sub>` element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H<sub>2</sub>0.

- Line break : `<br  />` 

- Horizontal rules : To create a break between themes — such as a change of topic in a book or a new scene in a play — you can add a horizontal rule between sections using the `<hr />` tag.

## What is Visual editors ? 
Visual editors often resemble word processors. Although each editor will differ slightly, there are some features that are common to most editors that allow you to control the presentation of text.


## What is code views ? 
Code views show you the code created by the visual editor so you can manually edit it, or so you can just enter new code yourself. It is often activated using a button with an icon that says HTML or has angled brackets. White space may be added to the code by the editor to make the code easier to read.

# Semantic markup
##  What is Semantic markup ? 
Elements that are not intended to affect the structure of your web pages, but they do add extra information to the pages — they are known as semantic markup.

##  Why we use Semantic markup ?
The reason for using these elements is that other programs, such as screen readers or search engines, can use this extra information.

## Examples of Semantic markup ?
- `<strong>`: The use of the `<strong>`element indicates that its content has strong importance. 
- `<em>` :The `<em>` element indicates emphasis that subtly changes the meaning of a sentence.
- `<blackqoute>` :The `<blockquote>` element is used for longer quotes that take up an entire paragraph. Note how the `<p>` element is still used inside the `<blockquote>`element. 
- `<q>`: The `<q>` element is used for shorter quotes that sit within a paragraph.
- `<cite>`: When you are referencing a piece of work such as a book, film or research paper, the  `<cite> `element can be used to indicate where the citation is from.
- `<address>` :The `<address>` element has quite a specific use: to contain contact details for the author of the page.
- `<ins>`: The `<ins>` element can be used to show content that has been inserted into a document. 
- `<del>` : The `<del>` element can show text that has been deleted from it.



# Introducing CSS

## CSS rule contain two parts : 
selector and declartion 

***Example***

p {
    background-color: blue;
}

***p*** is the ***selector*** 
inside the ***{}*** is the ***declartion***.

CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon.


## There is 3 ways to style your web with css

- External 
- Internal 
- Inline

## How  CSS inline rules?

***Last rule***
If the two selectors are identical, the latter of the two will take precedence. Here you can  see the second i selector takes precedence over the first.

***Specificity***
If one selector is more specific than the others, the more specific rule will take precedence over more general ones. 

***Important***
You can add !important after any property value to indicate that it should be considered more important than other rules that apply to the same element.



## Javascript instructures
- Statements should end with a semicolon. 
- STATEMENTS ARE INSTRUCTIONS AND
EACH ONE STARTS ON A NEW LINE 


## WHY we write comments? 
You should write comments to explain what your code does. 

## How we write comments ?
 1. Multipale line comments is written like this : /* here you wite the comment */
 2. Single line comments is written like this : here you wite the comment //


 ## What is variable ?
 A script will have to temporarily
store the bits of information it
needs to do its job. It can store this
data in variables.

## How to declare a variable ? 
Create a variable by typing var then give it a name that discribe it job 
var userName;

## How to give it a value ?
 by giving the variable name a value 

***example***
userName = 'sara';

## ARRAY 
An array is a special type of variable. It doesn't
just store one value; it stores a list of values. 

## WHEN to use Array
- You should consider using an
array whenever you are working
with a list or a set of values that
are related to each other.

- Arrays are especially helpful
when you do not know how
many items a list will contain
because, when you create the
array, you do not need to specify
how many values it will hold.

## How to create an array ?

`var color;

color = ['black', 'white','blue'];`  


- The values are assigned to the
array inside a pair of square
brackets, and each value is
separated by a comma. The
values in the array do not need
to be the same data type, so you
can store a string, a number and
a Boolean all in the same array.

- Values in an array are accessed as if they are in
a numbered list. It is important to know that the
numbering of this list starts at zero (not one). 

- Each array has a property called
length, which holds the number
of items in the array. 









