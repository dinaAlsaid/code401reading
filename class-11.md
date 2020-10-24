# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-10) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-12)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. Explain what a “Singleton” is (in Computer Science terms).
it is a single exported instance.
2. Explain how the Singleton pattern can be used with Node modules, specifically with classes.
instead of exporting the whole class then creating a new instance where you import it, exporet a new instance directly to make things easier.

## Term

* Router Middleware: Router-level middleware works in the same way as application-level middleware, where you can use the HTTP methods, except it is bound to an instance of express.Router()
* Dynamic Module Loading: mechanism by which a computer program can, at run time, load/import a library into memory. which means that they are only loaded when needed.
* Singleton Pattern: a design pattern that involves a single class responsible of creating an object while making sure that only single object gets created. This class provides a way to access its only object which can be accessed directly without need to instantiate the object of the class.
* CRUD -> REST Method Matches: mapping CRUD methods into REST methods  where create maps to POST, read maps to GET, update maps to PUT/PATCH/POST , and delete maps to delete.
* Mock Testing: an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules where dependencies are replaced with objects that simulate the behaviour of the real ones.

## Authentication

basic access authentication is a method for an HTTP client to provide a user name and password when making a request.
it does not require cookies, session identifiers, or login pages.

### Securing passwords using Bcrypt

Hashing is an irreversable process but it still has it's weaknesses
Hashing algorithm weaknesses:

1. Brute Force attack: instead of reversing the hash of the password, an attacker can simply keep trying different inputs until he does not find the right now that generates the same hash value.

2. Hash Collision attack:Hash functions have infinite input length and a predefined output length, so there is inevitably going to be the possibility of two different inputs that produce the same output hash

to over come these weaknesses new agorithms like Bcrypt are used. which use a technique called key streching.
Bcrypt is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor).

### Bcrypt

bcrypt is a password-hashing function, bcrypt is an adaptive function where over time, the iteration count can be increased to make it slower, so it remains resistant to brute-force search attacks even with increasing computation power.

### JWT (JSON web tokens)

is an open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. used in authorisation and information exchange.

It consists of three parts:

1. Header
2. Payload
3. Signature
