# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-02) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-04)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. Name 3 advantages to Test Driven Development

Better program design
Code flexibility and easier maintenance
educes the time required for project development
2. In what case would you need to use beforeEach() or afterEach() in a test suite?

BeforeEach runs before each test in the test suite preparing needed data/variables..etc.
afterEach runs after each test in the test suite to reset data or remove data ..etc.
3. What is one downside of Test Driven Development

It takes alot of time and effort and sometimes some cases get left out causing unexpected behaviours.
4. What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?

Syntax
Classes inherit from classes and create subclass relationships (Class inheritance creates parent/child object inherital relations as a side-effect.) where Objects inherit directly from other objects(do not create inherital relations (class taxonomies) as a side-effect ).
5. Name a use case for a static method

to create or clone objects
6. Write an example of a Higher Order function and describe the use case it solves

HO is a higheer order function, used to choose from two functions based on an input

```javascript
function HO (input){
    if(input){
        return function f1 (){//do something}
    } else {
        return function f2 (){//do something}

    }
}
```

## terms

* functional programming: is the process of building software by composing pure functions avoiding shared state, mutable data, and side-effects
* pure function:  a function where the return value is only determined by its input values, without observable side effects.
* higher-order function: functions that take other functions as arguments or return functions as their results.
* immutable state:state of an object that cannot be modified after it is created
* object: a collection of properties and methods that describe a real life object
* object-oriented programming (OOP): is a computer programming model that organizes software design around data, or objects, rather than functions (functional programming).
* class: program-code-template for creating objects, providing initial values for properties and methods
* prototype: a property that allows you to add new properties and methods to existing object types
* super: is a keyword used to access and call functions on an object's parent
* inheritance:  the concept of one thing (object/class) gaining the properties or behaviours of something else(another parent object/class).
* constructor: is a function that creates an instance of a class.
* instance; an object containing data and behavior described by the class.
* context:  It refers to the object within the function being executed.
* this:  keyword refers to an object in which it is in it's context.
* Test Driven Development (TDD): is a technique for ensuring that your code does what you think it does, once as a test, and once as production code. If the two approaches don’t match, your tests fail, and you’ve caught a bug.
* Jest: JavaScript Testing Framework
* Continuous Integration (CI): is a coding philosophy and set of practices that drive development teams to implement small changes and check in code to version control repositories frequently
* unit test: automated tests written and run by software developers to ensure that a component behaves as intended.

## NoSQL Databases

SQL : is a language to manage data in astructured way (in tables) deals with relational databases
NoSQL databases: data is in collections that have documents with different structure in the same collection.
And collections don't rely on relations and support horizantal and vertical scaling for very large databases.

examples of NoSQL databases:

1. MongoDB
2. CouchDB
3. Redis

## NOSQL DATA MODELING TECHNIQUES

* Denormalization
* Aggregates
* Application Side Joins
* Atomic Aggregates
* Enumerable Keys
* Dimensionality Reduction
* Index Table
* Composite Key Index
* Aggregation with Composite Keys
* Inverted Search – Direct Aggregation
* Tree Aggregation
* Adjacency Lists
* Materialized Paths
* Nested Sets
* Nested Documents Flattening: Numbered Field Names
* Batch Graph Processing

[for more info on these techniques](https://highlyscalable.wordpress.com/2012/03/01/nosql-data-modeling-technique)
