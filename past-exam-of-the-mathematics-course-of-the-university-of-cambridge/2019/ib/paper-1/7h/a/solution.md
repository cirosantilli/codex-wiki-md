<h1 id="7h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For observations $x_1,\ldots,x_n$, the [log-likelihood](../../../../../../log-likelihood.md) of the [normal distribution](../../../../../../normal-distribution.md) model is

$$
\ell(\mu,\sigma^2)
=-\frac n2\log(2\pi\sigma^2)
-\frac1{2\sigma^2}\sum_{i=1}^n(x_i-\mu)^2.
$$

Differentiating first with respect to $\mu$ gives $\widehat\mu=\overline x$. Substituting this value and differentiating with respect to $\sigma^2$ gives the [normal mean and variance maximum-likelihood estimators](../../../../../../normal-mean-and-variance-maximum-likelihood-estimators.md)

$$
\boxed{\widehat\mu=\overline X=\frac1n\sum_{i=1}^nX_i,
\qquad
\widehat{\sigma}^2=\frac1n\sum_{i=1}^n(X_i-\overline X)^2}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
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
