<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

Write $S(\beta)=\sum_{ij}\mu_{ij}(\beta)$. Ignoring only terms independent of $\beta$, the Poisson [log-likelihood](../../../../../log-likelihood.md) is $\ell_P=\sum y_{ij}\log\mu_{ij}-S(\beta)$. The multinomial model is defined on the constraint $S(\beta)=n$, since its probabilities must sum to one. On this constraint its full [log-likelihood](../../../../../log-likelihood.md) satisfies

$$
\ell_M(\beta)=\ell_P(\beta)+n-n\log n+\log(n!),
$$

where both likelihoods include the same $-\sum\log(y_{ij}!)$ terms. Thus they differ by a constant on the admissible multinomial parameter set.

If the Poisson [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) has $S(\widehat\beta)=n$, it is feasible for the multinomial problem, and no feasible parameter can have a larger likelihood than it. Consequently it is also a multinomial maximum. With the usual uniqueness and identifiability assumption,

$$
\boxed{\widehat\beta=\beta^*,\qquad\widehat y_{ij}=y^*_{ij}.}
$$

Without uniqueness, the precise conclusion is that $\widehat\beta$ is a multinomial maximizer; arbitrary independently chosen maximizers need not be identical. This qualification is necessary for a general unspecified parametrization.

In a log-linear [generalized linear model](../../../../../generalized-linear-model.md) with an unrestricted intercept, differentiation with respect to that intercept gives $\sum(y_{ij}-\widehat\mu_{ij})=0$. Thus the fitted total automatically equals $n$. One can fit independent Poisson cell counts using the usual GLM machinery and recover the multinomial fitted probabilities as $\widehat\mu_{ij}/n$. The result is [constrained Poisson and multinomial likelihood equivalence](../../../../../constrained-poisson-and-multinomial-likelihood-equivalence.md), not an assertion that the sampling experiments themselves are identical.

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
