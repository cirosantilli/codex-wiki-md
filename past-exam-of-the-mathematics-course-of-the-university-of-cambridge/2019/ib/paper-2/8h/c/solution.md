<h1 id="8h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For any action $a$, decompose the posterior expected [quadratic loss](../../../../../../squared-error-loss.md) around the [posterior mean](../../../../../../posterior-mean.md):

$$
\mathbb E[(a-\theta)^2\mid X]
=(a-\mathbb E[\theta\mid X])^2+\operatorname{Var}(\theta\mid X).
$$

The unique minimizer is therefore the [Bayes estimator under squared error loss](../../../../../../bayes-estimator-under-squared-error-loss.md). Using the mean of the posterior [Beta distribution](../../../../../../beta-distribution.md) gives

$$
\boxed{\widehat\theta=\mathbb E[\theta\mid X]
=\frac{S+1}{n+2}}.
$$

Under repeated sampling at parameter value $\theta$, $S$ has the [binomial distribution](../../../../../../binomial-distribution.md) with expected value $n\theta$. Consequently

$$
\boxed{\mathbb E_\theta[\widehat\theta]=\frac{n\theta+1}{n+2}},
$$

so its [bias of an estimator](../../../../../../bias-of-an-estimator.md) is $(1-2\theta)/(n+2)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [8H](../../8h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
