<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The second [logistic regression](../../../../../../../logistic-regression.md) adds $\gamma_2Y_{i,t-2}$ while retaining the first lag and baseline [covariates](../../../../../../../covariate.md). The models are nested under $H_0:\gamma_2=0$. Their [likelihood-ratio test statistic](../../../../../../../likelihood-ratio-test-statistic.md) is the reduction in [binomial deviance](../../../../../../../binomial-deviance.md),

$$
\boxed{2(\widehat\ell_2-\widehat\ell_1)=1164.4-1155.0=9.4.}
$$

Under the null and regular large-sample conditions for the correctly specified conditional [likelihood](../../../../../../../likelihood-function.md), this has an approximate [chi-squared distribution](../../../../../../../chi-squared-distribution.md) with one [statistical degree of freedom](../../../../../../../statistical-degrees-of-freedom.md). Since $9.4>3.841$, reject at 5%; the approximate [p-value](../../../../../../../p-value.md) is $0.0022$. **Prefer the two-lag model to the one-lag model.** Its additional lag captures statistically useful information in the history.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 30](../../../../paper-30-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
