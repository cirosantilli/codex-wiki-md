<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

Write $Y_i$ for the request count on day $i$. Both fits are [Poisson regression](../../../../../poisson-regression.md) models with independent

$$
Y_i\sim\operatorname{Poisson}(\lambda_i).
$$

In model 1,

$$
\log\lambda_i=\beta_0+\beta_WW_i+\beta_EE_i+\beta_BB_i
+\beta_LL_i+\beta_MM_i,
$$

where the variables are [indicator variables](../../../../../indicator-variable.md) for winter, weekend, bank holiday, and low or medium pollution; non-winter weekdays that are not bank holidays and have high pollution form the baseline. Model 2 imposes

$$
H_0:\quad\beta_B=\beta_L=\beta_M=0,
$$

retaining only winter and weekend effects.

The models are nested, and the [likelihood-ratio test statistic](../../../../../likelihood-ratio-test-statistic.md) is the decrease in residual deviance,

$$
316.39-304.97=11.42.
$$

There are three restrictions. By [Wilks theorem](../../../../../wilks-theorem.md), under $H_0$ this statistic is asymptotically a [chi-squared distribution](../../../../../chi-squared-distribution.md) with three degrees of freedom. Since

$$
11.42>\chi^2_{3,0.99}=11.34487,
$$

**we reject model 2 at the $1\%$ level in favour of model 1.**

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
