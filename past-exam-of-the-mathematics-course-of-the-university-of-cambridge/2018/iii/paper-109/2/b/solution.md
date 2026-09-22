<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $m=\lceil\log_2n\rceil$ and assign distinct complete [binary sequences](../../../../../../bitstream.md) in $\{0,1\}^m$ to the $n$ points. For each coordinate $i$, let $A_i$ be the points with bit zero and $B_i$ those with bit one. Distinct sequences disagree in some coordinate, so these pairs form a [separating family of disjoint set pairs](../../../../../../separating-family-of-disjoint-set-pairs.md).

Every point lies in exactly one side of every pair, hence the total incidence is $mn$, as allowed when $\lambda=1$. The construction reaches the bound:

$$
\boxed{m_{\min}=\lceil\log_2 n\rceil\quad(\lambda=1).}
$$

The reference to “(i)” in the original PDF's part (b) refers to part (a); the local TeX additionally duplicates that item.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
