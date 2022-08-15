# Readings: Introductions to React and Components

## Index

[Home](../README.md)  
[Component-Based Architecture](#component-based-architecture)  
[What is Props and How to Use it in React](#what-is-props-and-how-to-use-it-in-react)  

## [Component-Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

1. What is a “component”?
   - A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.  
   A component is a software object, intended to interact with other components, encapsulating certain functionality or a set of functionalities. It has an obviously defined interface and conforms to a recommended behavior common to all components within an architecture.  
   A software component can be defined as a unit of composition with a contractually specified interface and explicit context dependencies only. That is, a software component can be deployed independently and is subject to composition by third parties.
2. What are the characteristics of a component?
   - `Reusability` Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.
   - `Replaceable` Components may be freely substituted with other similar components.
   - `Not context specific` Components are designed to operate in different environments and contexts.
   - `Extensible` A component can be extended from existing components to provide new behavior.
   - `Encapsulated` A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.
   - `Independent` Components are designed to have minimal dependencies on other components.
3. What are the advantages of using component-based architecture?
   - `Ease of deployment` As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.
   - `Reduced cost` The use of third-party components allows you to spread the cost of development and maintenance.
   - `Ease of development` Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.
   - `Reusable` The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.
   - `Modification of technical complexity` A component modifies the complexity through the use of a component container and its services.
   - `Reliability` The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.
   - `System maintenance and evolution` Easy to change and update the implementation without affecting the rest of the system.
   - `Independent` Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

## [What is Props and How to Use it in React](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0#:~:text=%E2%80%9CProps%E2%80%9D%20is%20a%20special%20keyword,way%20from%20parent%20to%20child)

1. What is “props” short for?
   - Properties
2. How are props used in React?
   - Passing data from one component to another.
3. What is the flow of props?
   - Firstly, define an attribute and its value(data)  
     - We can define our own attributes & assign values with interpolation { }:

   ```html
   <ChildComponent someAttribute={value} anotherAttribute={value}/>
   ```

   - Then pass it to child component(s) by using Props  
     - Arguments passed to a function:

     ```js
     const addition = (firstNum, secondNum) => {  
     return firstNum + secondNum; 
     };
     ```

     - Arguments passed to a React component:

     ```js
     const ChildComponent = (props) => {  
     return <p>I'm the 1st child!</p>; 
     };
     ```

   - Finally, render the Props Data
     - Render a text property with an interpolation:

     ```js
     const ChildComponent = (props) => {  
     return <p>{props.text}</p>; 
     };
     ```

     ```js
     class ParentComponent extends Component {  
       render() {
         return (
           <h1>
             I'm the parent component.
             <ChildComponent text={"I'm the 1st child"} />
             <ChildComponent text={"I'm the 2nd child"} />
             <ChildComponent text={"I'm the 3rd child"} />
           </h1>
         );
       }
     }
     ```

4. RECAP
   - Props stand for properties and is a special keyword in React
   - Props are being passed to components like function arguments
   - Props can only be passed to components in one way (parent to child)
   - Props data is immutable (read-only)

[Back To Top](#index)
