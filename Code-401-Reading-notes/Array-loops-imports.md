# [Packages and Import]()

**Package = directory.** Java `classes` can be grouped together in `packages`.**A package name is the same as the directory (folder) name which contains the .java files.** You declare packages when you define your Java program, and you name the packages you want to use from other libraries in an import statement.

## Package declaration

The first statement, other than comments, in a Java source file, **must be the package declaration.**

Following the optional package declaration, you can have import statements, which allow you to specify classes from other packages that can be referenced without qualifying them with their package.

its recommends that you do not use default packages.

## Package declaration syntax

The statement order is as follows.

1. Package statment (optional).
2. Imports (optional).
3. Class or interface definitions.


`// This source file must be Drawing.java in the illustration directory.`

`package illustration;`
`
`import java.awt.*;`

`public class Drawing {`
 `   . . .`
`}`

## Imports:

example : 

The `JOptionPane` class is in the swing package, which is located in the javax package. The wildcard character (*) is used to specify that all classes with that package are available to your program. This is the most common programming style.

import javax.swing.*;  // Make all classes visible altho only one is used.

class ImportTest {
    public static void main(String[] args) {
        `JOptionPane`.showMessageDialog(null, "Hi");
        System.exit(0);
    }
}

## Common imports

- import java.awt.*;	Common GUI elements.
- import java.awt.event.*;	The most common GUI event listeners.
- import javax.swing.*;	More common GUI elements. Note "javax".
- import java.util.*;	Data structures (Collections), time, Scanner, etc classes.
- import java.io.*;	Input-output classes.
- import java.text.*;	Some formatting classes.
- import java.util.regex.*;	Regular expression classes.




# [Java loop](https://www.baeldung.com/java-loops)


## types of loops that we can find in Java:

- for loop  
 A for loop is a control structure that allows us to repeat certain operations by incrementing and evaluating a loop counter.

 exmaple:

 `for (int i = 0; i < 5; i++) {`
    `System.out.println("Simple for loop: i = " + i);`
 `}`


- for-each loop



- While loop

 The while loop is Java's most fundamental loop statement. It repeats a statement or a block of statements while its controlling Boolean-expression is true.
 `int i = 0;`
 `while (i < 5) {`
    `System.out.println("While loop: i = " + i++);`
 `}`



- Do-While loop
 The do-while loop works just like the while loop except for the fact that the first condition evaluation happens after the first iteration of the loop.
 `do {`
   ` statement;`
 `} while (Boolean-expression);`