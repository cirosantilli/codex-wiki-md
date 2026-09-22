<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The first output uses the equal-variance, pooled [Student's t-test](../../../../../student-s-t-test.md), as shown by its seven [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md). Its exact model assumes two independent samples from [normal distributions](../../../../../normal-distribution.md), with means $\mu_X,\mu_Y$ and a common unknown [variance](../../../../../variance-split.md) $\sigma^2$. The hypotheses are $H_0:\mu_X=\mu_Y$ against $H_1:\mu_X<\mu_Y$. The [sample means](../../../../../sample-mean.md) are $\bar x=4.35$ and $\bar y=9.88$, and the unbiased within-sample [sample variances](../../../../../sample-variance.md) are

$$
s_X^2=4.356667,\qquad s_Y^2=8.822.
$$

The [pooled sample variance](../../../../../pooled-sample-variance.md) and its resulting [standard error](../../../../../standard-error.md) are

$$
s_p^2=\frac{3s_X^2+4s_Y^2}{7}=6.908286,\qquad
\operatorname{se}(\bar X-\bar Y)=s_p\sqrt{\frac14+\frac15}=1.763159.
$$

Hence

$$
\boxed{T=\frac{4.35-9.88}{1.763159}=-3.136416.}
$$

To justify its reference distribution, under the null $(\bar X-\bar Y)/(\sigma\sqrt{1/4+1/5})$ is standard normal, while $(3s_X^2+4s_Y^2)/\sigma^2$ is $\chi^2_7$, independently of the two [sample means](../../../../../sample-mean.md). Dividing the first variable by the square root of the second divided by seven gives the [exact pooled two-sample t statistic](../../../../../exact-pooled-two-sample-t-statistic.md), with [Student t-distribution](../../../../../student-s-t-distribution.md) $t_7$. Its one-sided [p-value](../../../../../p-value.md) is the lower tail

$$
\boxed{\Pr\{t_7\le-3.136416\}=0.0082307.}
$$

The associated one-sided 95% [confidence interval](../../../../../confidence-interval.md) for $\mu_X-\mu_Y$ is

$$
\boxed{\left(-\infty,\;\bar x-\bar y+t_{7,0.95}s_p\sqrt{1/4+1/5}\right)=(-\infty,-2.189557).}
$$

The printed missing lower bound means that this is a one-sided upper confidence limit, not that a finite lower endpoint should be estimated. With such small samples the normality and common-variance assumptions matter; a Welch analysis would use a different [variance](../../../../../variance-split.md) estimate and generally different degrees of freedom.

The second output is the [Wilcoxon rank sum test](../../../../../mann-whitney-u-test.md) for two independent continuous samples. Under a common-distribution [null hypothesis](../../../../../null-hypothesis.md), labels are exchangeable conditional on the pooled values, so the four ranks assigned to the first sample form a uniformly chosen four-element subset of $\{1,\ldots,9\}$. The first sample receives ranks $2,1,3,5$, giving raw rank sum

$$
\boxed{W_X=2+1+3+5=11.}
$$

Equivalently the [Mann–Whitney U test](../../../../../mann-whitney-u-test.md) statistic is $U_X=W_X-4\cdot5/2=1$, the number of cross-sample pairs with an $X$ observation larger than a $Y$ observation. This output reports the raw rank sum, rather than the shifted statistic used by some software.

A first sample tending to be smaller has a small rank sum. Under the null, all $\binom94=126$ rank allocations have equal [probability](../../../../../probability.md). Only $\{1,2,3,4\}$ and $\{1,2,3,5\}$ have rank sum at most 11. By the [exact rank-sum tail one above the minimum](../../../../../exact-rank-sum-tail-one-above-the-minimum.md), the exact lower-tail [p-value](../../../../../p-value.md) is

$$
\boxed{\Pr(W_X\le11)=\frac2{126}=0.0158730.}
$$

No large-sample normal approximation or continuity correction is involved; the absence of ties makes this simple enumeration valid. For a common-shape location-shift family, the test's alternative is a negative location shift of $X$ relative to $Y$. Without that model, the null is equality of distributions and the rank comparison is not simply a test of equality of means or [medians](../../../../../median.md).

**Both tests reject at the 5% level in the direction of smaller $X$ observations; only the pooled t-test rejects at 1%.** The t-test uses the numerical spacing and targets a mean difference under its normal model. The rank-sum test uses ordering and an exact exchangeability calculation, avoiding the normality and common-normal-variance assumptions. Their different [p-values](../../../../../p-value.md) therefore reflect both different statistics and different modelling assumptions, not a numerical contradiction.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
