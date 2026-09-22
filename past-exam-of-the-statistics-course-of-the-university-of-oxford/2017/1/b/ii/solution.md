<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $z=z_{1-\alpha/2}$ be the $(1-\alpha/2)$ [standard normal quantile](../../../../../standard-normal-quantile.md). Since $\widehat\mu$ is a [consistent estimator](../../../../../consistency-statistics.md), [Slutsky's theorem](../../../../../slutsky-theorem.md) gives

$$
\frac{\sqrt{3n}(\widehat\mu-\mu)}{\widehat\mu}\xrightarrow dN(0,1).
$$

Its estimated [standard error](../../../../../standard-error.md) is $\widehat\mu/\sqrt{3n}$, giving the approximate $(1-\alpha)$ [Wald confidence interval](../../../../../wald-confidence-interval.md)

$$
\boxed{\left[\widehat\mu\left(1-\frac z{\sqrt{3n}}\right),\quad
\widehat\mu\left(1+\frac z{\sqrt{3n}}\right)\right]\cap(0,\infty).}
$$

For each fixed $\mu>0$, this procedure's [coverage probability](../../../../../coverage-probability.md) tends to $1-\alpha$. Intersecting with the positive parameter space preserves coverage of the true positive value.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
