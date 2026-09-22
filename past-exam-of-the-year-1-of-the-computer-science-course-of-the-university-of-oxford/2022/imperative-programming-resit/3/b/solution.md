<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A node needs a stored value and one successor reference:

```
final class QueueNode(val value: Int, var next: QueueNode)
```

A null successor terminates the chain. The stored value need not be mutable for a [FIFO queue](../../../../../fifo-queue.md), because enqueue creates a node and dequeue removes one rather than changing its payload.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
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
