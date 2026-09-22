# Undoing insertion of a new extreme key

↑ **Parent:** [Binary search tree](binary-search-tree.md)

If a key $q$ is smaller than every key of a finite [binary search tree](binary-search-tree.md) $R$, insert $q$ and then delete the minimum: the original tree, including its shape, is recovered. The insertion follows the leftmost search route and creates a new minimum leaf; deleting that leaf reverses the same route. The symmetric statement uses a fresh maximum. At a node with root $x$, the bounds on its children therefore let a direct [tree fold](tree-fold.md) reconstruct an untouched child from that child's insertion result. This gives a direct fold implementation of insertion without assuming that insertion is injective on arbitrary trees.

## ↑ Ancestors (5)

1. [Binary search tree](binary-search-tree.md)
2. [Binary tree](binary-tree.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/4/g/solution.md)
