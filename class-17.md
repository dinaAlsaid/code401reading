# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-16) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-18)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

Given the examples of front-end events such as button click, window resize, form submit, etc, what are some examples of back-end events?  
saving/reading in a database.  
Why are events sometimes better than asynchronous actions with callbacks?
What does an EventEmitter instance do?  
it will have all the event listeners attached to it, and provide the needed methods.  
When is a program’s call stack, event queue, and event loop active?  
call stack:function execution.  
event queue: when emitting multiple event handlers.  
event loop: when listening to events.

## Terms

Observer Pattern: software design pattern in which an object, called the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.  
Listener:
Event Handler: the function that will be executed when the event is emitted
Event Driven Programming: Event-driven programming is a programming pattern based on performing functions when an event is occuring.  
Event Loop: a programming construct or design pattern that waits for and dispatches events or messages in a program.  
Event Queue: a repository where events from an application are held prior to being processed by a receiving program or system.  
Call Stack: stack data structure that stores information about the active subroutines of a computer program
Emit/Raise/Trigger: perform a function when event occurs
Subscribe: listen for events.
