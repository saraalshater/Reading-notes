## EXECUTION CONTEXTS 


## UNDERSTANDING SCOPE
In the interpreter, each execution context has its own va ri ables object.
It holds the variables, functions, and parameters available within it.
Each execution context can also access its parent's v a ri ables object. 

The children can ask the parents for information in
their variables. But the parents cannot get variables
from their children. Each child will get the same
answer from the same parent. 


## UNDERSTANDING ERRORS
If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handl ing code. 



## ERROR OBJECTS 


There are seven types of built-in error objects in
JavaScript. You'll see them on the next two pages: 

- **Error** : Generic error - the other errors
are all based upon this error 

- **Syntax Error** : Syntax has not been followed

- **Reference Error** : Tried to reference a variable that is
not declared/within scope

- **TypeError** : An unexpected data type that
cannot be coerced 

- **Range Error** : Range Error

- **URI Error** : encodeURI ().decodeURI(),and
similar methods used incorrectly

- **Eval Error** : eval () function used incorrectly



## HOW TO DEAL WITH ERRORS

1. DEBUG THE SCRIPT TO FIX ERRORS

If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it.
You will find that the developer tools available in
every major modern browser will help you with
this task. In this chapter, you will learn about the
developer tools in Chrome and Firefox. (The tools in
Chrome are identical to those in Opera.)
IE and Safari also have their own tools (but there is
not space to cover them all).


2. HANDLE ERRORS GRACEFULLY

You can handle errors gracefully using try, catch,
throw, and f i na 1 ly statements.
Sometimes, an error may occur in the script for a
reason beyond your control. For example, you might
request data from a third party, and their server
may not respond. In such cases, it is particularly
important to write error-handling code. 




 [link](https://github.com/saraalshater/Reading-notes/blob/main/Code-201-Reading-notes/class-10.md)
