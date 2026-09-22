<h1 id="17h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the weighted loss, the [Bayes estimator under parameter-weighted squared error](../../../../../../bayes-estimator-under-parameter-weighted-squared-error.md) is the mean of the posterior after multiplication by

$$
\theta^{\alpha-1}(1-\theta)^{\beta-1}.
$$

Since the original posterior density is proportional to

$$
\theta^X(1-\theta)^{n-X},
$$

the reweighted density is $\operatorname{Beta}(X+\alpha,n-X+\beta)$. Its mean gives

$$
\widetilde\theta=\frac{X+\alpha}{n+\alpha+\beta}.
$$

Writing this in the required form,

$$
\boxed{
\widetilde\theta
=w\widehat\theta+(1-w)\theta_0,
\qquad
w=\frac n{n+\alpha+\beta},
\qquad
\theta_0=\frac{\alpha}{\alpha+\beta}
}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [17H](../../17h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
