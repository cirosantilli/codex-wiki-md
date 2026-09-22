<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $\sigma,\tau>0$ to be the positive standard deviations. Multiply the normal [likelihood function](../../../../../likelihood-function.md) by the normal [prior density](../../../../../prior-density.md). Terms independent of $\theta$ can be absorbed into the normalizing constant:

$$
\pi(\theta\mid x)\propto
\exp\!\left[-\frac1{2\sigma^2}\sum_i(x_i-\theta)^2
-\frac{\theta^2}{2\tau^2}\right].
$$

The identity $\sum_i(x_i-\theta)^2=\sum_i(x_i-\overline x)^2+n(\theta-\overline x)^2$ makes the quadratic term explicit. Completing the square gives

$$
\pi(\theta\mid x)\propto\exp\!\left[-\frac{(\theta-\mu_n)^2}{2v_n}\right],
$$

where

$$
\boxed{v_n=\left(\frac n{\sigma^2}+\frac1{\tau^2}\right)^{-1}
=\frac{\sigma^2\tau^2}{\sigma^2+n\tau^2},\qquad
\mu_n=\frac{n\tau^2}{\sigma^2+n\tau^2}\overline x.}
$$

Thus $\theta\mid x\sim N(\mu_n,v_n)$. This is [normal-normal conjugacy](../../../../../normal-normal-conjugacy-with-known-observation-variance.md): prior and data precisions add, and the [posterior mean](../../../../../posterior-mean.md) shrinks the [sample mean](../../../../../sample-mean.md) towards the prior mean zero.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
