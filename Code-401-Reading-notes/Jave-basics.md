# [Java basic](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/index.html)

## Variables

- Variables

  - **Instance Variables** (Non-Static Fields) Technically speaking, objects store their individual states in "non-static fields", that is, fields declared without the static keyword. Non-static fields are also known as instance variables because their values are unique to each instance of a class (to each object, in other words).

  - **Class Variables** (Static Fields) A class variable is any field declared with the static modifier; this tells the compiler that there is exactly one copy of this variable in existence, regardless of how many times the class has been instantiated.
  
  - **Local Variables** Similar to how an object stores its state in fields, a method will often store its temporary state in local variables. The syntax for declaring a local variable is similar to declaring a field (for example, int count = 0;). There is no special keyword designating a variable as local; that determination comes entirely from the location in which the variable is declared — which is between the opening and closing braces of a method. As such, local variables are only visible to the methods in which they are declared; they are not accessible from the rest of the class.

  - **Parameters**



- Names
   - **Always begin your variable names with a letter**, not "$" or "_", White space is not permitted.

   - When choosing a name for your variables, use full words instead of cryptic abbreviations.
 
   - use camelCase.




## Operator

| Operators | Precedence |
|-----------|------------|
| postfix | expr++ expr-- |
| unary | ++expr --expr +expr -expr ~ ! |
| multiplicative | * / % |
| additive | + - |
| shift | << >> >>>|
| relational | < > <= >= instanceof | 
| equality | == != |
| bitwise AND  | & |
| bitwise exclusive OR |  ^ |
| bitwise inclusive OR | | |
| logical AND | && | 
| logical OR |  || |
| ternary | ? : |
| assignment | = += -= *= /= %= &= ^= |= <<= >>= >>>= |



## Expressions, Statements, and Blocks

- Expressions
 The data type of the value returned by an expression depends on the elements used in the expression. The expression cadence = 0 returns an int because the assignment operator returns a value of the same data type as its left-hand operand; in this case, cadence is an int. As you can see from the other expressions, an expression can return other types of values as well, such as boolean or String.
 The Java programming language allows you to construct compound expressions from various smaller expressions as long as the data type required by one part of the expression matches the data type of the other.

- Statements
 Statements are roughly equivalent to sentences in natural languages. A statement forms a complete unit of execution. The following types of expressions can be made into a statement by terminating the expression with a semicolon (;).

 - Assignment expressions
 - Any use of ++ or --
 - Method invocations
 - Object creation expressions


- Blocks
A block is a group of zero or more statements between balanced braces and can be used anywhere a single statement is allowed. 


## Control Flow Statements
The statements inside your source files are generally executed **from top to bottom**, in the order that they appear. Control flow statements, however, break up the flow of execution by employing decision making, looping, and branching, enabling your program to conditionally execute particular blocks of code. This section describes the decision-making statements (if-then, if-then-else, switch), the looping statements (for, while, do-while), and the branching statements (break, continue, return) supported by the Java programming language.




----------------------------------------


# What does it mean to compile code?

When you compile code, the compilor (usually another program) takes the program the human wrote, and converts it into the program the computer can understand (i.e. converts from Java to machine language). The very short version could be, yes, compile means to make the code executable.

Something you may run into is people saying code does or does not compile. This means the compilor they used checks to make sure their program is written correctly according to the rules of the programming language. For example, most programming languages make you put a semicolon (;) at the end of every line. A very common mistake is to forget that semicolon, so when you try and compile the compilor gives you an error.

--------------------------------------------------


# [Making Sense of Java’s API Documentation](https://www.dummies.com/programming/java/making-sense-of-javas-api-documentation/)


## [Java’s API Documentation](https://docs.oracle.com/javase/8/docs/api/)