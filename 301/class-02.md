# State and Props

## Index

[Home](../README.md)  
[React Lifecycle](#react-lifecycle)  
[React State Vs Props](#ract-state-vs-props)  

## [React Lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
   - Render
2. What is the very first thing to happen in the lifecycle of React?
   - Mounting
3. Put the following things in the order that they happen: `componentDidMount`, `render`, `constructor`, `componentWillUnmount`, `React Updates`
   - Constructor, render, react updates, componentDidMount, componentWillUnmount
4. What does `componentDidMount` do?
   - [componentDidMount](https://reactjs.org/docs/react-component.html#componentdidmount) is invoked immediately after a compenet is mounted and is a good place to load anything using network requests or initialize the DOM.

## [React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

1. What types of things can you pass in the props?
   - arguments, any value you want to pass into a component/function.
2. What is the big difference between props and state?
   - Props you pass in and can only be updated outside of the component, state is handled inside a component and can be updated inside the component.
3. When do we re-render our application?
   - When you want to change something displayed in the application (usualy based on user input).
4. What are some examples of things that we could store in state?
   - Form data, counters, dynamic statistics (example: changing stockmarket info, weather conditions, etc.)

[Back To Top](#index)
