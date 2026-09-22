# Lazy breadth-first traversal with child iterators

↑ **Parent:** [Breadth-first tree search](breadth-first-tree-search.md)

Maintain a [FIFO queue](fifo-queue.md) of child iterators ordered by the breadth-first order of their parents. Consume a child from the front iterator and append a deferred iterator for that child's children; discard empty front iterators as needed. This enumerates descendants without first materializing a whole child list or level. On a [locally finite tree](locally-finite-tree.md), each node occurs after finitely many earlier outputs. If an earlier level is infinite, strict breadth-first order cannot put a deeper node at any finite output position; that obstruction is inherent in the requested ordering.

## ↑ Ancestors (7)

1. [Breadth-first tree search](breadth-first-tree-search.md)
2. [Breadth-first search](breadth-first-search.md)
3. [Tree (graph theory)](tree-graph-theory-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/imperative-programming-resit/7/b/i/solution.md)
