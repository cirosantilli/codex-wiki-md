<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The conditional mean estimator is the [posterior mean](../../../../../../posterior-mean.md)

$$
\boxed{\widehat u_{\mathrm{CM}}(m)=\mathbb E[u\mid m]
=\int_{\mathbb R^d}u\pi^m(u)\,du,}
$$

provided the first [moment](../../../../../../moment.md) is finite. A [maximum a posteriori estimate](../../../../../../maximum-a-posteriori-estimate.md) is any maximizer of the [posterior density](../../../../../../posterior-density.md) relative to [Lebesgue measure](../../../../../../lebesgue-measure.md):

$$
\boxed{\widehat u_{\mathrm{MAP}}(m)\in\operatorname*{arg\,max}_{u\in\mathbb R^d}\pi^m(u).}
$$

Existence of the [posterior density](../../../../../../posterior-density.md) alone does not guarantee a finite [posterior mean](../../../../../../posterior-mean.md) or existence of a maximizing point.

For the stated [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) and independent standard [Gaussian noise](../../../../../../gaussian-noise.md), the negative log of the [posterior density](../../../../../../posterior-density.md), up to a constant, is

$$
\frac12\|m-Au\|^2+\frac12u^T\Sigma^{-1}u.
$$

Its [precision matrix](../../../../../../precision-matrix.md) $A^TA+\Sigma^{-1}$ is a [positive-definite matrix](../../../../../../positive-definite-matrix.md), so [Gaussian conjugacy for a normal linear model](../../../../../../gaussian-conjugacy-for-a-normal-linear-model.md) gives

$$
\boxed{\widehat u_{\mathrm{CM}}=(A^TA+\Sigma^{-1})^{-1}A^Tm
=\Sigma A^T(A\Sigma A^T+I_k)^{-1}m.}
$$

The two forms agree because

$$
(A^TA+\Sigma^{-1})\Sigma A^T=A^T(A\Sigma A^T+I_k).
$$

The [covariance matrix](../../../../../../covariance-matrix.md) is $(A^TA+\Sigma^{-1})^{-1}$, and the [maximum a posteriori estimate](../../../../../../maximum-a-posteriori-estimate.md) equals the [posterior mean](../../../../../../posterior-mean.md) for this [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 350](../../../paper-350-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
