# In Memory Storage

## Index

[Home](../README.md)  

[Understanding the JavaScript Call Stack](#understanding-the-javascript-call-stack)  
[JavaScript Error Messages](#javascript-error-messages)  

## [Understanding the JavaScript Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)

1. What is a ‘call’?
   - Function invocation
2. How many ‘calls’ can happen at once?
   - In V8, the number of recursive calls you can make depends on two quantities: the size of the stack and the size of the stack frame (holding parameters and local variables).
3. What does LIFO mean?
   - Last in First Out
   - ![Callstack](../img/CallStack.png)
4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

   ```js
   function firstFunction(){
      console.log("Hello from firstFunction");
   }

   function secondFunction(){
      firstFunction();
      console.log("The end from secondFunction");
   }

   secondFunction();
   ```

5. What causes a Stack Overflow?
   - A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

## [JavaScript Error Messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

1. What is a ‘reference error’?
   - This is as simple as when you try to use a variable that is not yet declared you get this type os errors.
   `console.log(foo) // Uncaught ReferenceError: foo is not defined`
2. What is a ‘syntax error’?
   - This occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.
   - `JSON.parse( {'foo': 'bar'} ) // Uncaught SyntaxError: Unexpected token o in JSON at position 1`
3. What is a ‘range error’?
   - Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

   ```js
   var foo= []
   foo.length = foo.length -1 // Uncaught RangeError: Invalid array length
   ```

4. What is a ‘tyep error’?
   - this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

   ```js
   var foo = {}
   foo.bar // undefined
   foo.bar.baz // Uncaught TypeError: Cannot read property 'baz' of undefined
   ```

5. What is a breakpoint?
   - A break point is a point set in your code to have it pause execution which you can then step through one line at a time.
6. What does the word ‘debugger’ do in your code?
   - The breakpoint can also be achieved by putting a `debugger` statement in your code in the line you want to break.

[Back To Top](#index)