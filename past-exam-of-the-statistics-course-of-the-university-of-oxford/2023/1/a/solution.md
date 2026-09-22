<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Sort the observations into [order statistics](../../../../order-statistic.md) $x_{(1)}\leq\cdots\leq x_{(n)}$. Choose [plotting positions](../../../../plotting-position.md) $p_i=(i-1/2)/n$ and calculate the [standard normal quantiles](../../../../standard-normal-quantile.md) $z_i=\Phi^{-1}(p_i)$. The [normal Q-Q plot](../../../../normal-q-q-plot.md) consists of the pairs $(z_i,x_{(i)})$.

If the [normal distribution](../../../../normal-distribution.md) model is appropriate, the points should lie approximately on a straight line with positive slope, because its population [quantile function](../../../../quantile-function.md) is

$$
Q(p)=\mu+\sigma\Phi^{-1}(p).
$$

The intercept is approximately $\mu$ and the slope approximately $\sigma$; neither needs to be known in advance. The reference need not be the identity line. One justification is the [probability integral transform](../../../../probability-integral-transform.md): for an independent normal [statistical sample](../../../../statistical-sample.md), $\Phi((X_{(i)}-\mu)/\sigma)$ are uniform [order statistics](../../../../order-statistic.md), whose typical values are near their [plotting positions](../../../../plotting-position.md). The equality is approximate for a finite sample, particularly at the extremes. Systematic curvature, unusually heavy tails, or isolated extreme departures argue against the proposed distributional shape. A straight marginal [Q-Q plot](../../../../q-q-plot.md) does not itself establish [independence](../../../../independent-random-variables.md) of observations.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the statistics course of the University of Oxford](../../../split.md)
5. [Statistics course of the University of Oxford](../../../../statistics-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
