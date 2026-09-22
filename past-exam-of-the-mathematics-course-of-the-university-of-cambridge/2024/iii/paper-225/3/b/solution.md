<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For factorizations $C_i=L_iL_i^*$ and $C_j=L_jL_j^*$, the [Procrustes distance between covariance operators](../../../../../../procrustes-distance-between-covariance-operators.md) is the following infimum over unitary operators $R$:

$$
d_P(C_i,C_j)=\inf_R\lVert L_i-L_jR\rVert_{\mathrm{HS}}.
$$

Unitary invariance of the Hilbert-Schmidt norm gives

$$
\lVert L_i-L_jR\rVert_{\mathrm{HS}}^2
=\lVert L_i\rVert_{\mathrm{HS}}^2+\lVert L_j\rVert_{\mathrm{HS}}^2
-2\operatorname{Re}\operatorname{tr}(L_i^*L_jR).
$$

The [polar decomposition of a bounded operator](../../../../../../polar-decomposition-of-a-bounded-operator.md) and trace duality imply

$$
\sup_R\operatorname{Re}\operatorname{tr}(L_i^*L_jR)
=\lVert L_j^*L_i\rVert_1
=\sum_{k=1}^{\infty}\sigma_k,
$$

where the last equality expresses the [trace norm](../../../../../../trace-norm.md) as the sum of the [singular values](../../../../../../singular-value.md). Taking the infimum proves

$$
\boxed{d_P(C_i,C_j)^2
=\lVert L_i\rVert_{\mathrm{HS}}^2+\lVert L_j\rVert_{\mathrm{HS}}^2-2\sum_{k=1}^{\infty}\sigma_k.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
