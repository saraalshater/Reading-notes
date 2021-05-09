# **JavaScript Functions**

A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

## JavaScript Function Syntax
* Function names can contain ***letters, digits, underscores, and dollar signs (same rules as variables)***.

* The parentheses may include parameter names separated by commas:
***(parameter1, parameter2, ...)***

* **The code to be executed, by the function, is placed inside curly brackets: {}**

` function name(parameter1, parameter2, parameter3) {
  // code to be executed
}`

* function parameters are listed inside the parentheses **()** in the function definition.

* Function arguments are the values received by the function when it is invoked.

* Inside the function, the arguments (the parameters) behave as local variables.

## When function executed?
function executed when it called: 
* When an event occurs (when a user clicks a button)
* When it is invoked (called) from JavaScript code
* Automatically (self invoked)

## Function Return
* When JavaScript reaches a `return` statement, the function will stop executing.

* Functions often compute a return value. The return value is "returned" back to the "caller".

## Why Functions?
* You can reuse code: Define the code once, and use it many times.

* You can use the same code many times with different arguments, to produce different results.

## Local Variables
Variables declared within a JavaScript function, become LOCAL to the function.

Local variables can only be accessed from within the function.

``function myFunction() {
  var carName = "Volvo";
  // code here CAN use carName
}``
