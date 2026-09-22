<h1 id="6/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $1\leq i\leq n$. Apply a worst-case $\Theta(n\log n)$ [comparison sort](../../../../../../comparison-sort.md), such as [merge sort](../../../../../../merge-sort.md) or [heapsort](../../../../../../heapsort.md), to the whole [array](../../../../../../array-data-structure.md), then copy its first $i$ entries to the output. The copying costs $\Theta(i)$, so

$$
\boxed{T_1(n,i)=\Theta(n\log n+i)=\Theta(n\log n)\quad(n\geq2).}
$$

The [comparison sorting lower bound](../../../../../../comparison-sorting-lower-bound.md) makes the full-sort stage tight. For the sample [array](../../../../../../array-data-structure.md), the sorted order begins $2,6,7$, which is the required prefix for $i=3$. This method spends time ordering all $n-i$ unreported elements as well.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
