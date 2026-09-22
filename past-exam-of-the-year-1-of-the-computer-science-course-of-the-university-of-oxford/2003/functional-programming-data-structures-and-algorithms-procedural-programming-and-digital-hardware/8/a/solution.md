<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [list header](../../../../../list-header.md) is a stable entry record for a [linked list](../../../../../linked-list.md). In the dummy-header convention it is a [sentinel node](../../../../../sentinel-node.md), present even for an empty [linked list](../../../../../linked-list.md) and not representing an ordinary data item. It may also carry information such as the length.

In a [circular linked list](../../../../../circular-linked-list.md), following next links eventually returns to the start instead of reaching `NIL`. With a dummy [list header](../../../../../list-header.md), the last data node points to the header, whose next link points to the first data node; an empty header points to itself.

A [singly linked list](../../../../../singly-linked-list.md) stores a next pointer in every [linked list node](../../../../../linked-list-node.md). A [doubly linked list](../../../../../doubly-linked-list.md) additionally stores a previous pointer, allowing travel in both directions. For adjacent nodes, the consistency law is

$$
\boxed{u.next=v\quad\Longleftrightarrow\quad v.prev=u,}
$$

with suitable endpoint conventions in a noncircular representation.

## ↑ Ancestors (12)

1. [A](../a.md)
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
