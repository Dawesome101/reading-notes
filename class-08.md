# CSS Layout

## Index

[Home](./README.md)  
[Learn CSS - Flexbox](#learn-css---flexbox)  
[CSS Layout - Flexbox](#css-layout---flexbox)

## [Learn CSS - Flexbox](https://web.dev/learn/css/flexbox/)

1. Flexbox is designed for one-dimensional content. Explain what this means.
   - The Flexible Box Layout Model (flexbox) is a layout model designed for one-dimensional content. It excels at taking a bunch of items which have different sizes, and returning the best layout for those items.
   - Flex layouts have the following features, which you will be able to explore in this guide.
     - They can display as a row, or a column.
     - They respect the writing mode of the document.
     - They are single line by default, but can be asked to wrap onto multiple lines.
     - Items in the layout can be visually reordered, away from their order in the DOM.
     - Space can be distributed inside the items, so they become bigger and smaller according to the space available in their parent.
     - Space can be distributed around the items and flex lines in a wrapped layout, using the Box Alignment properties.
     - The items themselves can be aligned on the cross axis.
2. Explain the difference between the main axis and cross axis.
   - Flex items move as a group on the main axis. We are trying to get the best layout for a group. The cross axis runs in the other direction to the main axis, so if `flex-direction` is `row` the cross axis runs along the column.
3. How can using certain properties of flexbox negatively impact accessibility?
   - You should be cautious when using any properties that reorder the visual display away from how things are ordered in the HTML document, as it can negatively impact accessibility. The row-reverse and column-reverse values are a good example of this. The reordering only happens for the visual order, not the logical order. This is important to understand as the logical order is the order that a screen reader will read out the content, and anyone navigating using the keyboard will follow. You can see in the [following video](https://storage.googleapis.com/web-dev-uploads/video/VbAJIREinuYvovrBzzvEyZOpw5w1/IgpaIRZd7kOq8sd46eaR.mp4)  how in a reversed column layout, tabbing between links becomes disconnected as the keyboard navigation follows the DOM not the visual display. [**source**](https://web.dev/learn/css/flexbox/#reversing-the-flow-of-items-and-accessibility)

## [CSS Layout - Flexbox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)

1. What are some advantages of using flexbox over float?
   - Vertically centering a block of content inside its parent.
   - Making all the children of a container take up an equal amount of the available width/height, regardless of how much width/height is available.
   - Making all columns in a multiple-column layout adopt the same height even if they contain a different amount of content.
2. How does this topic connect with your long term goals?
   - Have a sleek and stylish website created with fluid design principles is a great way to easily show off your tallent with HTML, CSS and possibly even JS. Additionally, I may want to help some folks out or even take contracts where I'll need these skills to be sharp as a knife.  Plus, responsive design is awesome and looks cool.

[Back to Top](#index)
