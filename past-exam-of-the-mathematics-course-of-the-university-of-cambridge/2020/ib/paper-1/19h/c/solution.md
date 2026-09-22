<h1 id="19h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The scaled maximum

$$
U=\frac{M}{2\theta}=\frac{\widehat\theta}{\theta}
$$

has [cumulative distribution function](../../../../../../cumulative-distribution-function.md) $\mathbb P(U\le u)=u^n$ for $0\le u\le1$. Thus

$$
\mathbb E[U]=\frac n{n+1},
\qquad
\mathbb E[U^2]=\frac n{n+2}.
$$

The [mean squared error](../../../../../../mean-squared-error.md) of the maximum likelihood estimator is therefore

$$
\operatorname{MSE}(\widehat\theta)
=\theta^2\mathbb E[(U-1)^2]
=\boxed{\frac{2\theta^2}{(n+1)(n+2)}}.
$$

Each $X_i$ from the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $[0,2\theta]$ has mean $\theta$ and variance $\theta^2/3$. The sample mean is unbiased and has variance $\theta^2/(3n)$, hence

$$
\boxed{\operatorname{MSE}(\widetilde\theta)=\frac{\theta^2}{3n}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
