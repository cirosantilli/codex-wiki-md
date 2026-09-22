<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the balancing fact proved by the exchange argument in part d: every leaf of an optimal tree has depth $s-1$ or $s$. A [full binary tree](../../../../../../full-binary-tree.md) with this property has all $2^{s-1}$ possible vertices at level $s-1$; at least one of these is split into two deepest leaves. Thus

$$
2^{s-1}<m\le2^s.
$$

These inequalities characterize the maximum [codeword length](../../../../../../codeword-length.md) exactly:

$$
\boxed{s=\lceil\log_2m\rceil.}
$$

In the suggested notation $m=a2^k$, $1\le a<2$, this is $s=k$ for $a=1$ and $s=k+1$ for $1<a<2$. The distinction at a power of two is important.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
