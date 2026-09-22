<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Z=(Z_1,\ldots,Z_p)^T$. Independence of the standard [normal distributions](../../../../../../normal-distribution.md) gives $\mathbb EZ=0$, $\operatorname{Cov}(Z)=I_p$, and joint density

$$
f_Z(z)=(2\pi)^{-p/2}\exp(-z^Tz/2).
$$

Choose a matrix $C$ with $CC^T=\Sigma$, for example the lower-triangular factor from the [Cholesky decomposition](../../../../../../cholesky-decomposition.md). It exists and is nonsingular because $\Sigma$ is a [symmetric positive-definite matrix](../../../../../../symmetric-positive-definite-matrix.md). Then the required simulation is

$$
\boxed{X=\mu+CZ.}
$$

It has mean $\mu$ and [covariance matrix](../../../../../../covariance-matrix.md) $CC^T=\Sigma$, and every linear combination of its coordinates is Gaussian, so it has the required [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md).

For the [multivariate normal density](../../../../../../multivariate-normal-density.md), apply the [change of variables formula](../../../../../../change-of-variables-formula.md) to $z=C^{-1}(x-\mu)$. Its absolute Jacobian determinant is $|\det C|^{-1}=|\Sigma|^{-1/2}$, and

$$
z^Tz=(x-\mu)^TC^{-T}C^{-1}(x-\mu)=(x-\mu)^T\Sigma^{-1}(x-\mu).
$$

Hence

$$
\boxed{f_X(x)=\frac{1}{(2\pi)^{p/2}|\Sigma|^{1/2}}\exp\left[-\frac12(x-\mu)^T\Sigma^{-1}(x-\mu)\right],\qquad x\in\mathbb R^p.}
$$

The nonsingularity assumption is needed for a density with respect to $p$-dimensional Lebesgue measure.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
