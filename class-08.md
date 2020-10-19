# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-07) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-09)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. Name 3 real world use cases where you’d want to change the request with custom middleware.

- adds current server time to the request
- validate incoming cookies
- log the path for each incoming request

2. True or false: The route handler is middleware?

true
3. In what ways can a middleware function end the process and send data to the browser?
by setting the next function
4. At what point in the request lifecycle can you “inject” middleware?
anywhere
5. What can cause express to error with “Request headers sent twice, cannot start a second response”.
sending two responses for one request.

## terms

* Middleware: middleware functions are functions that have access to the request object (req), the response object (res) and the next middleware function in the application’s request-response cycle.
* Request Object: represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on.
* Response Object: The res object represents the HTTP response that an Express app sends when it gets an HTTP request
* Application Middleware: represented by app.use() and app.METHOD(), where METHOD is the HTTP method(in lowercase).
* Routing Middleware: works in the same way as application-level middleware, except it is bound to an instance of express.Router().

## routing

routing is how an application’s endpoints (URIs) respond to client requests.
Routing is defined using methods of the Express app that correspond to HTTP methods.
These routing methods specify a callback function (can have more than one callback function), called when the application receives a request to the specified route.

A route method is derived from one of the HTTP methods, and is attached to an instance of the express class.

**Route parameters** are named URL segments that are used to capture the values specified at their position in the URL.

## Express Router

Express Router is a mini express application with only the routing stuff.

Route middleware in Express is a way to do something before a request is processed. This could be things like checking if a user is authenticated, logging data for analytics, or anything else we'd like to do before we actually spit out information to our user.

usually we will use `router.use()` to define middleware.