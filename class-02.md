# Basics of HTML, CSS and JS

## Index

[Home](./README.md)

[Introduction to HTML (Cont.)](#introduction-to-html-cont-1)

[Learn CSS](#learn-css-1)

[Learn JS](#learn-js-1)

[Things I want to know more about](#things-i-want-to-know-more-about-1)

## Introduction to HTML (Cont.)

### [HTML text fundamentals](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals) and [Advanced text formatting](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting)

1. Why is it important to use semantic elements in our HTML?
   - SEO, Screen readers, expected behaviors.  We need to make sure we are using the correct elements, giving our content the correct meaning, function, or appearance.
2. How many levels of headings are there in HTML?
   - There are six heading elements: `<h1>` `<h2>` `<h3>` `<h4>` `<h5>` and `<h6>`. Each element represents a different level of content in the document; `<h1>` represents the main heading, `<h2>` represents subheadings, `<h3>` represents sub-subheadings, and so on.
   - Preferably, you should use a single `<h1>` per page.
   - Of the six heading levels available, you should aim to use no more than three per page. It is advisable to spread the content over multiple pages if possible.
3. What are some uses for the `<sup>` and `<sub>` elements?
   - Dates, chemical formulae, and mathematical equations are a few examples.
4. When using the `<abbr>` element, what attribute must be added to provide the full expansion of the term?
   - The `title` attribute.

## Learn CSS

### [How CSS is Structured](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_is_structured)

1. What are ways we can apply CSS to our HTML?
   - External stylesheet `<link rel="stylesheet" href="style.css">`.
      - Inside a subdirectory called styles inside the current directory `<link rel="stylesheet" href="styles/style.css">`
      - Inside a subdirectory called general, which is in a subdirectory called styles, inside the current directory `<link rel="stylesheet" href="styles/general/style.css">`
      - Go up one directory level, then inside a subdirectory called styles `<link rel="stylesheet" href="../styles/style.css">`
   - Internal stylesheets

      ```html
      <head>
         <meta charset="utf-8">
         <title>My CSS experiment</title>
         <style>
         h1 {
            color: blue;
            background-color: yellow;
            border: 1px solid black;
         }

         p {
            color: red;
         }
         </style>
      </head>
      ```  

   - Inline stylesheets
      - `<h1 style="color: blue;background-color: yellow;border: 1px solid black;">Hello World!</h1>` or `<p style="color:red;">This is my first CSS example</p>`
2. Why should we avoid using inline styles?
   - First, it is the least efficient implementation of CSS for maintenance. One styling change might require multiple edits within a single web page. Second, inline CSS also mixes (CSS) presentational code with HTML and content, making everything more difficult to read and understand. Separating code and content makes maintenance easier for all who work on the website.
3. Review the block of code below and answer the following questions:

```css
      h2 {
   color: black;
   padding: 5px;
}
```

1. What is representing the selector?
   - `h2`
2. Which components are the CSS declarations?
   - `color: black;`
   - `padding: 5px;`
3. Which components are considered properties?
   - `color`
   - `padding`

## Learn JS

1. What data type is a sequence of text enclosed in single quote marks?
   - `string`
2. List 4 types of JavaScript operators.
   - `+`
   - `-` `*` `/`
   - `=`
   - `===`
   - `!` `!==`
3. Describe a real world Problem you could solve with a Function.
   - Any accounting problem ever.
   - Any mathmatical problem ever.
   - Randomly pick what color icing I want on my cake. but... the cake is a lie.

### [Making Decisions In Your Code - Conditionals](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)

1. An if statement checks a \_\_ and if it evaluates to \_\_\_, then the code block will execute.
   - condition
   - true
2. What is the use of an else if?
   - It is used to test a specified condition, if it is true, run A, if false, run B.
3. List 3 different types of comparison operators.
   - `===` Strict equality
   - `!==` Strict-non-equality
   - `>` Greater than
   - `<` Less than
   - `<=` Less than or equal to
   - `>=` Greater than or equal to
4. What is the difference between the logical operator `&&` and `||`?
   - `&&` AND; allows you to chain together two or more expressions so that all of them have to individually evaluate to true for the whole expression to return true.
   - `||` OR; allows you to chain together two or more expressions so that one or more of them have to individually evaluate to true for the whole expression to return true.

## Things I want to know more about

- When if ever is it ok to use inline styles?

[Back to Top](#basics-of-html-css-and-js)
