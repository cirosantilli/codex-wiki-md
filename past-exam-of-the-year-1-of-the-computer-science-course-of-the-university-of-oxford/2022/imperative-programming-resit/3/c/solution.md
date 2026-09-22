<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep a head, a tail and a cached length:

```
private var first: QueueNode = null
private var last: QueueNode = null
private var size = 0
```

The [representation invariant](../../../../../representation-invariant.md) requires $0\leq size\leq Int.MaxValue$ and a finite acyclic [null-terminated linked list](../../../../../null-terminated-linked-list.md) of exactly `size` nodes starting at `first`. When `size == 0`, both endpoints are null. Otherwise `last` is precisely the final reachable node and `last.next == null`.

The [abstraction function](../../../../../abstraction-function.md) maps the chain from first to last to its payload [sequence](../../../../../sequence.md). Initially all pointers are null and the cached size is zero, giving the empty abstract queue. A tail pointer makes append constant-time; the cached size makes the `length` query constant-time without traversing the chain.

## ↑ Ancestors (12)

1. [C](../c.md)
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
