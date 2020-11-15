# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-26) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-28)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. Does a deployed React application require a server?
nope  
2. Why do we prefer to test a React application at the behavior rather than the unit level?
because it depends on the states where it needs to compare the DOM and the Virtual/React DOM and that can't be done in isolation (isolating tested components).
3. What does npm run build do?
It correctly bundles React in production mode and optimizes the build for the best performance.  
4. Describe the actual composition / architecture of a React application

## Term

BDD: behavior Driven Development.a process that encourages collaboration among developers, QA and non-technical or business participants in a software project  
Acceptance Tests:The purpose of this test is to evaluate the system’s compliance with the business requirements and assess whether it is acceptable for delivery  
mounting: process by which the operating system makes files and directories on a storage device available for users to access via the computer's file system. in react it happens when the component is first rendered.
build  

## Lfecycle methods

special methods on the component class to run some code when a component mounts and unmounts.  
`componentDidMount()` method runs after the component output has been rendered to the DOM.  
on a `setState()` call, React knows the state has changed, and calls the render() method again.  
if component is removed from the DOM, React calls the `componentWillUnmount()` lifecycle method.  
HTML form elements work a little bit differently from other DOM elements in React, because form elements naturally keep some internal state.  
In React, mutable state is typically kept in the state property of components, and only updated with setState().  
React events are named using camelCase, rather than lowercase  
This function is a valid React component because it accepts a single “props” object argument with data and returns a React element. We call such components “function components” because they are literally JavaScript functions.