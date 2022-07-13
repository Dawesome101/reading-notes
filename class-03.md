# HTML Lists, Control Flow with JS and the CSS Box Model

## Index

[Home](./README.md)  
[Learn HTML](#learn-html-1)  
[Learn CSS](#learn-css-1)  
[Learn JS](#learn-js-1)  

## [Learn HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)

1. [Unordered Lists](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul)
   - When should you use an unordered list in your HTML document?
     - The `<ul>` element is for grouping a collection of items that do not have a numerical ordering, and their order in the list is meaningless. Typically, unordered-list items are displayed with a bullet, which can be of several forms, like a dot, a circle, or a square. The bullet style is not defined in the HTML description of the page, but in its associated CSS, using the `list-style-type` property.
   - How do you change the bullet style of unordered list items?
     - `list-style-type` Here are many examples

      ```css
      /* Partial list of types */
      list-style-type: disc;
      list-style-type: circle;
      list-style-type: square;
      list-style-type: decimal;
      list-style-type: georgian;
      list-style-type: trad-chinese-informal;
      list-style-type: kannada;

      /* <string> value */
      list-style-type: '-';

      /* Identifier matching an @counter-style rule */
      list-style-type: custom-counter-style;

      /* Keyword value */
      list-style-type: none;

      /* Global values */
      list-style-type: inherit;
      list-style-type: initial;
      list-style-type: revert;
      list-style-type: revert-layer;
      list-style-type: unset;

      list-style-type: custom name example defined in @counter-style shown below;

      @counter-style thumbs {
            system: cyclic;
            symbols: "\1F44D";
            suffix: " ";
          }

          ul {
            list-style: thumbs;
          }

      ```

      - [For a list of @counter-style discriptors go here](https://developer.mozilla.org/en-US/docs/Web/CSS/@counter-style#descriptors).
2. [Ordered Lists](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol)
   - When should you use an ordered list vs an unorder list in your HTML document?
     - When the order matters:
       - Steps in a recipe
       - Turn-by-turn directions
       - The list of ingredients in decreasing proportion on nutrition information labels

       ```html
       <ol>
         <li>Fee</li>
         <li>Fi</li>
         <li>Fo</li>
         <li>Fum</li>
       </ol>

       ```

   - Describe two ways you can change the numbers on list items provided by an ordered list?
     - `type` Sets the numbering type. Example `<ol type="i">`
       - `a` for lowercase letters
       - `A` for uppercase letters
       - `i` for lowercase Roman numerals
       - `I` for uppercase Roman numerals
       - `1` for numbers (default)

     > Note: Unless the type of the list number matters (like legal or technical documents where items are referenced by their number/letter), use the CSS list-style-type property instead.

## [Learn CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)

- [The Box Model](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)

  1. Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?
     - Margin is my body guard, margin keeps me safe.  Margin always shoves jerks that are getting to close to my personal boundary away!  Margin is my hero.
     - Padding is always telling me to control me feelings and watch what I say.  Padding always wants me to hold things closer to my chest, push away from my outer walls and go inward.  Padding is a tough friend, but I wouldn't make it without padding... and I wouldn't want to.
  2. List and describe the four parts of an HTML elements box as referred to by the box model
     - Extended info on [Margins](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model#margin).
     - **Content box:** The area where your content is displayed; size it using properties like `inline-size` and `block-size` or `width` and `height`.
     - **Padding box:** The padding sits around the content as white space; size it using `padding` and related properties.
     - **Border box:** The border box wraps the content and any padding; size it using `border` and related properties.
     - **Margin box:** The margin is the outermost layer, wrapping the content, padding, and border as whitespace between this box and other elements; size it using `margin` and related properties.

## [Learn JS](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)

- [Arrays](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Arrays), [Operators and Expressions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators), [Conditionals](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals) and [Loops](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Looping_code)
  - What data types can you store inside of an Array?
    - Any data type can be stored in an array.
  - Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?
    - Yes it is valid.
    - There is more than one way to access the data.  For example: `people[1][1];` would return the value "pete".
  
  ```js
  const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];
  ```

  - List five shorthand operators for assignment in javascript and describe what they do.
    - [This](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#assignment_operators) is a link to a list table of the available operators.
    - `&=` **Bitwise And assignment** - The bitwise AND assignment operator (&=) uses the binary representation of both operands, does a bitwise AND operation on them and assigns the result to the variable.
    - `*=` The **multiplication assignment** operator (*=) multiplies a variable by the value of the right operand and assigns the result to the variable.
    - `<<=` The **left shift assignment** operator (<<=) moves the specified amount of bits to the left and assigns the result to the variable.
    - `%=` The **remainder assignment** operator (%=) divides a variable by the value of the right operand and assigns the remainder to the variable.
    - `??=` The **logical nullish assignment** (x ??= y) operator only assigns if x is nullish (null or undefined).

  - Read the code below and evaluate the last expression and explain what the result would be and why.
    - I have no idea.  The page is not clear and I've read it like 50 times.  It's 12:13AM and I dont have the energy to figure this out without having enough information to solve it.
  
  ```js
     let a = 10;
     let b = 'dog';
     let c = false;

     // evaluate this
     (a + c) + b;
  ```

  - Describe a real world example of when a conditional statement should be used in a JavaScript program.
    - If my pants are wet then through them in the dryer, orelse ignore the dryer completely.
  
  - Give an example of when a Loop is useful in JavaScript.
    - Say you wanted to make a 3D voxel game... say like minecraft.  Well, loops would be very useful for just such an ocasion.

[Back to Top](#index)