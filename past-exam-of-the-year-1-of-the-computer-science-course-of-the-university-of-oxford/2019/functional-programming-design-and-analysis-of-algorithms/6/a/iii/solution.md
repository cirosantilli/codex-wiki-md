<h1 id="6/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Leaves already obey the [heap order](../../../../../../heap-order.md). Process indices $\lfloor n/2\rfloor,\lfloor n/2\rfloor-1,\ldots,1$, calling the preceding repair at each. When an index is processed, its descendants have already been processed, so the repair's precondition holds. The resulting [array](../../../../../../array-data-structure.md) is a [max-heap](../../../../../../max-heap.md).

The bound obtained by charging $O(\log n)$ to every call is unnecessarily large. The number of nodes with height at least $h$ is at most $\lfloor n/2^h\rfloor$. Therefore

$$
\sum_v(1+\operatorname{height}(v))
\le n+\sum_{h\ge1}\lfloor n/2^h\rfloor<2n.
$$

The total repair work is thus **$O(n)$**, and the loop itself has a linear number of iterations, giving **$\Theta(n)$** for this [bottom-up heap construction](../../../../../../bottom-up-heap-construction.md). Most nodes are near the leaves and require little repair.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
