<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Define $R=\sum_i(Y_i-\overline Y)^2$ and $s_Y^2=R/(n-1)$, with $n\geq2$. The unrestricted [maximum-likelihood estimates](../../../../../maximum-likelihood-estimator.md) are $\widehat\mu=\overline Y$ and $\widehat\sigma^2=R/n$. Under the [null hypothesis](../../../../../null-hypothesis.md), maximizing the [normal distribution](../../../../../normal-distribution.md)'s [likelihood](../../../../../likelihood-function.md) over the remaining [variance](../../../../../variance-split.md) gives

$$
\widehat\sigma_0^2=\frac1n\sum_i(Y_i-\mu_0)^2
=\frac Rn+(\overline Y-\mu_0)^2,
$$

because the cross term vanishes when $\sum_i(Y_i-\overline Y)=0$. At either fitted [variance](../../../../../variance-split.md), the exponential factor in the [likelihood function](../../../../../likelihood-function.md) is $e^{-n/2}$, so it cancels in the ratio:

$$
\lambda=\left(\frac{\widehat\sigma^2}{\widehat\sigma_0^2}\right)^{n/2}
=\left(1+\frac{n(\overline Y-\mu_0)^2}{R}\right)^{-n/2}.
$$

The standardized [test statistic](../../../../../test-statistic.md) is

$$
\boxed{t=\frac{\sqrt n(\overline Y-\mu_0)}{s_Y},\qquad
\lambda=\left(1+\frac{t^2}{n-1}\right)^{-n/2}.}
$$

The sample [variance](../../../../../variance-split.md) $s_Y^2$ uses divisor $n-1$, whereas the [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) uses divisor $n$; this explains the $n-1$ in the final expression. Under a nondegenerate [normal distribution](../../../../../normal-distribution.md), $R>0$ with [probability](../../../../../probability.md) one.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
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
