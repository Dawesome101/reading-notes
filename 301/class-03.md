# Passing Functions as Props

## Index

[Home](../README.md)  
[React Docs - lists and keys](#react-docs--lists-and-keys)  
[The Spread Operator](#the-spread-operator)  

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

[Back To Top](#index)
