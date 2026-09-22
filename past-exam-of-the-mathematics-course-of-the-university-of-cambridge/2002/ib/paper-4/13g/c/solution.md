<h1 id="13g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let the finite [poles](../../../../../../pole.md) be $a_1,\ldots,a_N$. Their [Laurent series](../../../../../../laurent-series.md) have finite principal parts $P_j(z)=\sum_{k=1}^{m_j}c_{jk}(z-a_j)^{-k}$. Subtracting them removes all finite singularities: $h=f-\sum_jP_j$ is entire. Each $P_j$ tends to zero at infinity, so $h$ still has at most a finite-order [pole](../../../../../../pole.md) at infinity.

The Laurent expansion of $h(1/w)$ near $w=0$ has only finitely many negative powers. Thus $h(z)=P(z)+c+O(z^{-1})$ for large $|z|$, with $P$ a [polynomial](../../../../../../polynomial-split.md). The entire function $h-P$ is bounded outside a large disk and, by continuity, on that disk. [Liouville's theorem](../../../../../../liouville-theorem.md) makes it constant. Consequently

$$
f(z)=P(z)+c+\sum_{j=1}^N\sum_{k=1}^{m_j}\frac{c_{jk}}{(z-a_j)^k}.
$$

Combining denominators gives **a [rational function](../../../../../../rational-function.md) $p/q$**. This proves that [meromorphic functions on the sphere are rational](../../../../../../meromorphic-functions-on-the-sphere-are-rational.md) without assuming rationality at the start.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13G](../../13g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
