<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The two rank-one operators have orthogonal ranges. Their Hilbert-Schmidt inner product is zero, while $\lVert C_i\rVert_{\mathrm{HS}}=\lambda_i$, so the [Hilbert-Schmidt distance between covariance operators](../../../../../../hilbert-schmidt-distance-between-covariance-operators.md) is

$$
d_L(C_1,C_2)=\sqrt{\lambda_1^2+\lambda_2^2}.
$$

For each $C_i$, the [positive square root of an operator](../../../../../../positive-square-root-of-an-operator.md) is $C_i^{1/2}=\sqrt{\lambda_i}\,e_i\otimes e_i$. Orthogonality therefore gives the [square-root distance between covariance operators](../../../../../../square-root-distance-between-covariance-operators.md)

$$
d_R(C_1,C_2)=\sqrt{\lambda_1+\lambda_2}.
$$

Finally $C_2^{1/2}C_1^{1/2}=0$, so every singular value in the Procrustes cross-term vanishes. Hence

$$
\boxed{d_P(C_1,C_2)=\sqrt{\lambda_1+\lambda_2}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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
