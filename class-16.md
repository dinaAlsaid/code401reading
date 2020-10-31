# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-15) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-17)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. Why is access control important?
minimize the risk of unauthorized access to physical and logical systems.
2. Describe an application that would need access control.
a blog that has an admin that can read write, edit, approve and delete articles, an editor that can read write and edit, a writer that can read and write articles and a visitor that can read
3. What is a role used for?
to limit access of users to certain functionalities in a web app and organize their duties and capabilities.
4. Why is role based access control more scalable than discretionary or mandatory access control?

## Term

Authorization: the process of granting or denying access to a network resource which allows the user access to various resources based on the user's identity.
Role Based Access Control :Assigning system access to users based on their roles in the organization
Capabilities

## Event-driven programming

Event-driven programming is a programming pattern based on performing functions when an event is occuring.
Node.js provides a module called `EventEmitter` that will help incorporate event driven programming.
We access the EventEmitter class through the events module. Once imported we’ll need to create a new object from the class to start using it.  

```javascript
const EventEmitter = require('events').EventEmitter;
const myEventEmitter = new EventEmitter;
```

using `on` method for the EventEmitter we can attach an event listener to it.  
To remove event listeners in EventEmitter we can use the `removeListener` or `removeAllListeners` method.  

[list of events in Node.js](https://nodejs.org/api/events.html)
