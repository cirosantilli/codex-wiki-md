<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [list header](../../../../../list-header.md) is a permanent dummy [linked list node](../../../../../linked-list-node.md), distinct from the ordinary elements. It gives a stable reference to the [linked list](../../../../../linked-list.md) and can store metadata such as its length. In a [circular linked list](../../../../../circular-linked-list.md), following successor links eventually returns to the starting point; with a [list header](../../../../../list-header.md), the last ordinary element links to the header, and the empty structure has the header linked to itself.

A [singly linked list](../../../../../singly-linked-list.md) stores a successor reference per [linked list node](../../../../../linked-list-node.md). A [doubly linked list](../../../../../doubly-linked-list.md) additionally stores a predecessor reference. The latter supports traversal in both directions and deletion of a known [linked list node](../../../../../linked-list-node.md) in [constant time](../../../../../constant-time.md), without first searching for its predecessor. It costs another reference per [linked list node](../../../../../linked-list-node.md) and additional updates whose mutual consistency must be maintained. A [list header](../../../../../list-header.md) makes insertion and deletion at an endpoint use the same local splicing rules as an interior change; the empty case does not require replacing an external head reference.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
