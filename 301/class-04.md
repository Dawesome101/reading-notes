# React and Forms

## Index

[Home](../README.md)  
[React Docs - Forms](#react-docs---forms)  
[The Conditional (Ternary) Operator Explained](#the-conditional-ternary-operator-explained)  

## [React Docs - Forms](https://reactjs.org/docs/forms.html)

1. What is a ‘Controlled Component’?
   - In HTML, form elements such as `<input>`, `<textarea>`, and `<select>` typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with `setState()`.  
   We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a **“controlled component”**.  
   For example, if we want to make the previous example log the name when it is submitted, we can write the form as a controlled component:

   ```js
   class NameForm extends React.Component {
      constructor(props) {
         super(props);
         this.state = {value: ''};

         this.handleChange = this.handleChange.bind(this);
         this.handleSubmit = this.handleSubmit.bind(this);
      }

      handleChange(event) {
         this.setState({value: event.target.value});
      }

      handleSubmit(event) {
      alert('A name was submitted: ' + this.state.value);
      event.preventDefault();
      }

      render() {
         return (
            <form onSubmit={this.handleSubmit}>
            <label>
               Name:
               <input type="text" value={this.state.value} onChange={this.handleChange} />
            </label>
            <input type="submit" value="Submit" />
            </form>
         );
      }
   }
   ```

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
   - In the above example, since the `value` attribute is set on our form element, the displayed value will always be `this.state.value`, making the React state the source of truth. Since `handleChange` runs on every keystroke to update the React state, the displayed value will update as the user types.

3. How do we target what the user is entering if we have an event handler on an input field?
   - With a controlled component, the input’s value is always driven by the React state. While this means you have to type a bit more code, you can now pass the value to other UI elements too, or reset it from other event handlers.

## [The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

1. Why would we use a ternary operator?
   - To help write conditional statments in a more concise way.  This can be helpful when looking at the following example taken from [jraleman.medium.com](https://jraleman.medium.com/ternary-operators-vs-if-else-statements-6c26f7d034f7).  
   If statment:

   ```js
   bool y;
   if (x == 42){
      y = true;
   }
   else {
      y = false;
   }
   ```

   Ternary operator:

   ```js
   bool y = (x == 42) ? true : false;
   ```

   The ternary operator is much easier to create and very simple to read.

2. Rewrite the following statement using a ternary statement:

   ```js
   if(x===y){
   console.log(true);
   } else {
   console.log(false);
   }
   ```

   ```js
   console.log((x === y) ? true : false);
   ```

[Back To Top](#index)
