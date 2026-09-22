<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $f^\lambda$ be the number of [standard tableaux](../../../../../standard-young-tableau.md) of shape $\lambda$. First the associated [polytabloids](../../../../../polytabloid.md) are linearly independent. Order [tabloids](../../../../../tabloid.md) lexicographically by reading each row after sorting its entries. For a column-increasing tableau $t$, the term $\{t\}$ in $e_t$ has coefficient one; every other [tabloid](../../../../../tabloid.md) term has larger row word. To see this, take the first row changed by a nontrivial column permutation. Earlier rows are fixed entry by entry, since each entry belongs to one original column. The changed row can only receive entries from lower positions of those increasing columns, so after sorting it is lexicographically larger. In a linear relation between standard [polytabloids](../../../../../polytabloid.md), choose the smallest row word with a nonzero coefficient. Its own [tabloid](../../../../../tabloid.md) coefficient cannot be cancelled by a larger standard [polytabloid](../../../../../polytabloid.md), a contradiction. Thus $\dim S^\lambda\ge f^\lambda$.

Work first over $\mathbb C$. The [RSK](../../../../../robinson-schensted-knuth-correspondence.md) bijection between permutations and pairs of [standard tableaux](../../../../../standard-young-tableau.md) of the same shape gives $\sum_{\lambda\vdash n}(f^\lambda)^2=n!$. The assumed pairwise nonisomorphic irreducible [Specht modules](../../../../../specht-module.md), and the decomposition of the [regular representation](../../../../../regular-representation.md) with irreducible multiplicities equal to their dimensions, give $\sum_\lambda(\dim S^\lambda)^2\le n!$. Combining the two inequalities forces equality term by term: $\dim S^\lambda=f^\lambda$. Hence the independent standard [polytabloids](../../../../../polytabloid.md) are a **[basis](../../../../../basis.md)**.

The same conclusion holds over every characteristic-zero [field](../../../../../field.md). All [polytabloid](../../../../../polytabloid.md) coordinates in the [tabloid](../../../../../tabloid.md) [basis](../../../../../basis.md) are integers, so the ranks of their coordinate [matrices](../../../../../matrix.md) are the same over any characteristic-zero [field](../../../../../field.md) as over $\mathbb C$. In particular the [dimension](../../../../../dimension-vector-space.md) equality and independence transfer without requiring an embedding of the whole [field](../../../../../field.md) into $\mathbb C$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
