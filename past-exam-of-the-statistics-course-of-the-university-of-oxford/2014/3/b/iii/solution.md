<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $F$ be the [cumulative distribution function](../../../../../cumulative-distribution-function.md) of a [gamma distribution](../../../../../gamma-distribution.md) with shape $A=a+\sum_ix_i$ and rate $B=b+n$; explicitly,

$$
F(t)=\frac{B^A}{\Gamma(A)}\int_0^t u^{A-1}e^{-Bu}\,du\quad(t\geq0).
$$

The [posterior distribution](../../../../../bayesian-posterior.md) is continuous and has positive density on $(0,\infty)$, so its [quantiles](../../../../../quantile-function.md) give the requested [equal-tailed credible interval](../../../../../equal-tailed-credible-interval.md):

$$
\boxed{[F^{-1}(\alpha/2),\ F^{-1}(1-\alpha/2)].}
$$

Equivalently, $2B\theta\mid x\sim\chi^2_{2A}$, so the endpoints can be written as the corresponding [chi-squared distribution](../../../../../chi-squared-distribution.md) quantiles divided by $2B$. Either form excludes posterior [probability](../../../../../probability.md) $\alpha/2$ from each tail.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
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
