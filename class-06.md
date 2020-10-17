# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-05) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-07)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.

In a book application: Book(a string), author(a string) and category(a string from a predefined set).
the author belongs to the book and the book belongs in a category.
2. What is the advantage of an ORM, like Mongoose?

* provides an abstraction layer on top of MongoDB that eliminates the need to use named collections.
* ORM layers ensure that your code is future-proof against new database backends.

3. How does the repository pattern compare with an ORM?
Repositories deal with Domain/Business objects (has behaviour), an ORM handles database objects(has only data).
4. When making a repository/facade, what flexibility do you gain?
you can code to an interface and then your application does not care what that initialization of that database layer is (change the database layer used)
5. Name 3 cloud based NoSQL Databases
IBM Cloudant/Redis/Azure

## terms

* lifecycle :JavaScript Execution Order (node App.js => Start executing script => Code parsing, Register events and functions => event loop=> keeps on running as long as event are registered.)
* collections:simply a grouping of documents that have the same or a similar purpose. A collection acts similarly to a table in a traditional SQL database
* the “Repository” design pattern:A Repository mediates between the domain and data mapping layers, acting like an in-memory domain object collection. Client objects construct query specifications declaratively and submit them to Repository for satisfaction. Objects can be added to and removed from the Repository, as they can from a simple collection of objects, and the mapping code encapsulated by the Repository will carry out the appropriate operations behind the scenes. Repository pattern separates the data access logic and maps it to the business entities in the business logic. Communication between the data access logic and the business logic  is done through interfaces.
* mongoose middleware:(also called pre and post hooks) are functions which are passed control during execution of asynchronous functions, document middleware, model middleware, aggregate middleware, and query middleware.
* Object Relation Mapping (ORM):  technique for converting data between incompatible type systems using object-oriented programming languages.

## HTTP and REST

### HTTP

HTTP stands for Hypertext Transfer Protocol. It's a stateless, application-layer protocol for communicating between distributed systems, and is the foundation of the modern web.
HTTP allows for communication between a variety of hosts and clients, and supports a mixture of network configurations.
This makes HTTP a stateless protocol. The communication usually takes place over TCP/IP, but any reliable transport can be used. The default port for TCP/IP is 80, but other ports can also be used.
Custom headers can also be created and sent by the client.

Request verbs:

GET: fetch an existing resource. The URL contains all the necessary information the server needs to locate and return the resource.
POST: create a new resource. POST requests usually carry a payload that specifies the data for the new resource.
PUT: update an existing resource. The payload may contain the updated data for the resource.
DELETE: delete an existing resource.

### REST

REST is acronym for REpresentational State Transfer. It is architectural style for distributed hypermedia systems.

Principles of REST:

* Client–server
* Stateless
* Cacheable
* Uniform interface
* Layered system
* Code on demand

Another important thing associated with REST is resource methods to be used to perform the desired transition. A large number of people wrongly relate resource methods to HTTP GET/PUT/POST/DELETE methods. instead th eimportant thing is having a uniform interface.