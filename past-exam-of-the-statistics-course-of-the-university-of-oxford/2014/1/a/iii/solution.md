<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Here the [exponential distribution](../../../../../exponential-distribution.md) is parametrized by its [mean](../../../../../expected-value-split.md), so $f(x;\theta)=\theta^{-1}e^{-x/\theta}$ for $x\geq0$ and $\theta>0$. Its [log-likelihood](../../../../../log-likelihood.md) and [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) are

$$
\ell(\theta)=-n\log\theta-\frac{\sum_iX_i}{\theta},\qquad \widehat\theta=\overline X.
$$

For one observation, $\partial_\theta\log f=-1/\theta+X/\theta^2$. Since $\operatorname{Var}(X)=\theta^2$, its [Fisher information](../../../../../fisher-information-matrix.md) is $I_1(\theta)=1/\theta^2$. Consequently the estimated [standard error](../../../../../standard-error.md) is $\overline X/\sqrt n$, giving

$$
\boxed{\left[\overline X\left(1-\frac{z_{1-\alpha/2}}{\sqrt n}\right),\quad
\overline X\left(1+\frac{z_{1-\alpha/2}}{\sqrt n}\right)\right].}
$$

This is a large-sample [confidence interval](../../../../../confidence-interval.md), not an exact one. If its lower endpoint is negative, intersecting with the [parameter space](../../../../../parameter-space.md) $(0,\infty)$ removes impossible values without excluding any possible true [statistical parameter](../../../../../statistical-parameter.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
