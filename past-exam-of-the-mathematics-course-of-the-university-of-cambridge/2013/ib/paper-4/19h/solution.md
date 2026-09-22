<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

A [sufficient statistic](../../../../../sufficient-statistic.md) is one for which the conditional distribution of the full sample, given its value, is independent of the parameter. For independent observations the likelihood is $\prod_{i=1}^6p_i^{n_i}$, depending on the data only through the counts. The [factorization criterion for sufficiency](../../../../../fisher-neyman-factorization-theorem.md) therefore makes $(n_1,\ldots,n_6)$ sufficient. Directly, all ordered samples with given counts have the same probability, so their conditional distribution is uniform over the $n!/\prod n_i!$ possible arrangements, independently of the $p_i$.

The unrestricted [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) is $\widehat p_i=n_i/n$. Thus the [generalized likelihood-ratio test](../../../../../generalized-likelihood-ratio-test.md) uses

$$
\Lambda=\frac{(1/6)^n}{\prod_{i=1}^6(n_i/n)^{n_i}},\qquad D=-2\log\Lambda=2\sum_{i=1}^6n_i\log\frac{6n_i}{n},
$$

with zero-count terms interpreted by continuity. **Reject for small $\Lambda$, equivalently large $D$.**

Write $n_i=n/6+\delta_i$, so $\sum\delta_i=0$. A [Taylor series](../../../../../taylor-series.md) expansion of $(n/6+\delta_i)\log(1+6\delta_i/n)$ gives $\delta_i+3\delta_i^2/n+O(|\delta_i|^3/n^2)$. Summing cancels the linear terms, and yields

$$
D=\frac6n\sum_i\delta_i^2+O\left(\sum_i\frac{|\delta_i|^3}{n^2}\right),\qquad
\frac6n\sum_i\delta_i^2=-n+\frac6n\sum_i n_i^2=T.
$$

Under the [null hypothesis](../../../../../null-hypothesis.md), the [multinomial central limit theorem](../../../../../multinomial-central-limit-theorem.md) places the standardized count deviations in the five-dimensional subspace with coordinate sum zero, with identity covariance on that subspace. Their squared norm consequently tends to the [chi-squared distribution](../../../../../chi-squared-distribution.md) with five degrees of freedom. This gives the [Pearson chi-squared goodness-of-fit test](../../../../../pearson-chi-squared-goodness-of-fit-test.md).

For $T=8.12$, the asymptotic [p-value](../../../../../p-value.md) is about $0.150$. The 5% critical value of $\chi_5^2$ is approximately $11.07$. **Do not reject at the usual 5% level**, or at 10%. A [significance level](../../../../../significance-level.md) is not specified in the paper, so an unconditional yes-or-no decision is not determined: using this approximation, rejection would require a chosen level at least about $15\%$.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
