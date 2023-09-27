Queues

A queue is a FIFO ADT

Think of a line at Starbucks
- That is a queue

Queue Vocablulary
* A queue has a front 
  * This is the first node in the queue
  * This is where people in the line get proicessed
* A queue has a back

> Working with a list

* Enqueue
 * add to the back of the queue  
* Dequeue
 * remove from the front of the queue

```Java
 QueueInterface <String> myQueue = new LinkedQueue<>();

// Jess Jim Jane Jill
// Jess
```

Simulation
* simulate a real world problem
* This means important features of the problem are in the program
* this is a safe environment, business who use the simulation can try "What if" without any cost

* The data us fed into a simulation
* runs for a fixed time period
* results are analyzed

 ---

> Using java queues

there are two versions of add in the queue interface
* add
* offer
there are two versions of remove in the queue interface
* remove
* poll
there are two versions of return in the queue interface
* peek
* element


Deque = deck
- double ended queue
- you can remove or add to either end of the queue
  - add to front
  - add to back
- also a class called ArrayDeque

---
CompareTo method

__how to tell whether it returns a positive, negative or zero?__
* Think of subtraction of integers 
* a < b is the same as a - b < 0
* So a compareTo(b) < 0 when a < b
* The other two cases are similar

Back to Priority Queues
* items can be added to a queue in any order
* when they are removed they are removed based on priority
 * this is a reason why we need a method to compare entries
* the java standard does not say what happens when there is a tie in priority, th is means you shouldn't count on these items to come out in FIFO
 * if you want items to come out FIFO you must make that part of the comparison

> Implementing a queue using a linked list

* make sure the queue has a front and a back
  
> Implementing a queue using an array
*  This is difficult
*  as we move along the array, adding and removing, we can move to the end of the array very fast
*  BUT THERE WILL BE LOTS OF UNUSED SPACE AT THE FRONT


circular queue's and circular linked lists, doubly linked lists
