<h1 id="8g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Two [matrices](../../../../../../matrix.md) are equivalent when $A'=PAQ$ for invertible [matrices](../../../../../../matrix.md) $P$ and $Q$ of the appropriate sizes. A change of [basis](../../../../../../basis.md) in the codomain multiplies a [matrix](../../../../../../matrix.md) on the left, while a change of [basis](../../../../../../basis.md) in the domain multiplies it on the right. Hence two [matrices](../../../../../../matrix.md) of the same [linear map](../../../../../../linear-map.md) in two pairs of [bases](../../../../../../basis.md) are equivalent.

Conversely, start with the map $\alpha:F^n\to F^m$ having [matrix](../../../../../../matrix.md) $A$ in the standard [bases](../../../../../../basis.md). Given $A'=PAQ$, choose domain and codomain [bases](../../../../../../basis.md) whose change-of-coordinate [matrices](../../../../../../matrix.md) produce $Q$ and $P$; then $A'$ represents the same map in those [bases](../../../../../../basis.md). This proves the equivalence.

The column rank of $A$ is the dimension of the span of its columns, and its row rank is the dimension of the span of its rows. If $A$ represents $\alpha:F^n\to F^m$, its column rank is $\operatorname{rank}\alpha$. The transpose represents the dual map

$$
\alpha^*:(F^m)^*\to(F^n)^*,
\qquad \phi\mapsto\phi\circ\alpha,
$$

so the row rank is $\operatorname{rank}\alpha^*$.

If $\operatorname{rank}\alpha=r$, then

$$
\ker\alpha^*=(\operatorname{im}\alpha)^0,
$$

whose dimension is $m-r$: extend a [basis](../../../../../../basis.md) of $\operatorname{im}\alpha$ to one of $F^m$ and use the dual [basis](../../../../../../basis.md). Rank-nullity now gives $\operatorname{rank}\alpha^*=r$. This proves the [equality of row rank and column rank](../../../../../../equality-of-row-rank-and-column-rank.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8G](../../8g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
