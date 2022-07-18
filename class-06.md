# Problem Domain, Objects, and the DOM

## Index

[Home](./README.md)  
[JavaScript Object Basics](#javascript-object-basics)  
[Introduction to the DOM](#introduction-to-the-dom)  

## [JavaScript Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)

1. How would you describe an object to a non-technical friend you grew up with?
   - Objects in javaScript are much like the way a dictionary works.  you have a word that is assigned to a definition.  Same thing with objects.  They call these keys (dictionary word: Cat) and values(dictionary definition for cat: A little demon that has fur.).
2. What are some advantages to creating object literals?
   -It is very common to create an object using an object literal when you want to transfer a series of structured, related data items in some manner, for example sending a request to the server to be put into a database. Sending a single object is much more efficient than sending several items individually, and it is easier to work with than an array, when you want to identify individual items by name.
3. How do objects differ from arrays?
   - `Objects` represent a "thing" in your code.  Objects are defined by a set of characteristics called properties.
   - `Arrays` are essentially a list of values stored in a single variable.  Arrays use numerical indexing to store and retreve values.
4. Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.
   - If an object property name is defined at runtime then you can't use dot notation to access the value, but you can pass the name as a variable inside brackets.  Because javaScript reads object references as strings you can access them in thier index as a string, like so `person['name'] = 'myName';`
5. Evaluate the code below. What does the term `this` refer to and what is the advantage to using `this`?
   - `this` is refering to variable itself `dog`
   - When you only have to create a single object literal, it's not so useful. But if you create more than one, `this` enables you to use the same method definition for every object you create.

```javaScript
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}
```

## [Introduction to the DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)

1. What is the DOM?
   - The **Document Object Model** (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects; that way, programming languages can interact with the page.
2. Briefly describe the relationship between the DOM and JavaScript.
   - JavaScript uses the DOM to access the document and its elements. The DOM is not a programming language, but without it, the JavaScript language wouldn't have any model or notion of web pages, HTML documents, SVG documents, and their component parts. The document as a whole, the head, tables within the document, table headers, text within the table cells, and all other elements in a document are parts of the document object model for that document. They can all be accessed and manipulated using the DOM and a scripting language like JavaScript.
