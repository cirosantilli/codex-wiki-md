<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an ascending [sorted array](../../../../../sorted-array.md), maintain a candidate interval $[\ell,r]$ initially containing every index. Compare the target with the middle entry at $m=\lfloor(\ell+r)/2\rfloor$. Equality returns $m$; if the target is smaller, replace $r$ by $m-1$; if larger, replace $\ell$ by $m+1$. An empty interval reports absence.

The [loop invariant](../../../../../loop-invariant.md) is that any target occurrence still possible lies inside the candidate interval. [Sortedness](../../../../../sortedness.md) justifies discarding the appropriate half after each unequal comparison. The interval length decreases to at most half its previous length, establishing termination and correctness. After $t$ unsuccessful comparisons there are at most $n/2^t$ candidates, so at most $\lfloor\log_2n\rfloor+1$ comparisons suffice for $n\ge1$. Each iteration uses constant work on a random-access [array](../../../../../array-data-structure.md). Thus **[binary search](../../../../../binary-search.md) takes $O(\log(n+1))$ [running time](../../../../../running-time.md)**, conventionally written $O(\log n)$ for nontrivial input sizes. Empty input is handled in constant time.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
