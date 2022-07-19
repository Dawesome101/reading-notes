# Object-Oriented Programming, HTML Tables

## Index

[Home](./README.md)  
[Domain Modeling](#domain-modeling)  
[HTML Table Basics](#html-table-basics)  
[Introducing Constructors](#introducing-constructors)  
[Object Prototypes Using A Constructor](#object-prototypes-using-a-constructor)

## [Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)

1. Explain why we need domain modeling.
   - A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.
   - The idea behind domain modeling is to keep changes small and targeted if there is a need to change the algorithm in question.

## [HTML Table Basics](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics)

1. Why should tables not be used for page layouts?
   - Layout tables reduce accessibility for visually impaired users: Screenreaders, used by blind people, interpret the tags that exist in an HTML page and read out the contents to the user. Because tables are not the right tool for layout, and the markup is more complex than with CSS layout techniques, the screenreaders' output will be confusing to their users.
   - Tables produce tag soup: As mentioned above, table layouts generally involve more complex markup structures than proper layout techniques. This can result in the code being harder to write, maintain, and debug.
   - Tables are not automatically responsive: When you use proper layout containers (such as `<header>`, `<section>`, `<article>`, or `<div>`), their width defaults to 100% of their parent element. Tables on the other hand are sized according to their content by default, so extra measures are needed to get table layout styling to effectively work across a variety of devices.
2. List and describe 3 different semantic HTML elements used in an HTML `<table>`.
   - The [\<colgroup\>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/colgroup) HTML element defines a group of columns within a table.
   - [\<col\>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/col) The `<col>` HTML element defines a column within a table and is used for defining common semantics on all common cells. It is generally found within a `<colgroup>` element.
   - The [\<th\>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/th) HTML element defines a cell as header of a group of table cells. The exact nature of this group is defined by the scope and headers attributes.

## [Introducing Constructors](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics#introducing_constructors)

1. What is a constructor and what are some advantages to using it?
   - Constructors allow us to not have to duplicate code and make updating or changing objects much easier by alowing us to only have to change it once instead of for each object literal.
2. How does the term this differ when used in an object literal versus when used in a constructor?
   - When used in an object literal it really isn't that helpful as you could always just pull from the variable.  However, in a constructor it's very useful in that each instance will still work to pull for that objects instance information.  For example in this case, `person1.introduceSelf()` outputs "Hi! I'm Chris."; `person2.introduceSelf()` on the other hand outputs "Hi! I'm Deepti."

   ```JavaScript
    const person1 = {
    name: 'Chris',
    introduceSelf() {
      console.log(`Hi! I'm ${this.name}.`);
      }
    }
   ```

   ```JavaScript
    const person2 = {
      name: 'Deepti',
      introduceSelf() {
        console.log(`Hi! I'm ${this.name}.`);
      }
    }
   ```

## [Object Prototypes Using A Constructor](https://ui.dev/beginners-guide-to-javascript-prototype)

1. Explain prototypes and inheritance via an analogy from your previous work experience.
   - `prototype` is just a property that every function in JavaScript has and it allows us to share methods across all instances of a function. All our functionality is still the same but now instead of having to manage a separate object for all the methods, we can just use another object that comes built into the function itself, `Foo.prototype`.
   - Inheritance is when you create an instance of a class or constructor and "inhereit" its methods and/or properties while creating a subtyped object of said class or constructor. I.E.  Calf.health inherits the method heatlh from from Cow.health which inherits from Animal.health.  Calf is a type of Cow which is a Type of Animal.  The cool thing here is that calf can have special properties and methods if you like but doesn't need to recreate all of the basics that are already inside of its parrents.  For example, name, age, etc.

[Back to Top](#index)
