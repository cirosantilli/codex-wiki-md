<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [doubly linked list](../../../../../doubly-linked-list.md) supports backward traversal and removal of a known [linked list node](../../../../../linked-list-node.md) in [constant time](../../../../../constant-time.md), because that node supplies its own predecessor. In a [singly linked list](../../../../../singly-linked-list.md), removing a known node generally requires finding its predecessor by a forward scan unless the caller already supplies it. Inserting before a known node has the same advantage.

The cost is another pointer per node, more link assignments on every update, and a stronger consistency invariant to maintain. Hence

$$
\boxed{\text{bidirectional access and constant-time local deletion, with extra storage and updates}.}
$$

This does not make locating an arbitrary data value faster: a search still takes [linear time](../../../../../linear-time.md) in the worst case.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
