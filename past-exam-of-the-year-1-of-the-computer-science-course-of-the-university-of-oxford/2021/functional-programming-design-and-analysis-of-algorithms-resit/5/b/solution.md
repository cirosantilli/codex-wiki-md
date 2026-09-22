<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Sequential accumulation writes merged outputs of lengths $2n,3n,\ldots,kn$. Its total work is

$$
\Theta\!\left(n\sum_{j=2}^{k}j\right)=\boxed{\Theta(nk^2)}\quad(k\geq2).
$$

The growing [list prefix](../../../../../prefix-of-a-list.md) is repeatedly copied, even though its internal order is already known.

Instead, divide the family of [arrays](../../../../../array-data-structure.md) into two nearly equal halves, recursively merge each half, and merge the two resulting [sorted arrays](../../../../../sorted-array.md). A balanced merge tree has $\lceil\log_2 k\rceil$ levels; at each level at most $kn$ entries are read or written in merges. Thus the bound is **$\Theta(kn\log k)$ for $k\geq2$**, including the output work. Equivalently the recurrence in the number of [arrays](../../../../../array-data-structure.md) is $M(k)=M(\lfloor k/2\rfloor)+M(\lceil k/2\rceil)+\Theta(kn)$. The one-[array](../../../../../array-data-structure.md) case simply returns it, or costs $\Theta(n)$ if a fresh output [array](../../../../../array-data-structure.md) is required.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
