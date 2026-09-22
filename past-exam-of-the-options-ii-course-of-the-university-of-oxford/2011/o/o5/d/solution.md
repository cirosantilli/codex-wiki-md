<h1 id="o/o5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $v_i=[(X^TX)^{-1}]_{ii}>0$. Part (b) gives

$$
Z_i=\frac{\widehat\theta_i-\theta_i}{\sigma\sqrt{v_i}}\sim N(0,1).
$$

The residual vector and coefficient estimator are independent: they are jointly [normal](../../../../../multivariate-normal-distribution.md) and their cross-[covariance matrix](../../../../../covariance-matrix.md) is zero, since $X^T(I-H)=0$. Hence $Z_i$ is independent of $U=(n-p)s^2/\sigma^2\sim\chi^2_{n-p}$. By the definition of [Student's t-distribution](../../../../../student-s-t-distribution.md),

$$
\frac{\widehat\theta_i-\theta_i}{s\sqrt{v_i}}
=\frac{Z_i}{\sqrt{U/(n-p)}}\sim t_{n-p}.
$$

Let $t_{n-p,1-\alpha/2}$ be the $1-\alpha/2$ quantile of this distribution. Inverting the central [probability](../../../../../probability.md) statement gives the exact marginal [confidence interval](../../../../../confidence-interval.md)

$$
\boxed{\widehat\theta_i\ \pm\ t_{n-p,1-\alpha/2}\,s\sqrt{[(X^TX)^{-1}]_{ii}}.}
$$

Its coverage is $1-\alpha$ under the stated [Gaussian linear model](../../../../../normal-linear-model-split.md); simultaneous coverage for all coefficients would require a separate adjustment.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [O5](../../o5.md)
3. [O](../../../o.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
