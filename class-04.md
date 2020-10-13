# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-03) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-05)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. Why would a developer choose to make data models?
Data modeling makes it easier to integrate high-level business processes with data rules, data structures
2. What purpose do CRUD operations serve?
stands for create, read, update and delete, and helps to do these operations on the data in a database
3. What kind of database is Postgres? What kind of database is MongoDB?
Postgres: object-relational database
MongoDB: noSQL database
4. What is Mongoose and why do we need it?
is an Object Data Modeling (ODM) library for MongoDB and Node.js. It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB.

## Terms

* database: is a data structure that stores organized information
* data model: conceptual representation of Data objects, the associations between different data objects, and the rules.
* CRUD: create, read, update and delete, four basic functions that models should be able to do, at most
* schema:the skeleton structure that represents the logical view of the entire database
* sanitize: removing any illegal character from the data.
* Structured Query Language (SQL):is a programming language that is typically used in relational database or data stream management systems.
* Non SQL (NoSQL): non-relational database.
* MongoDB:document database
* Mongoose:is an Object Data Modeling (ODM) library for MongoDB and Node.js.
* record:  a database entry
* document:
* Object Relation Mapping (ORM): write queries using the object-oriented paradigm of your preferred programming language instead of SQL

## Repository design pattern

design  pattern is a reusable solution to a general problem occurring in a given context in software design and is not connected to particular language or framework.

Repository pattern separates the data access logic and maps it to the business entities in the business logic.
(business logic accesses the data object without having knowledge of underlying data access architecture).

Using repositories as an interface will not limit you to connect to one ORM or database. it gives flexibility to your application.

## In-memory database

helps with unit testing mongoose in node.js. is a process that stores the data in memory.

advantages:

* No need for mocks.
* Faster development
* More reliable tests
* Tests are easier to build

disadvantages:

* in-memory database needs seeding
* More memory usage
* Tests take longer to run depending on hardware
