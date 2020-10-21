# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-09) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-11)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Quick notes

* CRUD operations are for creating, reading, updating and deleting data from a database.
* REST uses get, post, put, patch, delete from HTTP to send requests to the client.
* a middleware will perform functions between the CRUD and the REST. (between the client-to-server and server-to-database).
* using Supertest will help test ensure that none of your data is persisted into a live database and that your server need not be started while testing.
* modularity in an API server will help alot in organising large apps and makes it easy to update and modify the code and makes it suitable for further additions.

## Stacks and Queues

### stacks

common terminology:

* push: add nodes to the stack
* pop: remove nodes from the stack
* top of the stack: the last node in the stack
* peek into the stack: when doingso you will see the top of the stack.
* FILO and LIFO : first inlast out and last in first out, which refer to the order of doing pushing and poping nodes.

when you pop from the stack you will pop the top, making the next node the new top of the stack.

the time efficiency of pop and push is O(1)

### Queues

common terminology:

* Enqueue: Nodes or items that are added to the queue
* Dequeue: Nodes or items that are removed from the queue.
* Front: This is the front/first Node of the queue.
* Rear: This is the rear/last Node of the queue.
* FIFO and LILO: First In First Out and Last In Last Out

the time efficiency of enqueue and dequeue is O(1)
