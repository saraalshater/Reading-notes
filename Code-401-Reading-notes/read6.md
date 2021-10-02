## What Is Inheritance?

Example : Many kind of obejcts in real life have common properties. yet they also have things that make them different. 

- Object-oriented programming allows classes to **inherit** commonly used state and behavior from other classes. each class **is allowed to have one direct superclass**, and each superclass has the potential for an unlimited number of **subclasses**.


#### The syntax for creating a subclass :

At the beginning of your class declaration, use the **extends** keyword, followed by the name of the class to inherit from:


 class MountainBike extends Bicycle {

    // new fields and methods defining 
    // a mountain bike would go here

 }

- A class that is derived from another class is called a **subclass** (also a derived class, extended class, or child class). The class from which the subclass is derived is called a **superclass** (also a base class or a parent class).
- Excepting **Object**, which **has no superclass**, every class has one and only one direct superclass (single inheritance). In the absence of any other explicit superclass, every class is implicitly a subclass of Object.

- When you want to create a new class and there is already a class that includes some of the code that you want, you can derive your new class from the existing class. In doing this, you can reuse the fields and methods of the existing class without having to write (and debug!) them yourself.

- A **subclass inherits** all the members **(fields, methods, and nested classes)** from its superclass.

- **Constructors are not members**, so they are **not** inherited by subclasses, but **the constructor of the superclass can be invoked from the subclass**.


### The Java Platform Class Hierarchy




![All Classes in the Java Platform are Descendants of Object](https://docs.oracle.com/javase/tutorial/figures/java/classes-object.gif)
#### All Classes in the Java Platform are Descendants of Object


## What You Can Do in a Subclass?

**A subclass inherits all of the public and protected members of its parent, no matter what package the subclass is in. If the subclass is in the same package as its parent, it also inherits the package-private members of the parent. You can use the inherited members as is, replace them, hide them, or supplement them with new members:**
- 

## What Is an Interface?

Example : the buttons on the front of your television set,are the interface between you and the electrical wiring on the other side of its plastic casing.

objects define their interaction with the outside world through the methods that they expose,**Methods form the object's interface with the outside world**


**an interface is a group of related methods with empty bodies.**


**Implementing an interface** allows a class to become more **formal** about the behavior it promises to provide. **Interfaces form a contract between the class and the outside world**, and this contract is enforced at build time by the compiler. **If your class claims to implement an interface, all methods defined by that interface must appear in its source code before the class will successfully compile.**


- interfaces is like a guidance that's wriiten by the auto manufacturers that spells out in detail what methods can be invoked to make the car move 


## Interfaces in Java

- an interface is a reference type, similar to a class, that can contain only constants, method signatures, default methods, static methods, and nested types.

-  **Interfaces cannot be instantiated—they can only be implemented by classes or extended by other interfaces.**

Define an enter face: 


public **interface** OperateCar {

   
}



**To use an interface**, you write a class that implements the interface. When an instantiable class implements an interface, it provides a method body for each of the methods declared in the interface. 

public class OperateBMW760i implements OperateCar {

   
}