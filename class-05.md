# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-04) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-06)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## TDD

test driven development is a developing approach that helps eleminate or reduce the problems in the code where you write tests first then write the code.
What you should consider when testing is that you need to cover all possible cases (covering passing, failing and edge cases).

All the test should have an expected output, meaning you have to provide solutions for all these cases in the code too.

## linked lists

A linear data structure that is a sequence of Nodes that are connected/linked to each other, where every node references the next one.
Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.

there are two types of linked lists according to the number of reference points:

* singly: there is only one reference, and the reference points to the Next node in a linked list.

* doubly: there is a reference to both the Next and Previous node.

other important terms:

1. Next: Each node contains a property called Next. This property contains the reference to the next node.
2. Head: The Head is a reference type of type Node to the first node in a linked list.
3. Current: The Current reference is a reference type of type Node that is currently being looked at. This node is traditionally used when traversing through a full linked list.

We don't loop (traverse) through linked lists using for or forEach since each node references the next. we do that using a while loop to make sure that the next node is not null.

Order of operations is extremely important in a Linked List.

The biggest differentiator between arrays and linked lists is the way that they use memory arrays need all the data (bytes) to be in a block when saved in memory unlike linked lists.

## Big O notation

is a way of evaluating the performance of an algorithm.
One way to think about Big O notation is a way to express the amount of time that a function, action, or algorithm takes to run based on how many elements we pass to that function.

ex: O(1) or O(n)
n is the size of the input

O(1) function takes constant time
O(n) function is linear
O(n²) function is exponential
