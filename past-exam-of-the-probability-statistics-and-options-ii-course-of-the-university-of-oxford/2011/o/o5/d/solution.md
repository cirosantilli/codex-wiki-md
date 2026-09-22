<h1 id="o/o5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $C=(X^TX)^{-1}$ and $\nu=n-p$. The normal law of the estimator gives $(\widehat\theta_i-\theta_i)/(\sigma\sqrt{C_{ii}})\sim N(0,1)$. The fitted and residual Gaussian projections are [orthogonal](../../../../../orthogonal-vectors.md) and hence independent, so this quantity is independent of $\nu s^2/\sigma^2\sim\chi^2_\nu$. Their ratio therefore has [Student's t-distribution](../../../../../student-s-t-distribution.md):

$$
\frac{\widehat\theta_i-\theta_i}{s\sqrt{C_{ii}}}\sim t_\nu.
$$

If $t_{\nu,1-\alpha/2}$ is its upper $1-\alpha/2$ [quantile](../../../../../quantile-function.md), rearranging its central [probability](../../../../../probability.md) event gives

$$
\boxed{\left[\widehat\theta_i-t_{\nu,1-\alpha/2}s\sqrt{C_{ii}},\quad
\widehat\theta_i+t_{\nu,1-\alpha/2}s\sqrt{C_{ii}}\right].}
$$

This interval has exact coverage $1-\alpha$ under the given normal linear model, rather than merely large-sample coverage.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [O5](../../o5.md)
3. [O](../../../o.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
