<h1 id="7h/solution">Solution</h1>

↑ **Parent:** [7H](../7h.md)

Let $\bar X=n^{-1}\sum_iX_i$ and $S=\sum_i(X_i-\bar X)^2$. The [Gaussian distribution](../../../../../normal-distribution.md) [likelihood](../../../../../likelihood-function.md) is proportional to $\tau^{n/2}\exp[-\tau\sum_i(X_i-\mu)^2/2]$. Multiplying by the [normal-gamma distribution](../../../../../normal-gamma-distribution.md) prior gives the quadratic exponent $\sum_i(X_i-\mu)^2+K_0(\mu-\mu_0)^2+2\beta_0$. Completing the square,

$$
\sum_i(X_i-\mu)^2+K_0(\mu-\mu_0)^2=(K_0+n)(\mu-\mu_n)^2+S+\frac{K_0n}{K_0+n}(\bar X-\mu_0)^2.
$$

The power of $\tau$ is $\tau^{\alpha_0+n/2-1}\sqrt\tau$, so the [posterior distribution](../../../../../bayesian-posterior.md) has exactly the required family with

$$
\boxed{K_n=K_0+n,\qquad\mu_n=\frac{K_0\mu_0+n\bar X}{K_0+n},\qquad\alpha_n=\alpha_0+\frac n2,}
$$

and

$$
\boxed{\beta_n=\beta_0+\frac12\sum_i(X_i-\bar X)^2+\frac{K_0n}{2(K_0+n)}(\bar X-\mu_0)^2.}
$$

For a proper prior, $K_0,\alpha_0,\beta_0>0$ and $\mu_0\in\mathbb R$. The separate $\sqrt\tau$ factor is retained in both densities; it does not add $1/2$ to the update of $\alpha$. This is a [conjugate prior](../../../../../conjugate-prior.md) for the Gaussian mean and [precision parameter](../../../../../precision-parameter.md).

## ↑ Ancestors (10)

1. [7H](../7h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
