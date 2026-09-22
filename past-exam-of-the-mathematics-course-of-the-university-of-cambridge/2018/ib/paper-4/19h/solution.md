<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

With the uniform prior, the [binomial likelihood](../../../../../binomial-likelihood.md) gives the [Beta distribution](../../../../../beta-distribution.md) posterior $\operatorname{Beta}(s+1,n-s+1)$. Under [squared-error loss](../../../../../squared-error-loss.md), the [Bayes estimator](../../../../../bayes-estimator.md) is the posterior mean:

$$
\boxed{\hat p_G=\frac{s+1}{n+2}.}
$$

The production manager's prior gives posterior density proportional to $p^{s+1}(1-p)^{n-s}$. Minimizing $\mathbb E[(1-p)(\hat p-p)^2\mid X=s]$ gives the weighted posterior mean

$$
\hat p_P=\frac{\mathbb E[p(1-p)\mid X=s]}{\mathbb E[1-p\mid X=s]}
=\boxed{\frac{s+2}{n+4}},
$$

using the supplied [beta function](../../../../../beta-function.md). Cross multiplication shows $\hat p_P>\hat p_G$ exactly when $n>2s$, so it is greater unless **$s\geq n/2$**.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
