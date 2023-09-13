# Trees Reading

## WHY:

Trees are a fundamental data structure in computer science used to organize and store data efficiently, it provides a way to store data in a hierarchical structure that allows for fast retrieval, insertion, and deletion of elements.

Moreover, balanced trees like Binary Search Trees (BSTs) ensure that data is organized in a way that guarantees logarithmic time complexity for operations, ensuring efficiency.

**PS:** Hierarchical Structure: elements are organized in a layered or tree-like arrangement, with each element having a parent and, potentially, one or more children)

## WHAT:

- A tree is a data structure composed of nodes, each node has a value and zero or more child nodes, forming a hierarchical structure.
- The Top node of a tree is called the Root node, it's the starting point for traversing the tree.
- Nodes in a tree have a parent-child relationship, the node from which a branch originates is the parent, and the nodes connected to it are its children.
- The Node that has NO children called leaves.
- A specific type of tree, called a Binary Tree, has at most two children per node.
- Binary Search Trees (BSTs): A type of binary tree where each node has a value, and the values in the left subtree are less than the node's value, while values in the right subtree are greater.

**PS:** A subtree is a smaller tree structure contained within a larger tree, sharing its hierarchical characteristics.

## HOW:

I'll explain how in java:

- We can implement trees in Java using classes, define a class for the tree structure and another class for nodes, each node contains a value and references to its children (Creating the Tree).
- Now how to insert:  We will start at the root and traverse down the tree, comparing values to determine whether to move left or right until we find an appropriate spot for the new node.
- Searching in a tree involves similar traversal, we will start at the root and follow the path left or right based on the comparison of the target value with the current node's value.
- Finally the Deleting: when deleting a node from a tree data structure, we can choose to replace it with either its in-order predecessor (older sibling) or in-order successor (younger sibling), this replacement ensures that the tree structure remains intact and maintains the correct relationships between nodes.