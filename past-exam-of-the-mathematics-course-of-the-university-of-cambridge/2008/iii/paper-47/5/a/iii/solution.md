<h1 id="5/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose an initial $s^{(0)}>0$. At each iteration, evaluate $V$ and $m$ using $s^{(t)}$ and draw $\beta^{(t+1)}$ from the conditional [multivariate normal distribution](../../../../../../../multivariate-normal-distribution.md) just derived. Next compute $b_t=b+\|y-X_k\beta^{(t+1)}\|^2/2$ and draw

$$
s^{(t+1)}\sim\operatorname{IG}(a+n/2,b_t).
$$

For example, generate $G\sim\Gamma(a+n/2,\text{rate }b_t)$ and set $s^{(t+1)}=1/G$. A draw of the conditional [multivariate normal distribution](../../../../../../../multivariate-normal-distribution.md) can be formed as $m+LZ$ with $LL^T=V$ a [Cholesky decomposition](../../../../../../../cholesky-decomposition.md) and $Z$ a vector of independent standard [normal distributions](../../../../../../../normal-distribution.md).

This two-block [Gibbs sampler](../../../../../../../gibbs-sampler.md) alternates the [full conditional distributions](../../../../../../../full-conditional-distribution.md) of the [independent normal and inverse-gamma regression priors](../../../../../../../independent-normal-and-inverse-gamma-regression-priors.md) posterior. The conditional-integration argument proves that its [invariant distribution](../../../../../../../stationary-distribution.md) is the joint [posterior distribution](../../../../../../../bayesian-posterior.md). Under the usual convergence conditions, retain the pairs $(\beta^{(t)},s^{(t)})$ after an initial transient as the requested dependent posterior sample. The new variance update uses the newly drawn coefficients, rather than the previous coefficients.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
