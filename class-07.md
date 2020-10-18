# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-06) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-08)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. What’s the difference between PUT and PATCH?
when using PUT you have to provide all the data even the things are not changed in the request body when updating it. On the other hand PATCH will only update the specified enteries.
2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server
Postman/Insomnia REST Client/Firebase
3. Compare and contrast Swagger and APIDoc.js
Swagger: is a suite of API developer tools for teams and individuals, enabling development across the entire API lifecycle, from design and documentation, to test and deployment.
APIDoc.js: Inline Documentation for RESTful web APIs
4. Compare and contrast SOAP and ReST?
SOAP is a protocol that defines a set of rules for communication using XML-based messaging.SOAP is not meant to be used over HTTP.
REST is not based on any protocol but has a standard architecture principle used to send data over standard protocols (HTTP)

## terms

SOAP:(Simple Object Access Protocol) a protocol that defines a set of rules for communication using XML-based messaging
ReST Verbs: GET, PUT, PATCH, DELETE
CRUD Verbs: Read, Update/Replace, Update/Modify, Delete
Swagger: is a suite of API developer tools for teams and individuals, enabling development across the entire API lifecycle, from design and documentation, to test and deployment.

## MiddleWare with an Express application

middleware functions are functions that have access to the request object (req), the response object (res) and the next middleware function in the application’s request-response cycle.
types of middleware an express application can use:

* Application-level middleware: represented by app.use() and app.METHOD(), where METHOD is the HTTP method(in lowercase).
* Router-level middleware: Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router()
* Error-handling middleware: functions in the same way as other middleware functions, except with four arguments instead of three, specifically with the signature (err, req, res, next))
* Built-in middleware: built-in with express (express.static,express.json,express.urlecoded)
* Third-party middleware:adds functionality to Express apps.

examples of third-party middleware:

1. body-parser
2. cookie-parser
3. express-session

## Routing

which is how an application’s endpoints (URIs) respond to client requests, using methods of the Express app object that correspond to HTTP methods.

These routing methods specify a callback function called when the application receives a request to the specified route and HTTP method.

The characters ?, +, *, and () are subsets of their regular expression counterparts. The hyphen (-) and the dot (.) are interpreted literally by string-based paths.If you need to use the dollar character ($) in a path string, enclose it escaped within ([ $ ]).
