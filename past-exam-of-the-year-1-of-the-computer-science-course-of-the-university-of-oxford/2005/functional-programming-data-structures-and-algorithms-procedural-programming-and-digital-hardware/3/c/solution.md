<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Each of the finitely many distinct values has a first occurrence at a finite position, so every one is eventually emitted. After the last new value, however, the [list filters](../../../../../list-filter.md) keep searching the remaining infinite input for another new value. They never observe a terminating `[]`. Therefore the result has a finite visible prefix followed by the [bottom value](../../../../../bottom-value.md):

$$
\boxed{x_1:x_2:\cdots:x_k:\bot,\qquad\text{rather than }[x_1,\ldots,x_k].}
$$

For example, `remalldups (repeat 1)` exposes `1 : ...`, but demanding its tail diverges. This is the [absence-detection obstruction for infinite lists](../../../../../absence-detection-obstruction-for-infinite-lists.md): no finite inspection can certify that an unseen new value will never occur. The emitted values are correct, but computing the output length or proving the output empty after its last value does not terminate.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
