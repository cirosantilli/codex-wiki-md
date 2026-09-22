<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Every $2\times2$ principal [submatrix](../../../../../../../submatrix.md) of a [kernel matrix](../../../../../../../kernel-matrix.md) is positive semidefinite, so

$$
|k_\tau(x,y)|^2\leq k_\tau(x,x)k_\tau(y,y).
$$

The [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) for integrals therefore gives

$$
\int_{-\infty}^{\infty}|k_\tau(x,y)|\,d\tau
\leq
\left(\int_{-\infty}^{\infty}k_\tau(x,x)\,d\tau\right)^{1/2}
\left(\int_{-\infty}^{\infty}k_\tau(y,y)\,d\tau\right)^{1/2}<\infty.
$$

Thus every entry of $k(x,y)=\int k_\tau(x,y)d\tau$ is well defined. For any finite coefficients $c_r$ and points $x_r$, linearity of the integral gives

$$
\sum_{r,s}c_rc_s k(x_r,x_s)
=\int_{-\infty}^{\infty}\sum_{r,s}c_rc_s k_\tau(x_r,x_s)\,d\tau\geq0,
$$

because the integrand is nonnegative. Hence $k$ is a [positive-semidefinite kernel](../../../../../../../positive-semidefinite-kernel.md). This proves the [integral closure of positive-semidefinite kernels](../../../../../../../integral-closure-of-positive-semidefinite-kernels.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 205](../../../../paper-205-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
