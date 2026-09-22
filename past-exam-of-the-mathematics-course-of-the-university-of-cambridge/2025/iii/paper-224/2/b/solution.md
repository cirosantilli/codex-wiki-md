<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The likelihood-ratio event depends only on the type $R=\widehat P_n$ and is

$$
\sum_xR(x)\log\frac{P(x)}{Q(x)}\geq0,
$$

equivalently $D(R\Vert Q)\geq D(R\Vert P)$. This constraint defines a closed subset of the finite probability simplex, so Sanov's upper bound gives the exponent

$$
C(P,Q)=\inf_{R:\,D(R\Vert Q)\geq D(R\Vert P)}D_e(R\Vert Q).
$$

It is strictly positive: the only distribution with zero divergence from $Q$ is $R=Q$, but $Q$ violates the constraint because $0=D(Q\Vert Q)<D(Q\Vert P)$. Compactness and continuity under full support keep the infimum away from zero. This exponent is the [Chernoff information](../../../../../../chernoff-information.md) between $P$ and $Q$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
