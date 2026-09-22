<h1 id="29j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiating the [ridge regression](../../../../../../ridge-regression.md) objective gives

$$
\nabla_\theta\bigl(\lVert Y-X\theta\rVert_2^2+\lambda\lVert\theta\rVert_2^2\bigr)
=2(X^TX+\lambda I_p)\theta-2X^TY.
$$

For every nonzero $z$,

$$
z^T(X^TX+\lambda I_p)z=\lVert Xz\rVert_2^2+\lambda\lVert z\rVert_2^2>0,
$$

so $X^TX+\lambda I_p$ is [positive definite](../../../../../../positive-definite-matrix.md) and hence invertible. The strictly convex objective therefore has the unique [closed-form ridge regression estimator](../../../../../../closed-form-ridge-regression-estimator.md)

$$
\boxed{\widehat\theta_\lambda=(X^TX+\lambda I_p)^{-1}X^TY.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29J](../../29j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
