<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $S=\sum_i(x_i-\bar x)^2$ and $q=S/\sigma_0^2$. Under the [null hypothesis](../../../../../null-hypothesis.md), maximizing over the nuisance [mean](../../../../../expected-value-split.md) gives $\widehat\mu_0=\bar x$. The unrestricted [normal mean and variance maximum-likelihood estimators](../../../../../normal-mean-and-variance-maximum-likelihood-estimators.md) are $\widehat\mu=\bar x$, $\widehat{\sigma^2}=S/n$. Thus, for $S>0$,

$$
\lambda(\boldsymbol x)=\frac{(2\pi\sigma_0^2)^{-n/2}e^{-S/(2\sigma_0^2)}}{(2\pi S/n)^{-n/2}e^{-n/2}}
=\boxed{\left(\frac qn\right)^{n/2}e^{(n-q)/2}}.
$$

The [likelihood-ratio test statistic](../../../../../likelihood-ratio-test-statistic.md) is consequently

$$
\boxed{W=-2\log\lambda=q-n-n\log(q/n)}.
$$

The usual model assumes $n\geq2$. The event $S=0$ has [probability](../../../../../probability.md) zero under a nondegenerate [normal distribution](../../../../../normal-distribution.md); at that observation the unrestricted likelihood is unbounded as the variance tends to zero, and the ratio has limiting value zero. This is the [likelihood-ratio test for a normal variance](../../../../../likelihood-ratio-test-for-a-normal-variance.md) with unknown mean.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
