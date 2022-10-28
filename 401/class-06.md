# Class 06

## Index

[Home](../README.md)  
[Java: Object and Class](#java-object-and-class)  
[Java: Static Keyword](#java-static-keyword)  
[Singleton](#java-singleton-class)  

## [Java: Object and Class](https://docs.oracle.com/javase/tutorial/java/concepts/)

- What is the difference between an Object and a Class in Java?
  - An `object` is a software bundle of related state and behavior. Software objects are often used to model the real-world objects that you find in everyday life.
  - A `class` is a blueprint or prototype from which objects are created.

| Class                                                             | Object                                                                          |
|-------------------------------------------------------------------|---------------------------------------------------------------------------------|
| A class is a template for creating objects in program.            | The object is an instance of a class.                                           |
| A class is a logical entity                                       | Object is a physical entity                                                     |
| A class does not allocate memory space when it is created.        | Object allocates memory space whenever they are created.                        |
| You can declare class only once.                                  | You can create more than one object using a class.                              |
| Example: Car.                                                     | Example: Jaguar, BMW, Tesla, etc.                                               |
| Class generates objects                                           | Objects provide life to the class.                                              |
| Classes can’t be manipulated as they are not available in memory. | They can be manipulated.                                                        |
| It doesn’t have any values which are associated with the fields.  | Each and every object has its own values, which are associated with the fields. |
| You can create class using “class” keyword.                       | You can create object using “new” keyword in Java                               |

[Tables Source](https://www.guru99.com/difference-between-object-and-class.html)

- What is a `Design Pattern`? Describe one or two with analogies from your previous work experience.
  - A design pattern is a template for how to solve a problem. It is common practice to create design patterns that provide a reusable solution to a commonly occuring problem.

    - When designing a 3D player controller, working with analog controller input was frequently a thing to wrangle. Specifically, I found the need to translate controller input relative to the player facing in regard to the camera view. I created an algorithm to process the data and provide a flattend angle to drive the player movement in the correct direction.  This design patter was reusable for many applications such as driving a car, steering a boat and even applying force to a submarine.

    - Another design patter was processing LERP (linear interpolation) data. With game development, lerps and slerps (sphereical liner interpolation) are used all the time for many different applications. I wrote two algorithms to handle each, lerp and slerp, allowing me to quickly get lerped data on the fly.

## [Java: Static Keyword](https://www.programiz.com/java-programming/static-keyword)

- `Static` methods are also called what? Why?
  - `Static` methods are also call class methods.
  - The benifit of class methods is that you don't have to create an instance of the class to have access to it. the `Math` class is a good example of this as almost all of its members are static.

## [Java: Singleton Class](https://www.programiz.com/java-programming/singleton)  

- A `Singleton` is a design pattern rather than a feature specific to Java. You can use the concept of a singleton in many programming languages.

- It's important to note that, there are only a few scenarios (like logging) where singletons make sense. It is recommended you avoid using singletons completely if you are not sure whether to use them or not.
  - They are generally used as a global instance, why is that so bad? Because you hide the dependencies of your application in your code, instead of exposing them through the interfaces. Making something global to avoid passing it around is a code smell.

  - They violate the single responsibility principle: by virtue of the fact that they control their own creation and lifecycle.

  - They inherently cause code to be tightly coupled. This makes faking them out under test rather difficult in many cases.

  - They carry state around for the lifetime of the application. Another hit to testing since you can end up with a situation where tests need to be ordered which is a big no no for unit tests. Why? Because each unit test should be independent from the other.

[Back To Top](#class-06)
