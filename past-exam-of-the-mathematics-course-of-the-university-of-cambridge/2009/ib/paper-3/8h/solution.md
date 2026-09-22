<h1 id="8h/solution">Solution</h1>

↑ **Parent:** [8H](../8h.md)

Treat the four fixed row totals as four independent samples from [binomial distributions](../../../../../binomial-distribution.md). Under independence, each has the same unknown probability $p$ of a third-child boy. The pooled [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) is $\widehat p=100/200=1/2$, so each expected cell count is $25$. The [Pearson chi-squared test of homogeneity](../../../../../pearson-chi-squared-test-of-homogeneity.md) statistic is

$$
X^2=\sum_{i=1}^4\left[\frac{(B_i-25)^2}{25}+\frac{(G_i-25)^2}{25}\right]
=\frac{2}{25}(9^2+3^2+0^2+6^2)
=\boxed{10.08}.
$$

There are four independently varying row probabilities under the alternative, and one estimated common probability under the null; the [degrees of freedom](../../../../../degree-of-freedom.md) are therefore $4-1=3$. Equivalently this is the $(4-1)(2-1)$ contingency-table count. The fact that the pooled estimate happens to equal one half does not make it a specified null probability and does not change the [degrees of freedom](../../../../../degree-of-freedom.md) to four.

Since $10.08>7.8147$, **reject independence at the 5% level** using the stated chi-squared calibration. All expected counts are sufficiently large for the usual asymptotic test.

## ↑ Ancestors (10)

1. [8H](../8h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
