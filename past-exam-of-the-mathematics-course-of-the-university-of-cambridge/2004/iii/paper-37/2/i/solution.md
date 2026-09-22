<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Treat the counts as independent [binomial distributions](../../../../../../binomial-distribution.md), $R_i\sim\operatorname{Bin}(n_i,\pi_i)$, conditional on the known numbers of operations. The [null hypothesis](../../../../../../null-hypothesis.md) is that the probabilities $\pi_i$ are all equal, with no assumed numerical value. Centre 4 has no operations in this period and hence contributes [likelihood](../../../../../../likelihood-function.md) one, supplying no information about its mortality [probability](../../../../../../probability.md). The [empty groups in a binomial homogeneity test](../../../../../../empty-groups-in-a-binomial-homogeneity-test.md) principle leaves **11 contributing centres and 10 test degrees of freedom**.

Under the common-probability model the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is

$$
\widehat\pi=\frac{\sum_i r_i}{\sum_i n_i}=\frac{283}{1353}=0.209165.
$$

Use the two-column [contingency table](../../../../../../contingency-table.md) of deaths and survivors, deleting its all-zero row. The [Pearson chi-squared test of homogeneity](../../../../../../pearson-chi-squared-test-of-homogeneity.md) has statistic

$$
X^2=\sum_{i:n_i>0}\left\{\frac{(r_i-n_i\widehat\pi)^2}{n_i\widehat\pi}+\frac{((n_i-r_i)-n_i(1-\widehat\pi))^2}{n_i(1-\widehat\pi)}\right\}
=\sum_{i:n_i>0}\frac{(r_i-n_i\widehat\pi)^2}{n_i\widehat\pi(1-\widehat\pi)}.
$$

Under the null, the large-sample reference distribution is $\chi^2_{10}$. The expected counts are adequate for this approximation here, including at the smallest nonempty centre. Calculating gives

$$
\boxed{X^2=39.3923,\qquad p\approx2.17\times10^{-5}.}
$$

An alternative is the [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) against separate centre probabilities, with [binomial deviance](../../../../../../binomial-deviance.md)

$$
D=2\sum_{i:n_i>0}\left\{r_i\log\frac{r_i}{n_i\widehat\pi}+(n_i-r_i)\log\frac{n_i-r_i}{n_i(1-\widehat\pi)}\right\}.
$$

The unrestricted probabilities are $r_i/n_i$; subtracting one fitted common [probability](../../../../../../probability.md) leaves the same 10 degrees of freedom. Here $D=39.5033$ and $p\approx2.07\times10^{-5}$. Thus **there is strong evidence against a common mortality [probability](../../../../../../probability.md)**. This omnibus test does not identify Centre 1 as the sole source of the heterogeneity. If its comparison with the remaining centres is the primary scientific question, specify a separate planned one-versus-rest comparison; inspection of many pairwise comparisons calls for consideration of [multiple testing](../../../../../../multiple-hypothesis-testing.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
