<h1 id="6/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $\Phi\alpha=\sum_i\alpha_i\phi(X_i)$. By the definition of the [kernel matrix](../../../../../../../kernel-matrix.md),

$$
\lVert\Phi\alpha\rVert_{\mathcal H}^2=\alpha^TK\alpha
$$

and

$$
\frac1n\sum_{j=1}^n
\langle\Phi\alpha,\phi(X_j)\rangle_{\mathcal H}^2
=\frac1n\alpha^TK^2\alpha.
$$

The irrelevant positive factor $1/n$ gives exactly the stated constrained optimization.

Let $Kv_1=\lambda_1v_1$, where $\lambda_1>0$ is the largest [eigenvalue](../../../../../../../eigenvalue.md) and $\lVert v_1\rVert_2=1$. The generalized [Rayleigh quotient](../../../../../../../rayleigh-quotient.md) is maximized by

$$
\widehat\alpha=\frac{v_1}{\sqrt{\lambda_1}},
$$

up to sign and addition of a vector in $\ker K$, which does not change $\widehat u=\Phi\widehat\alpha$. Repeated leading eigenvectors give further principal directions.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Paper 218](../../../../paper-218-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
