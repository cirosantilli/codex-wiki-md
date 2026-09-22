<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $w_i=1/v_i$ for the inverse within-study [variances](../../../../../../variance-split.md), and $m=21$. For [Cochran's Q statistic](../../../../../../cochran-s-q-statistic.md), the [DerSimonian–Laird estimator](../../../../../../dersimonian-laird-estimator.md) of the between-study [variance](../../../../../../variance-split.md) is

$$
\widehat\tau^2=\max\left\{0,\frac{Q-(m-1)}{C}\right\},\qquad
C=\sum_iw_i-\frac{\sum_iw_i^2}{\sum_iw_i}
=400-\frac{16000}{400}=360.
$$

Consequently **the estimated heterogeneity variance and standard deviation are**

$$
\boxed{\widehat\tau^2=\frac{38-20}{360}=0.05,\qquad
\widehat\tau=\sqrt{0.05}=0.2236.}
$$

These describe dispersion of underlying study [log odds ratios](../../../../../../log-odds-ratio.md), not ordinary sampling error of a single trial. The [between-study heterogeneity](../../../../../../between-study-heterogeneity.md) is additional to the within-study [variances](../../../../../../variance-split.md).

The [I-squared statistic](../../../../../../i-squared-statistic.md) is

$$
\boxed{I^2=\max\left\{0,\frac{Q-(m-1)}Q\right\}\times100\%
=\frac{18}{38}\times100\%=47.37\%.}
$$

It estimates the share of variation beyond that expected from sampling error in this collection of studies. Approximately half the variation is attributed to heterogeneity on that scale; this is neither the percentage of trials with different effects nor a percentage change in mortality. The PDF omits the symbol naming its heterogeneity estimate, so both $\widehat\tau^2$ and $\widehat\tau$ are reported explicitly.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
