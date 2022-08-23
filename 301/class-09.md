# Functional Programming

## Index

[Home](../README.md)  
[Functional Programming Concepts](#functional-programming-concepts)  
[Node JS Tutorial for Beginners - Modules and Require()](#node-js-tutorial-for-beginners---modules-and-require)

[Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

1. What is functional programming?
   - Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data - Wikipedia
2. What is a pure function and how do we know if something is a pure function?
   - It returns the same result if given the same arguments (it is also referred as deterministic)
   - It does not cause any observable side effects
3. What are the benefits of a pure function?
   - Easier to test
4. What is immutability?
   - Unchanging over time or unable to be changed. When data is immutable, **its state cannot change after it’s created.**
5. What is Referential transparency?
   - Basically, if a function consistently yields the same result for the same input, it is referentially transparent.
   - `pure functions + immutable data = referential transparency`

[Node JS Tutorial for Beginners - Modules and Require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

1. What is a module?
   - Snipits of single functions/behaviors.  Small bits of codues that are simply small javascript files.
2. What does the word ‘require’ do?
   - Essentially it imports in another file
3. How do we bring another module into the file the we are working in?
   - `var variable = require('./file');`
4. What do we have to do to make a module available?
   - `module.exports = function;`

[Back To Top](#index)
