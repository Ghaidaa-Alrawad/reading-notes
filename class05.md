# Linked Lists

## Why We Use Linked Lists:

Okay, imagine we're working with data in our programs. Sometimes, we need a way to organize this data in a flexible manner. That's where linked lists come in! Linked lists are like chains of connected boxes, where each box holds some information and knows how to find the next box. We use linked lists when we want to handle data that can change a lot, like adding or removing pieces of information. Unlike arrays, where we need to plan ahead for the size, linked lists allow us to easily add or remove data without worrying too much about the memory. Plus, they're the building blocks for other cool data structures like stacks and queues.




## What Linked Lists Are:

Alright, so let's dive into what linked lists actually are. Imagine you have a bunch of boxes, and each box holds something important. We call each of these boxes a "node." But these nodes don't just hold data; they also have a special arrow that points to the next node in line. This connection between nodes creates a link, forming a linked list. It's like when you hold hands with your friends, you're all linked together in a line. Linked lists can be a bit different too. In some linked lists, each node only points to the next one, and that's called a "singly linked list." In others, nodes have arrows to both the next and the previous node, and that's called a "doubly linked list." The very first box is called the "head," and the last box usually points to nothing, like a sign that says "end of the line."




## How Linked Lists Work:

Alright, let's see how this works step by step. Imagine we want to make a list of names using linked lists. We start by creating a box, which is our first node. We put a name inside and say, "Hey, next box is null, there's nothing after this." Now, let's add more names. We create new boxes for each name, and we connect them by arrows. When we want to add a name in the middle, we just adjust the arrows to make space for the new box. If we need to remove a name, we adjust the arrows again to skip the empty box. To find a name in the list, we start from the head and follow the arrows until we reach the right box. So, linked lists are like building a chain of connected boxes, and it's a really handy way to manage data that can change a lot.