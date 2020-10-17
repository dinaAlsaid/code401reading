# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-01) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-03)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Classes and inheretance

1. Why would you want to run JavaScript code outside of a browser?

To create a back-end application that will communicate with a database and be able to create a RESTful API (use the get/post/put/delete/patch methods)
2. What is the difference between a module and a package?

A module is smaller than a package.
a module is a set of functions or methods, where a package is a collection of modules.

[ref](https://medium.com/ieee-ensias-student-branch/framework-vs-library-vs-package-vs-module-the-debate-e1013a3e114d)
3. What does the node package manager do?

npm is the world’s largest software registry used to share and install packges, and itcan help run packages without downloading them

[ref](https://docs.npmjs.com/about-npm/index.html)
4. Provide code snippets showing 3 different ways to export a function from a node module

```javascript
module.exports = 'Hello world';
```

```javascript
exports.SimpleMessage = 'Hello world';
```

```javascript
module.exports.SimpleMessage = 'Hello world';
```

[ref](https://www.tutorialsteacher.com/nodejs/nodejs-module-exports)

## Terms

* ecosystem: all the node.js files, packages, server, modules and libraries and the relations between them that help create a fully functional Node app.
* Node.js: JavaScript runtime ( includes everything you need to execute a program) built on Chrome's V8 JavaScript engine.
* V8 Engine: V8 is Google’s open source high-performance JavaScript and WebAssembly engine, written in C++
* module:Is the smallest piece of software. A module is a set of methods or functions ready to be used somewhere else.
* package:a collection of modules that gather a number of modules holding in general the same functional purpose.
* node package manager (npm): npm is the world’s largest software registry used to share and install packages
* server: a piece of computer hardware or software (software in our case) that provides functionality for other programs or devices, called "clients".
* environment: is a base on top of which we can do our programming, where you can define variables to control the conditions at which the program is run.
* interpreter: coverts each high-level program statement, one by one, into the machine code, during program run.
* compiler: transforms code written in a high-level programming language into the machine code, at once, before program runs.

## Context and 'this'

Can be simply described as the value of this pointer. which can refer to an object, the window object or a function.
the context can be changed using three methods (call, apply, bind)

* Inside a function, the value of this depends on how the function is called.
in non strict mode, and because the value of this is not set by the call, this will default to the global object, which is window in a browser.
In strict mode, however, if the value of this is not set when entering an execution context, it remains as undefined.

* in classes and functions is similar, since classes are functions.

## inheretence

When it comes to inheritance, JavaScript only has one construct: objects. Each object has a private property which holds a link to another object called its prototype. That prototype object has a prototype of its own, and so on until an object is reached with null as its prototype. By definition, null has no prototype, and acts as the final link in this prototype chain.
JavaScript does not have "methods" in the form that class-based languages define them. In JavaScript, any function can be added to an object in the form of a property. An inherited function acts just as any other property.
When an inherited function is executed, the value of this points to the inheriting object, not to the prototype object where the function is an own property.
