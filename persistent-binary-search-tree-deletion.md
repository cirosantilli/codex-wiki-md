# Persistent binary search tree deletion

↑ **Parent:** [Binary search tree](binary-search-tree.md)

A [pure function](pure-function.md) deletes a key from a [binary search tree](binary-search-tree.md) by rebuilding its search path and sharing untouched subtrees. At a matching node with two children, replace its key by the least key in its right subtree, removing that occurrence from the right subtree. The ordering invariant is preserved, with [time complexity](time-complexity.md) and fresh-node allocation proportional to the [height of a binary tree](height-of-a-binary-tree.md).

## ↑ Ancestors (5)

1. [Binary search tree](binary-search-tree.md)
2. [Binary tree](binary-tree.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/4/g/solution.md)
