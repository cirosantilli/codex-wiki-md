<h1 id="8h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $S=\sum_{i=1}^nX_i$ be the number of heads. The [likelihood function](../../../../../../likelihood-function.md) for the [Bernoulli distribution](../../../../../../bernoulli-distribution.md) sample is proportional to $\theta^S(1-\theta)^{n-S}$. A [uniform distribution](../../../../../../continuous-uniform-distribution.md) prior on $[0,1]$ is the $\operatorname{Beta}(1,1)$ distribution, so [Beta-binomial conjugacy](../../../../../../beta-binomial-conjugacy.md) gives the [posterior distribution](../../../../../../bayesian-posterior.md)

$$
\boxed{\theta\mid X_1,\ldots,X_n\sim\operatorname{Beta}(S+1,n-S+1)}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
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
