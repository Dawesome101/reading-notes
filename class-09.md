# Forms and JS Events

## Index

[Home](./README.md)  
[HTML Forms](#html-forms)  
[Learn JS](#learn-js)  

## [HTML Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms)

- [Your first Web Form](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form)
- [How To Structure A Web Form](https://developer.mozilla.org/en-US/docs/Learn/Forms/How_to_structure_a_web_form)

1. Why are forms so important in web development?
   - Web forms are one of the main points of interaction between a user and a web site or application. Forms allow users to enter data, which is generally sent to a web server for processing and storage, or used on the client-side to immediately update the interface in some way (for example, add another item to a list, or show or hide a UI feature). A web form's HTML is made up of one or more form controls (sometimes called widgets), plus some additional elements to help structure the overall form — they are often referred to as HTML forms.
   - The controls can be:
     - Single or multi-line text fields
     - Dropdown boxes
     - Buttons
     - Checkboxes
     - Radio buttons
   - These are mostly created using the [\<input\>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input) element, although there are some other elements to learn about too.
2. When designing a form, what are some key things to keep in mind when it comes to user experience?
   - Before starting to code, it's always better to step back and take the time to think about your form.
   - Designing a quick mockup will help you to define the right set of data you want to ask your user to enter.
   - From a user experience (UX) point of view, it's important to remember that the bigger your form, the more you risk frustrating people and losing users.
   - Keep it simple and stay focused: **ask only for the data you absolutely need**.
3. List 5 form elements and explain their importance.
   1. [\<form\>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form) The `<form>` HTML element represents a document section containing interactive controls for submitting information.
   2. [\<label\>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/label) The `<label>` HTML element represents a caption for an item in a user interface.
   3. [\<input\>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input) The `<input>`HTML element is used to create interactive controls for web-based forms in order to accept data from the user; a wide variety of types of input data and control widgets are available, depending on the device and user agent. The `<input>` element is one of the most powerful and complex in all of HTML due to the sheer number of combinations of input types and attributes.
   4. [\<textarea\>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/textarea) The `<textarea>` HTML element represents a multi-line plain-text editing control, useful when you want to allow users to enter a sizeable amount of free-form text, for example a comment on a review or feedback form.
   5. [\<button\>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/button)The `<button>` HTML element is an interactive element activated by a user with a mouse, keyboard, finger, voice command, or other assistive technology. Once activated, it then performs a programmable action, such as submitting a [form](https://developer.mozilla.org/en-US/docs/Learn/Forms) or opening a dialog.

## [Learn JS](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)

- [Introduction To Events](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

1. How would you describe events to a non-technical friend?
   - Events in programming are like the idea of paying attention to something until it does what you are expecting.  For example, when a door closes.  You can use this to build functional things, like say "activate the door lock" when the door closes. etc.
2. When using the `addEventListener()` method, what 2 arguments will you need to provide?
   1. `type` A case-sensitive string representing the [event type](https://developer.mozilla.org/en-US/docs/Web/Events) to listen for.
   2. `listener` The object that receives a notification (an object that implements the [Event](https://developer.mozilla.org/en-US/docs/Web/API/Event) interface) when an event of the specified type occurs. This must be `null`, an object with a `handleEvent()` method, or a JavaScript [function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions). See The [event listener callback](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener#the_event_listener_callback) for details on the callback itself.
3. Describe the event object. Why is the target within the event object useful?
   - An event object is intended to pass information back to the handler. This enables it to provide extra features and information. The `target` is useful because it's always pointing back at the elemnt the event occured upon. This is helpful for us to focus our code to get the results we want.
4. What is the difference between event bubbling and event capturing?
   - Capturing phase:
     - The browser checks to see if the element's outer-most ancestor (`<html>`) has a click event handler registered on it for the capturing phase, and runs it if so.
     - Then it moves on to the next element inside `<html>` and does the same thing, then the next one, and so on until it reaches the direct parent of the element that was actually clicked.
   - Bubbling phase:
     - The browser checks to see if the direct parent of the clicked element has a `click` event handler registered on it for the bubbling phase, and runs it if so.
     - Then it moves on to the next immediate ancestor element and does the same thing, then the next one, and so on until it reaches the `<html>` element.

[Back to Top](#index)
