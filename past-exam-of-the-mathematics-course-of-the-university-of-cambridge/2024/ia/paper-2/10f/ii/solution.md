<h1 id="10f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

When exactly $n-j$ faces have appeared, there are $j$ unseen faces, so each new roll discovers one with probability $j/n$. Let $G_j$ be the number of further rolls needed at that stage. Then

$$
G_j\sim\operatorname{Geom}\left(\frac jn\right),
\qquad j=n,n-1,\ldots,1.
$$

These waiting times concern disjoint successive blocks of independent rolls, so they are independent. Thus the [coupon collector problem](../../../../../../coupon-collector-problem.md) has the decomposition

$$
\boxed{T_n=\sum_{j=1}^nG_j}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
