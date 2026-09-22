<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [list header](../../../../../list-header.md) is a permanent dummy node that represents the list boundary rather than a data entry. A [circular linked list](../../../../../circular-linked-list.md) links the last node back to the first or to the header. A [singly linked list](../../../../../singly-linked-list.md) stores only a successor; a [doubly linked list](../../../../../doubly-linked-list.md) stores both successor and predecessor references.

A header provides a stable object even for an empty list, makes insertions and deletions at the ends resemble interior operations, and can hold metadata such as the vector length in this question. In a circular header-based representation, the empty list is the header linked to itself.

A [doubly linked list](../../../../../doubly-linked-list.md) permits backward traversal and constant-time unlinking of a known node without searching for its predecessor. It uses an extra reference per node and requires more pointer updates and a stronger consistency invariant. Finding a node by an arbitrary index can still require a linear scan: bidirectional links alone do not provide random access.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
