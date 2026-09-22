<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Assume the known [covariance matrix](../../../../../../covariance-matrix.md) $\Sigma$ is [positive definite](../../../../../../positive-definite-matrix.md). The [Gaussian likelihood](../../../../../../gaussian-likelihood.md), up to constants, is

$$
\ell(\beta)=-\tfrac12(Y-X\beta)^T\Sigma^{-1}(Y-X\beta).
$$

Its gradient is $X^T\Sigma^{-1}(Y-X\beta)$. The negative [Hessian matrix](../../../../../../hessian-matrix.md) $X^T\Sigma^{-1}X$ is [positive definite](../../../../../../positive-definite-matrix.md) because $X$ has [full column rank](../../../../../../full-column-rank.md). Thus the unique [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is the [generalized least squares](../../../../../../generalized-least-squares.md) estimator

$$
\boxed{\widehat\beta_{\mathrm{GLS}}=(X^T\Sigma^{-1}X)^{-1}X^T\Sigma^{-1}Y.}
$$

It is unbiased, and multiplication of its linear coefficient matrix by $\Sigma$ gives

$$
\boxed{\operatorname{Cov}(\widehat\beta_{\mathrm{GLS}})=(X^T\Sigma^{-1}X)^{-1}.}
$$

In fact $\widehat\beta_{\mathrm{GLS}}\sim N_p(\beta,(X^T\Sigma^{-1}X)^{-1})$. Equivalently, a [whitening transformation](../../../../../../whitening-transformation.md) premultiplies $Y$ and $X$ by $\Sigma^{-1/2}$, after which [ordinary least squares](../../../../../../ordinary-least-squares.md) applies. There is no extra $\sigma^2$ factor when $\Sigma$ is the complete known covariance; such a factor appears if only a shape matrix $\Omega$ is known and $\Sigma=\sigma^2\Omega$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
