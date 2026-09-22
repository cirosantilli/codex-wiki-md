<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For an active segment of length $s$, partitioning takes $\Theta(s)$ comparisons. If pivot choice costs at most linear time and always leaves at most an $\alpha<1$ fraction on the searched side, the total is bounded by the [geometric series](../../../../../geometric-series.md) $N+\alpha N+\alpha^2N+\cdots$, giving **$\Theta(N)$** time.

Repeatedly choosing an extreme pivot while searching toward the other end retains lengths $N-1,N-2,\ldots$, giving **$\Theta(N^2)$** worst-case time. The equality interval makes an all-equal input finish in one partition. Independent uniform random pivots give expected linear time for duplicate-aware [Quickselect](../../../../../quickselect.md), but this is not a deterministic worst-case guarantee. More expensive pivot selection must be included in the cost rather than hidden inside the partition bound.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
