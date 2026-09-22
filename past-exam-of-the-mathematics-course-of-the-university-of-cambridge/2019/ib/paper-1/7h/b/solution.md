<h1 id="7h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [unbiased estimator](../../../../../../unbiased-estimator.md) $T$ of a parameter $\theta$ satisfies $\mathbb E_\theta[T]=\theta$ for every permissible value of $\theta$. Since the [sample mean](../../../../../../sample-mean.md) is linear,

$$
\mathbb E[\widehat\mu]=\frac1n\sum_{i=1}^n\mathbb E[X_i]=\mu,
$$

so $\widehat\mu$ is unbiased.

Use the identity

$$
\sum_{i=1}^n(X_i-\overline X)^2
=\sum_{i=1}^n(X_i-\mu)^2-n(\overline X-\mu)^2.
$$

The two expectations on the right are $n\sigma^2$ and $n\operatorname{Var}(\overline X)=\sigma^2$, respectively. Hence

$$
\mathbb E[\widehat{\sigma}^2]=\frac{n-1}{n}\sigma^2.
$$

Thus

$$
\boxed{\widehat\mu\text{ is unbiased},
\qquad
\widehat{\sigma}^2\text{ has bias }-\frac{\sigma^2}{n}}.
$$

The unbiased [sample variance](../../../../../../sample-variance.md) instead divides the same sum of squares by $n-1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7H](../../7h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
