# Linked List

* A way to store collection of elements like an array. Each element in a Linked list is stored in the form of a `Node`.

* A `Node` is a collection of two sub-elements/parts.

    1. `Data` - that stores the element

    2. `Next` - that stores the link to the next node

* A Linked list is formed when many such nodes are linked together to forma a chain. Each node points to the next node present in the order.

* The first node is always useds as a reference to traverse the list and is called `Head`.

* The last node points to `Null`.

## Basic operations

1. Insertion

2. Deletion

3. Display

4. Search

5. Delete

## Variations

1. Doubly Linked List

*  Here the navigation is possible in both ways, either forward and backward.

* A `Node` contains

    1. `Data` - that store the element

    2. `Next` - that store the link to the next node

    3. `Prev` - that store the link to the prev node

**Basic operations**

* Basic Linked List operations + Below

    1. Display forward

    2. Display backword

    3. Insert Last

    4. Delete Last

    5. Insert After

2. Circular Linked List

* A Linked list in which the first element points to the last element and the last element points to the first element.

* Both Singly and Doubly Linked list can be made into a circular Linked list.

**For Singly Linked list:**

* The next pointer of the last node points to first node

**For Duubly Linked list:**

* The next pointer of the last node points to the first node.

* The previous pointer of the first node points to the last node making the circular in both directions.

