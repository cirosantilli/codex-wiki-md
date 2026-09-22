<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix any seven-element [subset](../../../../../subset.md) $S$. Its [power set](../../../../../power-set.md) supplies $2^7=128$ pigeons. Map each [subset](../../../../../subset.md) to its [integer](../../../../../integer-split.md) sum. Since the elements are positive, all such sums lie between $0$ and $\sum_{s\in S}s$. The latter is at most the sum of the seven largest available elements,

$$
10+11+\cdots+16=91.
$$

There are therefore at most $92$ possible sums, fewer than the $128$ [subsets](../../../../../subset.md). The [pigeonhole principle](../../../../../pigeonhole-principle.md) forces two distinct [subsets](../../../../../subset.md) to have the same sum. **Every seven-element subset has the two-sum property.** This is the [subset-sum pigeonhole bound](../../../../../subset-sum-pigeonhole-bound.md). The weaker estimate $\sum_{s\in S}s\leq7\cdot16=112$ would also suffice, since $128>113$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
