# Stacks and Queues

## What is a Stack

A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

## terminology for a stack is:

1. Push - Nodes or items that are put into the stack are pushed
2. Pop - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
3. Top - This is the top of the stack.
4. Peek - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
5. IsEmpty - returns true when stack is empty otherwise returns false.

## concepts:

### FILO

First In Last Out

This means that the first item added in the stack will be the last item popped out of the stack.

### LIFO

Last In First Out

This means that the last item added to the stack will be the first item popped out of the stack.

## Stack Visualization

Here’s an example of what a stack looks like. As you can see, the topmost item is denoted as the top. When you push something to the stack, it becomes the new top. When you pop something from the stack, you pop the current top and set the next top as top.next.

Pushing a Node onto a stack will always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.

When adding a Node, you push it into the stack by assigning it as the new top, with its next property equal to the original top.
![Stack](401-Notes/assets/stack.png)

## What is a Queue

A queue is one of the linear data structures used to store data in the memory. Queue is a linear data structure that stores data sequentially based on the First In First Out manner. The queue data structure is also known as the First Come, First Served data structure.

## terminology

1. Enqueue - Nodes or items that are added to the queue.
2. Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
3. Front - This is the front/first Node of the queue.
4. Rear - This is the rear/last Node of the queue.
5. Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
6. IsEmpty - returns true when queue is empty otherwise returns false.

## concepts

### FIFO

First In First Out

This means that the first item in the queue will be the first item out of the queue.

### LILO

Last In Last Out

This means that the last item in the queue will be the last item out of the queue.

## Queue Visualization

![queue](401-Notes/assets/queue.png)


[link-to-reading-notes](https://react.dev/learn/scaling-up-with-reducer-and-context).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?