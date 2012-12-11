# Queue

A queue is a data structure in which elements are kept in order and new elements are added to the end of the collection *enqueue()* and removed from the beginning *dequeue()*.
A queue is a FIFO (first in first out) data structure.

## Examples and Use Cases

Check-out lines are an example of queues- the first customer to enter the line is the first one served.

In Computer Science, queues are used to store items that must be processed sequentially in the order they are enqueued. For example, you could implement Breadth-First Search using a queue to hold to nodes that need to be visited.

## Potential Implementations

Common implementations of queues include linked lists and arrays. Using linked lists comes with the overhead of storing pointers to the next item in the queue for each element. Array based queues would reduce this overhead but must be resized if more elements are added than space allocated, an expensive operation.

###Linked List Based Queue
A linked queue class in C++ would need to contain a pointer to the root node of the queue. Each node must have a pointer to the next node, with the last node having a null pointer. The last node may also point to the root node in the case of a cirular queue.

Using a linked implementation, *enqueue()* could add an item to the end of the list in O(n) time where n is the size of the list. If the queue class contains a data member that points to the last node, this could be done in constant time. The *dequeue()* operation will always take constant time because it must only store the node, then assign the root pointer either to null or to the next node in the list.

###Array Based Queue
An array based queue with the first node always stored in the first position of the array could implement both *enqueue()* and *dequeue()* in O(n) time where n is the size of the queue because each element would need to be shifted in each of these operations.

Using a fixed size circular array to implement a queue, where two pointers are used to point to the beginning and end of the queue, both *enqueue()* and *dequeue()* could be implemented in constant time. This would mean that the queue would have to be of constant size or have an expensive operation that increases the size of the queue, which would run in O(n) time where n is the number of elements in the queue.

## Time and Space Analysis
See above for time analysis.

The space required by any implementation of a queue will always be O(n) where n is the size of the queue.
