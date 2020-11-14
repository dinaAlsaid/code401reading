# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-19) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-27)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. Name 5 Javascript UI Frameworks (other than React).  

* Ext JS
* Angular
* Vue
* Ember
* Svelte 3

2. What’s the difference between a framework and a library?

a Library is a collections of packages. It’s purpose is to offer a set of functionalities ready to use without worrying about the subsequent packages.  
a Framework is a set of libraries. it also provides an architecture for the development work. In other words you don’t include a framework. You integrate you code into it.

## Terms

Rendering: displaying an element.
Templates: s a generic class or other unit of source code that can be used as the basis for unique units of code.  
State: represented as subclasses implementing a common interface (each method in this interface corresponds to an event).

## React

React is a JavaScript library.  
JSX (JavaScript XML) is a syntax extension to JavaScript.It produces React elements.  

```javascript
const element = <h1>Hello, world!</h1>;
```

After compilation, JSX expressions become regular JavaScript function calls and evaluate to JavaScript objects.
If a tag is empty, you may close it immediately with />.  
Elements are the smallest building blocks of React apps, it describes what you see on the screen.  
React elements are immutable. Once you create an element, you can’t change its children or attributes.  
