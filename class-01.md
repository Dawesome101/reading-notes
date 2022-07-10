# Index
##### [HOME](./README.md)  
##### [_What is The Web_](#what-is-the-web-1)  
##### [_Getting Started_](#getting-started-1)
##### [_Introduction to HTML_](#introduction-to-html-1)
##### [_Miscellaneous_](#miscellaneous-1)
##### [_Side Notes_](#side-notes-1)
##### [_Website Development Tools_](#website-development-tools-1)
##### [_Website Design Tools_](#website-design-tools-1)

# [What is the Web](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web)
- [How does the Internet Work](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/How_does_the_Internet_work)  
  - [8 Minute Video of How it Works](https://www.youtube.com/watch?v=x3c1ih2NJEg)
![Simplified diagram of how the internet works](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works/simple-client-server.png)
- [What is HTML](https://developer.mozilla.org/en-US/docs/Glossary/HTML)
  - HTML (HyperText Markup Language) is a descriptive language that specifies webpage structure. 
  - At its heart, HTML is a language made up of elements, which can be applied to pieces of text to give them different meaning in a document (Is it a paragraph? Is it a bulleted list? Is it part of a table?), structure a document into logical sections (Does it have a header? Three columns of content? A navigation menu?), and embed content such as images and videos into a page.
- [What is JavaScript](https://developer.mozilla.org/en-US/docs/Glossary/JavaScript)
  - JavaScript (or "JS") is a programming language used most often for dynamic client-side scripts on webpages, but it is also often used on the server-side, using a runtime such as Node.js.
  - JavaScript is a programming language that adds interactivity to your website. This happens in games, in the behavior of responses when buttons are pressed or with data entry on forms; with dynamic styling; with animation, etc.
- [What is CSS](https://developer.mozilla.org/en-US/docs/Glossary/CSS)
  - CSS (Cascading Style Sheets) is a declarative language that controls how webpages look in the browser.
- [What is the DOM \(Document Object Model\)](https://developer.mozilla.org/en-US/docs/Glossary/DOM)
  - The DOM (Document Object Model) is an API that represents and interacts with any HTML or XML document. The DOM is a document model loaded in the browser and representing the document as a node tree, where each node represents part of the document (e.g. an element, text string, or comment).
- [What is an API](https://developer.mozilla.org/en-US/docs/Glossary/API) 
  - An API (Application Programming Interface) is a set of features and rules that exist inside a software program (the application) enabling interaction with it through software - as opposed to a human user interface. The API can be seen as a simple contract (the interface) between the application offering it and other items, such as third party software or hardware.

# [Getting Started](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started)
1. Compose a short poem describing how HTTP sends data between computers.
   - Hungry for cake? Find a place that will bake, then travel to its location.  
   Ready to buy, just ask the guy(or girl) for a cake to quench your satiation.  
   Baker gets busy, bakes a cake thats the shizzy, then you take it back to your place.  
   Having arrived, cut the cake to divide and stuff it into your face.
   
2. Describe how HTML, CSS, and JS files are “parsed” in the browser. 
   - The browser parses the HTML file first, and that leads to the browser recognizing any <link>-element references to external CSS stylesheets and any \<script\>-element references to scripts.
   - As the browser parses the HTML, it sends requests back to the server for any CSS files it has found from <link> elements, and any JavaScript files it has found from \<script\> elements, and from those, then parses the CSS and JavaScript.
   - The browser generates an in-memory DOM tree from the parsed HTML, generates an in-memory CSSOM structure from the parsed CSS, and compiles and executes the parsed JavaScript.
   - As the browser builds the DOM tree and applies the styles from the [CSSOM](https://developer.mozilla.org/en-US/docs/Glossary/CSSOM) tree and executes the JavaScript, a visual representation of the page is painted to the screen, and the user sees the page content and can begin to interact with it.

3. How can you find images to add to a Website?
   - [Google Images](https://images.google.com/)
     - Note that most images on the web, including in Google Images, are copyrighted. To reduce your likelihood of violating copyright, you can use Google's license filter. Click on the Tools button, then on the resulting Usage rights option that appears below. You should choose the option Creative Commons licenses.

4. How do you create a String vs a Number in JavaScript?
   - To signify that the value is a string, enclose it in single quote marks. __let myVariable = 'Bob';__
   - Numbers do not have quotes. __let myVariable = 10;__

5. What is a Variable and why are they important in JavaScript?
   - Variables are containers that store values. Variables are necessary to do anything interesting in programming. If values couldn't change, then you couldn't do anything dynamic, like personalize a greeting message or change an image displayed in an image gallery.

# [Introduction to HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML)
1. What is an HTML attribute?
   - An [attribute](https://developer.mozilla.org/en-US/docs/Glossary/Attribute) extends an HTML or XML element, changing its behavior or providing metadata.
![Image of an Attribute](https://user-images.githubusercontent.com/107971336/178159431-f6a57894-2728-47c7-89a7-93df16c53fd4.png)

2. Describe the Anatomy of an HTML element.
   - **Opening tag, Content, Closing Tag** _or described another way as_ **Opening tag, An attribute and its value, Enclosed text content, Closing tag**.  
  ![Anatomy of an HTML Element](https://developer.mozilla.org/en-US/docs/Glossary/Element/anatomy-of-an-html-element.png)  
  ![Anatomy of an HTML Element](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started/grumpy-cat-small.png)
  
3. What is the Difference between \<article\> and \<section\> element tags?
   - [\<article\>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/article) encloses a block of related content that makes sense on its own without the rest of the page (e.g., a single blog post). 
   - [\<section\>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/section) is similar to \<article\>, but it is more for grouping together a single part of the page that constitutes one single piece of functionality (e.g., a mini map, or a set of article headlines and summaries), or a theme. It's considered best practice to begin each section with a heading; also note that you can break <article>s up into different \<section\>s, or \<section\>s up into different \<article\>s, depending on the context.

4. What Elements does a “typical” website include?
   - [Header](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/header)
   - [Navigation Bar](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav)
   - [Main Content](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/main)
     - [Article](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/article)
     - [Section](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/section)
     - [Div](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/div)
   - [Sidebar](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/aside)
   - [Footer](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/footer)
  
5. How does metadata influence Search Engine Optimization?
  - [Search Engine Optimization or SEO](https://developer.mozilla.org/en-US/docs/Glossary/SEO)
  - Specifying a description that includes keywords relating to the content of your page is useful as it has the potential to make your page appear higher in relevant searches performed in search engines.
  
6. How is the \<meta\> HTML tag used when specifying metadata?
   - Metadata is data about the HTML, such as the author, and important keywords that describe the document. 
   - [\<meta\>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta) is an HTML element represents metadata that cannot be represented by other HTML meta-related elements, like \<base\>, \<link\>, \<script\>, \<style\> or \<title\>.

## Miscellaneous

[How to start to design a Website](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Thinking_before_coding)
1. What is the first step to designing a Website?
   - Planning, before doing anything, you need some ideas. What should your website actually do?
2. What is the most important question to answer when designing a Website?
   - What is it you want to accomplish.
     - What is your website about? Do you like dogs, New York, or Pac-Man?
     - What information are you presenting on the subject? Write a title and a few paragraphs and think of an image you'd like to show on your page.
     - What does your website look like, in simple high-level terms? What's the background color? What kind of font is appropriate: formal, cartoony, bold and       loud, subtle?
  
[Semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)
1. Why should you use an \<h1\> element over a \<span\> element to display a top level heading?
   - By default, most browser [user agent stylesheets](https://developer.mozilla.org/en-US/docs/Web/CSS/Cascade#user-agent_stylesheets) apply semantic value to \<h1\> giving it a large font size to make it look like a heading (although you could style it to look like anything you wanted) whereas \<span\> is a generic element that carries no semantic value without explicitly defining it with attributes.
2. What are the benefits of using semantic tags in our HTML?
   - Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO).
   - Screen readers can use it as a signpost to help visually impaired users navigate a page.
   - Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes.
   - Suggests to the developer the type of data that will be populated.
   - Semantic naming mirrors proper custom element/component naming.

[What is JavaScript?](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript)
1. Describe 2 things that require JavaScript in the Browser?
   - **A clock:** Displaying timely content updates
   - **Google Maps:** Interactive maps
   - animated 2D/3D graphics
   - **YouTube:** Scrolling video jukeboxes
2. How can you add JavaScript to an HTML document?
- JavaScript is applied to your HTML page in a similar manner to CSS. Whereas CSS uses \<link\> elements to apply external stylesheets and \<style\> elements to apply internal stylesheets to HTML, JavaScript only needs one friend in the world of HTML — the <script> element. Let's learn how this works.
   - Internal JavaScript \- Using the \<script\> element without a source attribute inside the \<head\> tag.
   - External JavaScript \- Using the \<script\> element without with a source attribute (example: src="script.js") inside the \<head\> tag.

#### Side Notes
- Tags in HTML are not case-sensitive. This means they can be written in uppercase or lowercase. However, it is best practice to write all tags in lowercase for consistency and readability.
- Block vrs inline elements
  - [Block-level](https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements) elements form a visible block on a page. 
    - A block-level element always starts on a new line and takes up the full width available (stretches out to the left and right as far as it can).
  - [Inline](https://developer.mozilla.org/en-US/docs/Web/HTML/Inline_elements) elements are those which only occupy the space bounded by the tags defining the element, instead of breaking the flow of the content.
    - An inline element does not start on a new line and only takes up as much width as necessary. 
- Elements can be placed within other elements. This is called nesting.
- Empty elements are sometimes called _void_ elements.
- Double quotes or single quotes around an attribute?  The only difference is style so it doesn't matter but consistency is important for readability.
  
#### Website Development Tools
   - [Browser Dev Tools](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_browser_developer_tools)
   - [Basic Software](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/Installing_basic_software)
   - [How to Setup a Local Testing Web Server](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/set_up_a_local_testing_server)

#### Website Design Tools
   - Design
     - [Photon](https://design.firefox.com/photon/)
     - [Wireframe](https://wireframe.cc/)
     - [Free Online Tools for Developers](https://www.freeformatter.com/)
   - Colors  
     - [CSS Colors Info](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value) 
     - [Color Generator](https://coolors.co/generate)
     - [Google RGB Color Picker](https://www.google.com/search?q=rgb+color+picker)
   - Fonts
     - [Google Fonts](https://fonts.google.com/)
     - [Google Fonts API](https://developers.google.com/fonts/docs/getting_started)
   - Debug & Testing
     - [Browser support tables for modern web technologies](https://caniuse.com/)
   - Cheat Sheets
     - [List of HTML entities](https://www.freeformatter.com/html-entities.html)
     - [HTML Living Standard](https://html.spec.whatwg.org/multipage/indices.html#element-content-categories)
  
  ##### [Back to Top](#index)
