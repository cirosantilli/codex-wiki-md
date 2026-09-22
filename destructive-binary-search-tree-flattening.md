# Destructive binary search tree flattening

↑ **Parent:** [Binary search tree](binary-search-tree.md)

Turn a [binary search tree](binary-search-tree.md) into a sorted [doubly linked list](doubly-linked-list.md) by reusing each [linked list node](linked-list-node.md)'s left and right child fields as predecessor and successor fields. An [inorder traversal](inorder-traversal.md) determines the required order. A recursive implementation first saves both child references, flattens the disjoint child [subtrees](subtree.md), and splices their endpoints around the root. [Structural induction](structural-induction.md) proves that it preserves every original entry exactly once and produces reciprocal links with null outside endpoints. An explicit [stack](stack-data-structure.md) implements the same traversal without [recursive calls](recursive-call.md); each original right child must be saved before its field is overwritten. Both versions take linear [time complexity](time-complexity.md) and $O(h+1)$ [auxiliary space](auxiliary-space.md) for original height $h$. The old [binary search tree](binary-search-tree.md) representation is consumed, so outside aliases must not continue to interpret the changed links as child pointers.

## ↑ Ancestors (5)

1. [Binary search tree](binary-search-tree.md)
2. [Binary tree](binary-tree.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/5/d/ii/solution.md)
