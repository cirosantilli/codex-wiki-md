<h1 id="8/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The displayed reference to index $n+1$ makes the nontrivial case $0\leq n<k$; at $n=k$ the trees already agree and no further edge exists. Write $F=\{e_1,\ldots,e_n\}$ and $e=e_{n+1}$. If $e\in T'$, its weight is at least the first nonprefix weight $w(e'_{n+1})$ and at most that weight by hypothesis. Thus it ties for the next position, and simply ordering this tie with $e$ first gives the result.

Otherwise add $e$ to $T'$. The resulting [fundamental cycle](../../../../../../fundamental-cycle.md) contains an edge $f\notin F$: if its whole path lay in $F$, then $F\cup\{e\}\subseteq T$ would already contain a cycle. Every edge of $T'\setminus F$, including $f$, has weight at least $w(e'_{n+1})\geq w(e)$. Set $\widetilde T=T'-f+e$.

This is a [spanning tree](../../../../../../spanning-tree.md) and still contains $F$. Its sorted order can begin with the specified prefix and then $e$, because all remaining edges have weight at least $w(e)$ and each prefix weight is at most $w(e)$. Replacing one entry of a multiset by a no-larger entry cannot increase any sorted [order statistic](../../../../../../order-statistic.md): for every threshold, the number of entries below or equal to it cannot decrease. Hence **$w(\widetilde e_j)\leq w(e'_j)$ for every $j$**. Ties may be ordered as needed; the paper prescribes nondecreasing weights, not an immutable global tie-break rule. This is [spanning-tree prefix exchange](../../../../../../spanning-tree-prefix-exchange.md).

## ↑ Ancestors (13)

1. [I](../i.md)
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
