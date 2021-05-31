# Objects
Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names. 

- IN AN OBJECT: VARIABLES BECOME
KNOWN AS PROPERTIES 

- IN AN OBJECT: FUNCTIONS BECOME
KNOWN AS METHODS

Using an object literal, you both define and create an object in one statement.
its the easiest way to create an object

## Example of an object:

`var person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};`

## How to access?

You can access object properties in two ways:

with Dot

`objectName.propertyName`


with sequare braket

`objectName["propertyName"]`



# The Document Object Model (DOM)

specifies
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window. 


## Accessing elements

DOM queries may return one element, or they may return a Nodelist,
which is a collection of nodes. 


Sometimes you will just want to access one
individual element (or a fragment of the page that
is stored within that one element). Other times you
may want to select a group of element s, for example,
every `<hl>` element in the page or every <1 i>
element within a particular list. 


**GROUPS OF ELEMENT NODES**
If a method can return more than one node, it will
always return a Nodelist, which is a collection of
nodes (even if it only finds one matching element).
You then need to select the element you want from
this list using an index number (which means the
numbering starts at 0 like the items in an array). 

**FASTEST ROUTE**
Finding the quickest way to access an element
within your web page will make the page seem
faster and/or more responsive. This usually means
evaluating the minimum number of nodes on the
way to the element you want to work with. For
example, getEl ementByld () will quickly return one
element (because no two elements on the same
page should have the same value for an id attribute),
but it can only be used when the element you want
to access has an id attribute. 

[link](https://github.com/saraalshater/Reading-notes/blob/main/Code-201-Reading-notes/class-06.md)