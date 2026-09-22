<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use an immutable index and mutable value and links:
```
class Node(var value: Double, val index: Int,
           var prev: Node = null, var next: Node = null)
```
For the [sparse linked vector representation](../../../../../../sparse-linked-vector-representation.md), a header `h` has `h.index >= 0`, records that [vector](../../../../../../vector.md)'s dimension, and lies on a finite [circular linked list](../../../../../../circular-linked-list.md). Every ordinary [linked list node](../../../../../../linked-list-node.md) has an index in `[0,h.index)`, a nonzero finite value, and a unique index; indices increase strictly from `h.next` to `h.prev`. For every reachable [linked list node](../../../../../../linked-list-node.md), including `h`, `p.next.prev eq p` and `p.prev.next eq p`. The [abstraction function](../../../../../../abstraction-function.md) fills unspecified coordinates with zero. The header's value has no meaning. Finite real coordinates are assumed throughout; infinities and `NaN` are not ordinary [real number](../../../../../../real-number.md) coordinates for a mathematical [inner product](../../../../../../inner-product-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
