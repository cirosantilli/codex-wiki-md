<h1 id="15/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For conditionally independent binary labels, the [likelihood](../../../../../likelihood-function.md) is

$$
L(\mathbf w)=\prod_{i=1}^{m} h_i^{y_i}(1-h_i)^{1-y_i},\qquad
h_i=h(\mathbf z_i;\mathbf w).
$$

Maximizing it is equivalent to minimizing its negative [log-likelihood](../../../../../log-likelihood.md), the mean [binary cross-entropy](../../../../../binary-cross-entropy.md):

$$
\boxed{\mathcal L(\mathbf w)=-\frac1m\sum_{i=1}^{m}
[y_i\log h_i+(1-y_i)\log(1-h_i)].}
$$

It is the loss implied by a [Bernoulli distribution](../../../../../bernoulli-distribution.md) for each target, penalizes confident errors strongly and is convex in the linear-logistic parameters. For numerical stability, each contribution can be evaluated as $\log(1+e^{u_i})-y_i u_i$ using a stable softplus implementation.

The 10:90 class imbalance does not invalidate this [likelihood](../../../../../likelihood-function.md). Class weighting or resampling may be useful if errors have unequal costs, but changes the training objective and potentially the interpretation of fitted [probabilities](../../../../../probability.md). Optional [ridge regression](../../../../../ridge-regression.md) adds $\lambda\|\mathbf w\|^2/2$, usually excluding the intercept, to control overly large weights or complete separation.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
