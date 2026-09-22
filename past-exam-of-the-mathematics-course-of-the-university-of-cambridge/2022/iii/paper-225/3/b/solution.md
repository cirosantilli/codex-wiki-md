<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an orthogonal $R$, unitary invariance of the [Hilbert-Schmidt norm](../../../../../../hilbert-schmidt-norm.md) gives

$$
\lVert L_1-L_2R\rVert_{\rm HS}^2
=\lVert L_1\rVert_{\rm HS}^2+\lVert L_2\rVert_{\rm HS}^2
-2\operatorname{Re}\operatorname{tr}(R^*L_2^*L_1).
$$

The product $L_2^*L_1$ is trace-class. Its [polar decomposition of a bounded operator](../../../../../../polar-decomposition-of-a-bounded-operator.md) and [trace duality](../../../../../../trace-duality.md) give

$$
\sup_{R\in\mathcal O(H)}
\operatorname{Re}\operatorname{tr}(R^*L_2^*L_1)
=\lVert L_2^*L_1\rVert_1
=\sum_{k=1}^{\infty}\sigma_k,
$$

where $(\sigma_k)$ are its [singular values](../../../../../../singular-value.md). Taking the infimum proves

$$
\boxed{d_P(C_1,C_2)^2
=\lVert L_1\rVert_{\rm HS}^2+\lVert L_2\rVert_{\rm HS}^2
-2\sum_{k=1}^{\infty}\sigma_k.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
