# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-08) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-10)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## review

1. How does route prefixing work with an external routing module?

2. When routing, what’s the difference between app.get('/data/:id') and app.get('/data/:name')?
The parameter name. if you were to type an id number in the one with the name parameter it will take it and store it in req.params.name
3. Explain how Express handles routing conflicts?
it'll go through each of the routes matching in the order they are set in.
4. What are the ways that a browser can send “data” or request variables to an HTTP server

## Terms

* Routing: is how an application’s endpoints (URIs) respond to client requests.
* Route Prefixing: specify the common route prefix at the controller level to eliminate the need to repeat the common route prefix on each and every controller action by using ~ in front of the route.
Request “Body”:the data sent by the client to your API
Request “Query”: set of parameters attached to the end of a url. They are extensions of the URL that are used to help define specific content or actions based on the data being passed.
Request “Params”: parameters in the url used to request specific data and are stored in the request as params.

## preperation amterial

### router.param(name, callback)

Adds callback triggers to route parameters, where name is the name of the parameter and callback is the callback function.

The parameters of the callback function are:

* the request object.
* the response object.
* indicating the next middleware function.
* The value of the name parameter.
* The name of the parameter.

### mongoose middlewares

Mongoose has 4 types of middleware: document middleware, model middleware, aggregate middleware, and query middleware and they all support post and pre hooks.

* In document middleware functions, this refers to the document.
* In query middleware functions, this refers to the query.
* In aggregate middleware, this refers to the aggregation object. and executes when you call exec() on an aggregate object.
* In model middleware functions, this refers to the model.

### subdocuments

Subdocuments are documents embedded in other documents. which means having schemas inside schemas.
ne important reason to use subdocuments is to create a path where there would otherwise not be one to allow for validation over a group of fields

### mongoose virtuals

Using mongoose virtuals, you can define more sophisticated relationships between documents. which is an alternative for using the _id property.
If you want populate virtuals to show up when using functions that rely on JSON.stringify(), like Express' res.json() function, set the virtuals: true option on your schema's toJSON options.

``` javascript
const BandSchema = new Schema({
  name: String
}, { toJSON: { virtuals: true } });
```
