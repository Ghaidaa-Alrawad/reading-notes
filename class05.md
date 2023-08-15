# Linked Lists

## Why, What, How

### Why We Use Linked Lists:

Okay, imagine we're working with data in our programs. Sometimes, we need a way to organize this data in a flexible manner. That's where linked lists come in! Linked lists are like chains of connected boxes, where each box holds some information and knows how to find the next box. We use linked lists when we want to handle data that can change a lot, like adding or removing pieces of information. Unlike arrays, where we need to plan ahead for the size, linked lists allow us to easily add or remove data without worrying too much about the memory. Plus, they're the building blocks for other cool data structures like stacks and queues.




### What Linked Lists Are:

Alright, so let's dive into what linked lists actually are. Imagine you have a bunch of boxes, and each box holds something important. We call each of these boxes a "node." But these nodes don't just hold data; they also have a special arrow that points to the next node in line. This connection between nodes creates a link, forming a linked list. It's like when you hold hands with your friends, you're all linked together in a line. Linked lists can be a bit different too. In some linked lists, each node only points to the next one, and that's called a "singly linked list." In others, nodes have arrows to both the next and the previous node, and that's called a "doubly linked list." The very first box is called the "head," and the last box usually points to nothing, like a sign that says "end of the line."




### How Linked Lists Work:

Alright, let's see how this works step by step. Imagine we want to make a list of names using linked lists. We start by creating a box, which is our first node. We put a name inside and say, "Hey, next box is null, there's nothing after this." Now, let's add more names. We create new boxes for each name, and we connect them by arrows. When we want to add a name in the middle, we just adjust the arrows to make space for the new box. If we need to remove a name, we adjust the arrows again to skip the empty box. To find a name in the list, we start from the head and follow the arrows until we reach the right box. So, linked lists are like building a chain of connected boxes, and it's a really handy way to manage data that can change a lot.

---

## Cheat Sheet

### Definition and Purpose:

- Linked lists are a data structure used to organize and manage data in a flexible way.
- They are composed of nodes, where each node contains a value and a reference (or pointer) to the next node.
- Linked lists are valuable for scenarios where data size changes frequently or when memory allocation is limited.

## Types of Linked Lists:

### Singly Linked List:

-Each node points only to the next node in the sequence.
-Starts with a head node and ends with a tail node pointing to null.

### Doubly Linked List:

- Each node points to both the next and previous nodes.
- Provides faster backward traversal.
- Requires slightly more memory for the additional previous pointers.

## Operations:

### Insertion:

Adding a new node to the list.
Adjust the references of neighboring nodes to link the new node correctly.
Deletion:

Removing a node from the list.
Reconfigure the references of neighboring nodes to bypass the deleted node.
Traversal:

- Moving through the linked list to access or manipulate nodes.
- Start from the head and follow the references until you reach the desired node.

### Advantages:

### Dynamic Size:

Easily add or remove nodes without needing contiguous memory allocation.
Efficient Insertions/Deletions:

Compared to arrays, linked lists excel at insertions and deletions at any position.
Versatility:

Serve as building blocks for more complex data structures like stacks, queues, and graphs.
Considerations:

### Memory Overhead:

Linked lists store references along with data, which can lead to slightly higher memory usage compared to arrays.
Traversal Complexity:

Traversing linked lists can be slower than arrays due to the need to follow references.
Use Cases:

- When the size of the data structure is unpredictable or frequently changes.
- When efficient insertions and deletions are required.
- For implementing stacks, queues, and other specialized data structures.