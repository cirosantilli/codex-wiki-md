<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[EM likelihood monotonicity](../../../../../../em-likelihood-monotonicity.md) makes EM an ascent method, not a global-optimization theorem. If the [log-likelihood](../../../../../../log-likelihood.md) is bounded above along the iterates, its nondecreasing values converge. That alone does not show that the parameters converge, nor that any limiting parameter is a global [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md). Under additional regularity, accumulation points can be stationary; local maxima, other stationary points or flat sets can depend on initialization. Multiple starting values and comparison of the achieved observed likelihoods are therefore useful.

The upper-bound hypothesis is substantive. In a [finite mixture model](../../../../../../finite-mixture-model.md) with a freely shrinking normal-component [variance](../../../../../../variance-split.md), placing one component at an observed value can make the [likelihood](../../../../../../likelihood-function.md) unbounded while other components cover the remaining observations. In that situation monotonicity provides no finite maximum to converge to. EM may also improve very slowly, and a small change in [likelihood](../../../../../../likelihood-function.md) alone is not proof of an accurate global solution. The guarantee in part (b) is nondecrease, not strict increase at every iteration.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
