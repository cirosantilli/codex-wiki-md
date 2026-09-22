<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [bounding number](../../../../../../bounding-number.md) $\mathfrak b$ is the least size of an unbounded family in $(\omega^\omega,\le^*)$. The [almost disjointness number](../../../../../../almost-disjointness-number.md) $\mathfrak a$ is the least size of an infinite [maximal almost disjoint family on omega](../../../../../../maximal-almost-disjoint-family-on-omega.md) of infinite [subsets](../../../../../../subset.md) of $\omega$. Requiring the family to be infinite excludes trivial finite maximal partitions.

A countable family $\{f_i:i<\omega\}$ is bounded by $g(n)=1+\max_{i\le n}f_i(n)$. Thus $\aleph_1\le\mathfrak b$.

Suppose an infinite [almost disjoint family on omega](../../../../../../almost-disjoint-family-on-omega.md) $\mathcal A$ has size less than $\mathfrak b$. Choose distinct members $A_n$ and put $C_n=A_n\setminus\bigcup_{i<n}A_i$. These are infinite and pairwise disjoint. For each $B\in\mathcal A$, define $h_B(n)=\max((B\cap C_n)\cup\{0\})$ whenever the intersection is finite. If $B=A_n$ at the exceptional index $n$, [set](../../../../../../set-split.md) $h_B(n)=0$. These are the only possible infinite intersections. A single $g$ eventually dominates every $h_B$, because there are fewer than $\mathfrak b$ of them. Pick $x_n\in C_n$ with $x_n>g(n)$ and put $X=\{x_n:n<\omega\}$.

For $B$ not among the selected $A_n$, only finitely many $x_n$ can lie in $B$. The same is true for $B=A_j$, with its single exceptional index $j$ ignored. Thus $X$ is infinite and almost disjoint from every member of $\mathcal A$, so the family was not maximal. This [bounding-to-almost-disjointness inequality](../../../../../../bounding-to-almost-disjointness-inequality.md) proves $\mathfrak b\le\mathfrak a$.

Finally start with an infinite pairwise disjoint family and use [Zorn's lemma](../../../../../../zorn-s-lemma.md) to extend it to a [maximal almost disjoint family on omega](../../../../../../maximal-almost-disjoint-family-on-omega.md). It is a family of [subsets](../../../../../../subset.md) of $\omega$, so has [cardinality](../../../../../../cardinality.md) at most $2^{\aleph_0}$. Therefore

$$
\boxed{\aleph_1\le\mathfrak b\le\mathfrak a\le2^{\aleph_0}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
