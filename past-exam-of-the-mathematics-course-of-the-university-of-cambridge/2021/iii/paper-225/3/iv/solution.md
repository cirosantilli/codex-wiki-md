<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The common eigenbasis gives

$$
C_1^{1/2}\phi_k=\sqrt{\lambda_k}\phi_k,\qquad
C_2^{1/2}\phi_k=\sqrt{\lambda_k^*}\phi_k.
$$

Consequently

$$
\boxed{d_R(C_1,C_2)^2
=\sum_{k=1}^\infty(\sqrt{\lambda_k}-\sqrt{\lambda_k^*})^2}.
$$

For the positive square-root factors, the singular values of $C_2^{1/2}C_1^{1/2}$ are $\sqrt{\lambda_k\lambda_k^*}$, so

$$
d_P(C_1,C_2)^2
=\sum_k\lambda_k+\sum_k\lambda_k^*
-2\sum_k\sqrt{\lambda_k\lambda_k^*}
=d_R(C_1,C_2)^2.
$$

**Thus the distances coincide when the covariance operators commute and share an eigenbasis.**

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
