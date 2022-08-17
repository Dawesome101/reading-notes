# Passing Functions as Props

## Index

[Home](../README.md)  
[React Docs - lists and keys](#react-docs--lists-and-keys)  
[The Spread Operator](#the-spread-operator)  
[How to Pass Functions Between Components](#how-to-pass-functions-between-components)  

## [React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)

1. What does `.map()` return?
   - It itterates over an array and returns a new array of the same size.
2. If I want to loop through an array and display each value in JSX, how do I do that in React?

    ```js
    const numbers = [1, 2, 3, 4, 5];
    const listItems = numbers.map((number) =>
      <li>{number}</li>
    );

    <ul>{listItems}</ul>
    ```

3. Each list item needs a unique ____.
   - `key`
4. What is the purpose of a key?
   - Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside an array to give the elements a stable identity

## [The spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

1. What is the spread operator?
   - The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.
2. List 4 things that the spread operator can do.
   - Copying an array
   - Concatenating or combining arrays
   - Using Math functions
   - Using an array as arguments
   - Adding an item to a list
   - Adding to state in React
   - Combining objects
   - Converting NodeList to an array
3. Give an example of using the spread operator to combine two arrays.

    ```js
    const foo = ['f', 'o', 'o']
    const bar = {'b', 'a', 'r'}
    const foobar = {...foo, ...bar}
    console.log(foobar) //foobar
    ```

4. Give an example of using the spread operator to add a new item to an array.

    ```js
    const stuff = ['ninja star', 'katana']
    const moreStuff = ['ninjato', 'nunchaku', ...stuff]
    console.log(moreStuff) //['ninjato', 'nunchaku','ninja star', 'katana']
    ```

5. Give an example of using the spread operator to combine two objects into one.

    ```js
    const super {super: 'super'}
    const foo {foo: 'foo'}
    const bar {...super, ...foo, bar: 'bar'}
    const superFooBar {...super, ...foo, bar: () => {console.log('bar'.repeat(5))}}
    superFooBar.bar() //barbarbarbarbar
    ```

## [How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

1. In the video, what is the first step that the developer does to pass functions between components?
   - Create a function where ever the state is that you're going to change.
2. In your own words, what does the increment function do?
   - It creates a new arry out of state `people: \[a,b,c,d,e\]` by looping through it using the map method.  Each iteration, it checks `.name` to see if it's equal to the name passed into the increment function.  If it is the name passed into the increment function, then it increments the count: `value` by one.
3. How can you pass a method from a parent component into a child component?
   - First you'll need to make a object and store the method `object={this.myMethod}` From inside the child, you create a constructor `constructor(props)` and call `super(props)` to get access to all the properties of its parrent.  Then you can access it using the this keyword. `this.props.myMethod(pass in value here)`
4. How does the child component invoke a method that was passed to it from a parent component?
   - `this.props.myMethod(pass in value here)`

[Back To Top](#index)
