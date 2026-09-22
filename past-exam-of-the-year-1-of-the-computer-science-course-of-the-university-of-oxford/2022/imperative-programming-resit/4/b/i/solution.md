<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Within the sparse-vector implementation, use:

```
class Node(var value: Double, val index: Int,
           var prev: Node, var next: Node)
```

The header's `index` is the fixed vector dimension, so it need not change after construction. For a data node it is the coordinate index. The [representation invariant](../../../../../../representation-invariant.md) requires a finite simple cycle through the header, reciprocal predecessor/successor links, strictly increasing indices in the forward data-node traversal, indices in $[0,dimension)$, and a nonzero value at every data node. The header's value is ignored. The [abstraction function](../../../../../../abstraction-function.md) assigns stored values to their indices and zero to all missing coordinates.

The numerical code below takes entries to be finite `Double` values. Excluding NaN and infinities makes the relationship to a real [sparse vector](../../../../../../sparse-vector.md) explicit; arithmetic results still follow ordinary [floating-point arithmetic](../../../../../../floating-point-arithmetic-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Imperative programming (resit)](../../../../imperative-programming-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
