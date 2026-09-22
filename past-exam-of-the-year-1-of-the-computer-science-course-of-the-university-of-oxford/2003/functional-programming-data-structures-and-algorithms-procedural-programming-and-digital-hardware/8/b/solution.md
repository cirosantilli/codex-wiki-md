<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A dummy [list header](../../../../../list-header.md) makes insertion or deletion at the front resemble insertion or deletion in the middle: there is always a predecessor record to update. In a circular [doubly linked list](../../../../../doubly-linked-list.md), it also supplies a stable end position, handles the empty case uniformly, and avoids changing an external head pointer every time the first data node changes.

Its disadvantage is the extra record and associated storage and initialization work; traversal must also distinguish the [sentinel node](../../../../../sentinel-node.md) from real data. Thus

$$
\boxed{\text{simpler boundary operations at the cost of one extra header record}.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
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
