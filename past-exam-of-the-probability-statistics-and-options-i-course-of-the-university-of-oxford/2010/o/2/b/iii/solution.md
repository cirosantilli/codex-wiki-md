<h1 id="o/2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

With independent Gaussian errors, maximizing the [likelihood](../../../../../../likelihood-function.md) over $\alpha,\beta$ minimizes the residual sum of squares, so the [maximum-likelihood estimators](../../../../../../maximum-likelihood-estimator.md) are the same as least squares. The [invariance property of maximum likelihood estimation](../../../../../../invariance-property-of-maximum-likelihood-estimation.md) gives

$$
\widehat E_t=\widehat\alpha+(e^{-t}-c)\widehat\beta.
$$

The two estimates have zero [covariance](../../../../../../covariance.md) by part (ii). Therefore

$$
\boxed{\operatorname{Var}(\widehat E_t)=\sigma^2\left[\frac1n+
\frac{(e^{-t}-c)^2}{\sum_i(e^{-t_i}-c)^2}\right].}
$$

This is the uncertainty in the estimated expected response. Estimating an additional noisy observation would add its own error [variance](../../../../../../variance-split.md), but the quantity requested is the [mean](../../../../../../expected-value-split.md) response $E_t$.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [O](../../../../o.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options I course of the University of Oxford](../../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
