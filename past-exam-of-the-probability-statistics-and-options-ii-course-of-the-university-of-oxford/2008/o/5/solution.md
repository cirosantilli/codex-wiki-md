<h1 id="o/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a sample size $m\ge2$ define $\overline X=m^{-1}\sum_iX_i$ and $S_X^2=(m-1)^{-1}\sum_i(X_i-\overline X)^2$. The normal-sample theorem gives

$$
\boxed{\overline X\sim N(\mu_X,\sigma^2/m),\qquad\frac{(m-1)S_X^2}{\sigma^2}\sim\chi^2_{m-1},\qquad c=\frac{m-1}{\sigma^2}.}
$$

It also states that the mean and [sample variance](../../../../sample-variance.md) are [independent](../../../../independent-random-variables.md). Combining (i) and (ii), and the [independence](../../../../independent-random-variables.md) across samples, the correctly centred pivot is

$$
\boxed{T_0=\frac{\overline X-\overline Y-(\mu_X-\mu_Y)}{S\sqrt{1/m+1/n}}\sim t_{m+n-2}.}
$$

The source reverses the mean difference inside the subtraction. Its literal statistic is generally noncentral when $\mu_X\ne\mu_Y$, rather than having a central Student distribution. Under the [null hypothesis](../../../../null-hypothesis.md) both differences are zero, so this misprint does not change the requested null test.

For a two-sided level-$\alpha$ test reject when $|T|>t_{m+n-2,1-\alpha/2}$. In the numerical example the pooled [variance](../../../../variance-split.md) is $0.038$, the standard error is $\sqrt{0.038(2/5)}\approx0.12329$, and $T\approx-2.190$. There are eight [degrees of freedom](../../../../degree-of-freedom.md) and the supplied critical value is $2.31$. Thus **do not reject equal mean cell volume at the 5% level**. This does not establish equality of the means; it states that the observed difference does not cross this test's two-sided threshold.

Age [matching](../../../../matching-graph-theory-split.md) introduces a shared block factor: the two observations in a pair can be associated, and their age-dependent means also undermine the simple unblocked [independent](../../../../independent-random-variables.md)-samples model. A **[paired t-test](../../../../paired-t-test.md)** on the within-pair drug-minus-placebo differences accounts for that design, assuming [independent](../../../../independent-random-variables.md) pairs and the corresponding normal-difference model. Shared age [variation](../../../../variation.md) cancels in those differences; positive within-pair association reduces their [variance](../../../../variance-split.md) and can increase [power](../../../../power-function-of-a-statistical-test.md), although the reduction in [degrees of freedom](../../../../degree-of-freedom.md) means improvement is not automatic. The paired test cannot be computed from the two marginal means and [variances](../../../../variance-split.md) alone: the within-pair differences or [covariance](../../../../covariance.md) are needed.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [O](../../o.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
