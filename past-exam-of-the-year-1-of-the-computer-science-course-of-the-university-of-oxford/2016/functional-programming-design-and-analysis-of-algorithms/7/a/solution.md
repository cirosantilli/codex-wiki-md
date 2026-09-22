<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The active prefix of the [array](../../../../../array-data-structure.md) must represent a complete $d$-ary tree, filled in the prescribed order, and must obey [heap order](../../../../../heap-order.md):

$$
\boxed{A[\operatorname{Parent}(i)]\leq A[i]
\quad\text{for every }1\leq i<A.\text{heap-size}}.
$$

Equivalently, every parent is no larger than each existing child. Repeatedly following parents shows that the root contains a global minimum. The array representation already provides the complete-tree shape; it is not enough to check only that the root is a minimum, since the inequality must hold throughout the [d-ary min-heap](../../../../../d-ary-min-heap.md). Assume integral $d\geq2$ throughout the heap operations.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
