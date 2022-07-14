# HTML Links, JS Functions and Intro to CSS Layout

## Index

[HOME](./README.md)  
[Learn HTML](#learn-html)

- [Creating Hyperlinks](#creating-hyperlinks)

[CSS Layout](#css-layout)

- [CSS Layout: Normal Flow](#css-layout-normal-flow)
- [CSS Layout: Positioning](#css-layout-positioning)

[Learn JS](#learn-js)

- [Functions - Reusable Blocks of Code](#functions---reusable-blocks-of-code)

[Miscellaneous](#miscellaneous)

- [6 Reasons for Pair Programming](#6-reasons-for-pair-programming)

## [Learn HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML)

### [Creating Hyperlinks](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks)

1. To create a basic link, we wrap text or other content inside what element?
   - The `<a>` HTML element (or anchor element), with its `href` attribute, creates a hyperlink to web pages, files, email addresses, locations in the same page, or anything else a URL can address.
2. The `href` attribute contains what information?
   - The URL that the hyperlink points to. Links are not restricted to HTTP-based URLs — they can use any URL scheme supported by browsers:
   - Sections of a page with fragment URLs
   - Pieces of media files with media fragments
   - Telephone numbers with `tel:` URLs
   - Email addresses with `mailto:` URLs
   - While web browsers may not support other URL schemes, web sites can with `registerProtocolHandler()`
3. What are some ways we can ensure links on our pages are accessible to all readers?
   - Screen reader users like jumping around from link to link on the page, and reading links out of context.
   - Search engines use link text to index target files, so it is a good idea to include keywords in your link text to effectively describe what is being linked to.
   - Visual readers skim over the page rather than reading every word, and their eyes will be drawn to page features that stand out, like links. They will find descriptive link text useful.
   - Don't repeat the URL as part of the link text — URLs look ugly, and sound even uglier when a screen reader reads them out letter by letter.
   - Don't say "link" or "links to" in the link text — it's just noise. Screen readers tell people there's a link. Visual users will also know there's a link, because links are generally styled in a different color and underlined (this convention generally shouldn't be broken, as users are used to it).
   - Keep your link text as short as possible — this is helpful because screen readers need to interpret the entire link text.
   - Minimize instances where multiple copies of the same text are linked to different places. This can cause problems for screen reader users, if there's a list of links out of context that are labeled "click here", "click here", "click here".

### Additional Notes

- Another attribute you may want to add to your links is `title`. The `title` contains additional information about the link, such as which kind of information the page contains, or things to be aware of on the website. **This gives us the following result and hovering over the link displays the title as a tooltip.**

## [CSS Layout](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout)

### [CSS Layout: Normal Flow](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Normal_Flow)

1. What is meant by “normal flow”?
   - Normal Flow, or Flow Layout, is the way that Block and Inline elements are displayed on a page before any changes are made to their layout. The flow is essentially a set of things that are all working together and know about each other in your layout. Once something is taken out of flow it works independently.
2. What are a few differences between block-level and inline elements?
   - By default, a **block level** element's content fills the available inline space of the parent element containing it and grows along the block dimension to accommodate its content.
   - The size of **Inline elements** is just the size of their content. You can't set width or height on inline elements — they just sit inside the content of block level elements.
     - If you want to control the size of an inline element in this manner, you need to set it to behave like a block level element (e.g., with `display: block;` or `display: inline-block;`, which mixes characteristics from both).

### [CSS Layout: Positioning](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning)

1. ___ positioning is the default for every html element.
   - **Static** positioning is the default that every element gets. It just means "put the element into its normal position in the document flow — nothing special to see here."
2. Name a few advantages to using absolute positioning on an element.
   - we can create isolated UI features that don't interfere with the layout of other elements on the page.
     - Popup information boxes
     - Control menus
     - Rollover panels
     - UI features that can be dragged and dropped anywhere on the page
3. What is a key difference between fixed positioning and absolute positioning?
   - **Absolute positioning** fixes an element in place relative to its nearest positioned ancestor (the initial containing block if there isn't one), **fixed positioning** usually fixes an element in place relative to the visible portion of the viewport. (An exception to this occurs if one of the element's ancestors is a fixed containing block because its transform property has a value other than none.) This means that you can create useful UI items that are fixed in place, like **persistent navigation menus that are always visible no matter how much the page scrolls.**

## [Learn JS](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)

### [Functions - Reusable Blocks of Code](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Functions)

1. Describe the difference between a function declaration and a function invocation.
   - Fuction declaration is creating a function.
   - Function invocation is calling or invoking the fuction to run.
2. What is the difference between a parameter and an argument?
   - Parameters are variables used in a functions definition.

   ```C#
   private void Foo(string myParameter) {}
   ```

   - Arguments are variables passed into a functions parameters.

   ```C#
   string myArgument = "Argument";
   myClass.FOO(myArgument);
   ```

## Miscellaneous

### [6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

1. Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey.
   - Learning from fellow students
     - Something I've picked up over time is that people often interperate information and derived meaning differently.  That is not to say that one interpretation is more correct than the other, but that the understandings we reach are often relative.  Pairing up with people helps me to see problems from angles I wouldn't normally be able to on my own.
   - Job interview readiness
     - Job interviews almost always require showing off your ability to do the job.  Some places even want to pair you up with employees to see if you fit the culture.  Pair programming gets you aclimated and even used to being able to be focused and productive with other people watching exactly what it is that you do.  This builds confidence and understand for one another.  More often then not, people will build healthy work relationships by working together and pair programming is a solid way to achive just that.
