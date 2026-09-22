<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use a non-dummy [circular linked list](../../../../../circular-linked-list.md) with a pointer to its last node:

```
private var last: Node = null
```

**Null represents the empty book.** In a nonempty book, `last.next` is the first node, and following `next` makes one finite simple cycle containing `last`. Names are unique around that cycle. This representation makes appending a new entry constant-time once a failed name search has established absence. The [abstraction function](../../../../../abstraction-function.md) collects every name/number pair on one complete turn of the cycle, rather than following pointers until null.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
