<h1 id="17h/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For

$$
\widetilde\theta=w\frac Xn+(1-w)\theta_0,
$$

the bias and variance are

$$
\mathbb E_\theta\widetilde\theta-\theta
=(1-w)(\theta_0-\theta),
\qquad
\operatorname{Var}_\theta(\widetilde\theta)
=\frac{w^2}{n}\theta(1-\theta).
$$

The [bias-variance decomposition of mean squared error](../../../../../../bias-variance-decomposition-of-mean-squared-error.md) yields

$$
\boxed{
g_{w,\theta_0}(\theta)
=\frac{w^2}{n}\theta(1-\theta)
+(1-w)^2(\theta-\theta_0)^2
}.
$$

This is the risk formula for an [affine shrinkage estimator for a binomial proportion](../../../../../../affine-shrinkage-estimator-for-a-binomial-proportion.md).

## ↑ Ancestors (11)

1. [E](../e.md)
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
