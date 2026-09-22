<h1 id="1d/solution">Solution</h1>

↑ **Parent:** [1D](../1d.md)

By the [spectral theorem for real symmetric matrices](../../../../../spectral-theorem-for-real-symmetric-matrices.md), choose an [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md) $u_1,u_2,u_3$ with $Au_i=\lambda_i u_i$. If $x=\sum_i y_i u_i$, then

$$
1=x^TAx=\sum_i\lambda_i y_i^2
\leq\lambda_1\sum_i y_i^2=\lambda_1|x|^2.
$$

Thus every point of the [ellipsoid](../../../../../ellipsoid.md) has distance at least $\lambda_1^{-1/2}$ from the origin. Equality holds precisely when

$$
(\lambda_1-\lambda_2)y_2^2+(\lambda_1-\lambda_3)y_3^2=0.
$$

Both coefficients are strictly positive, so $y_2=y_3=0$. The surface equation then gives $y_1=\pm\lambda_1^{-1/2}$. Therefore

$$
\boxed{d_{\min}=\frac1{\sqrt{\lambda_1}},\qquad
x=\pm\frac{u_1}{\sqrt{\lambda_1}}.}
$$

**Exactly two points attain the minimum.** The strict ordering makes the largest-eigenvalue [eigenspace](../../../../../eigenspace.md) one-dimensional; this is the equality case in [nearest points to the origin on a positive-definite ellipsoid](../../../../../nearest-points-to-the-origin-on-a-positive-definite-ellipsoid.md).

## ↑ Ancestors (10)

1. [1D](../1d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
