<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [Jackknife resampling](../../../../../../jackknife-resampling.md), calculate the leave-one-out estimates $\widehat\theta_{(-i)}$ by deleting observation $i$, and their average $\overline\theta_J=n^{-1}\sum_i\widehat\theta_{(-i)}$. The [Jackknife variance estimator](../../../../../../jackknife-variance-estimator.md) is

$$
\boxed{\widehat V_J=\frac{n-1}{n}\sum_{i=1}^n(\widehat\theta_{(-i)}-\overline\theta_J)^2.}
$$

The factor $n-1$ compensates for the small differences between the overlapping samples. For sufficiently smooth [statistics](../../../../../../statistic.md) it estimates their [sampling variance](../../../../../../variance-of-an-estimator.md). The related estimated bias is $(n-1)(\overline\theta_J-\widehat\theta)$, leading to the [jackknife bias correction](../../../../../../jackknife-bias-correction.md) $n\widehat\theta-(n-1)\overline\theta_J$.

For the nonparametric [bootstrap](../../../../../../bootstrapping-statistics.md), replace the unknown distribution by its [empirical distribution function](../../../../../../empirical-distribution-function.md)

$$
\boxed{\widehat F_n(t)=\frac1n\sum_{i=1}^n\mathbf1\{x_i\leq t\}.}
$$

Independently sample $n$ observations with replacement from the original observations, compute the [estimator](../../../../../../estimator.md) on that [bootstrap sample](../../../../../../bootstrap-sample.md), and repeat this for $B$ independently generated [bootstrap samples](../../../../../../bootstrap-sample.md). If the resulting values are $\widehat\theta_1^*,\ldots,\widehat\theta_B^*$, estimate the conditional [bootstrap](../../../../../../bootstrapping-statistics.md) variance by

$$
\boxed{\widehat V_B=\frac1{B-1}\sum_{b=1}^B(\widehat\theta_b^*-\overline\theta^*)^2.}
$$

Its interpretation as an approximation to the original [sampling variance](../../../../../../variance-of-an-estimator.md) relies on the [bootstrap](../../../../../../bootstrapping-statistics.md) approximating the sampling law of the [statistic](../../../../../../statistic.md); increasing $B$ only reduces simulation error and cannot repair a failure of that approximation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
