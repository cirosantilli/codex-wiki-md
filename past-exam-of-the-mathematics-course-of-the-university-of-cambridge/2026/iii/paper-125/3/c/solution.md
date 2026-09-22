<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because the [canonical height of an elliptic curve](../../../../../../canonical-height-of-an-elliptic-curve.md) is a quadratic form, polarization makes

$$
B(P,Q)=\widehat h(P+Q)-\widehat h(P)-\widehat h(Q)
$$

a symmetric bilinear form on the free part of the [Mordell-Weil group](../../../../../../mordell-weil-group.md). If $P'_i=\sum_jU_{ij}P_j$ is another integral basis, then $U\in\operatorname{GL}_r(\mathbb Z)$ and the Gram matrices satisfy

$$
M'=UMU^T.
$$

Since $\det U=\pm1$, their determinants agree. Thus the [regulator of an elliptic curve](../../../../../../regulator-of-an-elliptic-curve.md) is independent of the chosen basis.

Now let $Q_1,\ldots,Q_r$ be a basis for the free part of $E'(\mathbb Q)$. The images $\phi(P_i)$ span a finite-index sublattice, so modulo torsion

$$
\phi(P_i)=\sum_jA_{ij}Q_j
$$

for an integral matrix $A$ with nonzero determinant. The height identity gives

$$
B'(\phi P_i,\phi P_j)=\deg(\phi)B(P_i,P_j).
$$

Taking determinants in the two descriptions of this Gram matrix yields

$$
(\det A)^2\operatorname{Reg}(E'/\mathbb Q)
=\deg(\phi)^r\operatorname{Reg}(E/\mathbb Q).
$$

**Therefore the required formula holds with $d=(\det A)^{-1}\in\mathbb Q^\times$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
