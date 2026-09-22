<h1 id="8/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Maintain two [spanning trees](../../../../../../spanning-tree.md) $U,U'$ whose sorted edge sequences share a prefix, initially of length zero. At the next position, select whichever next edge has smaller weight, breaking equal-weight ties arbitrarily. Keep that tree unchanged and apply [spanning-tree prefix exchange](../../../../../../spanning-tree-prefix-exchange.md) from part (i) to the other tree. Both trees now have a common prefix one edge longer; one tree's sorted weight vector is unchanged and the other's cannot increase coordinatewise.

Repeat for $k$ positions. The final trees have all their edges in common, so they are one tree $\widetilde T$. Throughout, the sorted weight vector of $U$ never exceeds its original vector from $T$, and that of $U'$ never exceeds its original vector from $T'$. Consequently their common final vector satisfies **$w(\widetilde e_i)\leq\min\{w(e_i),w(e'_i)\}$ at every position**.

This proves the required existence without assuming either original tree was minimum. More generally, a [minimum spanning tree](../../../../../../minimum-spanning-tree.md) has a [coordinatewise minimum spanning-tree weight vector](../../../../../../coordinatewise-minimum-spanning-tree-weight-vector.md): after restricting the graph to edges of weight at most any threshold, a maximum forest contains at least as many edges as the corresponding portion of every other spanning tree. This threshold viewpoint explains why an optimum can simultaneously dominate every sorted coordinate, rather than merely having a smaller total weight.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
