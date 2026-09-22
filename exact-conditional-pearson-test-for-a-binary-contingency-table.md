# Exact conditional Pearson test for a binary contingency table

↑ **Parent:** [Pearson chi-squared statistic for contingency tables](pearson-chi-squared-statistic-for-contingency-tables.md)

Consider independent [binomial counts](binomial-count.md) $X_i\sim\operatorname{Bin}(n_i,p)$ under the common-probability [null hypothesis](null-hypothesis.md), with fixed positive row sizes $n_i$. Let $N=\sum_i n_i$, $K=\sum_i X_i$ and assume $0<K<N$. Conditional on $K$, the [probability mass function](probability-mass-function.md) is the displayed [multivariate hypergeometric distribution](multivariate-hypergeometric-distribution.md): in the joint likelihood, the factor $p^K(1-p)^{N-K}$ is common to all admissible tables and cancels. The [Vandermonde identity](vandermonde-s-identity.md) gives the denominator, so the conditional distribution is free of the unknown [nuisance parameter](nuisance-parameter.md) $p$.

For a table $x$, its [Pearson chi-squared statistic](pearson-chi-squared-statistic.md) is

$$
Q(x)=\sum_i\frac{(Nx_i-n_iK)^2}{n_iK(N-K)}.
$$

An exact conditional [p-value](p-value.md) sums the displayed probabilities over all tables with the same margins and $Q(x)\ge Q(x_{\rm obs})$. The ordering is by the [Pearson chi-squared statistic](pearson-chi-squared-statistic.md), rather than by the probability of an individual table; different exact-test orderings can give different answers. Enumeration is practical when $K$ and the number of rows are small. [Monte Carlo tests](monte-carlo-test.md) can approximate the same tail by sampling tables with fixed margins.[Details: simulated contingency-table tests sample tables with fixed marginals and use the Pearson statistic](pearson-s-chi-squared-test-for-count-data-in-the-r-documentation.md)

An exact arithmetic comparison is easy too. Let $M$ be the [least common multiple](least-common-multiple.md) of the row sizes. Compare the [integer](integer-split.md)

$$
A(x)=\sum_i(Nx_i-n_iK)^2\frac{M}{n_i},
$$

since every table has the same positive denominator $MK(N-K)$. This includes boundary ties without a floating-point tolerance. Conditional [p-values](p-value.md) are discrete and can be conservative; “exact” concerns their null calibration, not equality of rejection probability with every chosen [significance level](significance-level.md).

## ↑ Ancestors (9)

1. [Pearson chi-squared statistic for contingency tables](pearson-chi-squared-statistic-for-contingency-tables.md)
2. [Pearson chi-squared test of homogeneity](pearson-chi-squared-test-of-homogeneity.md)
3. [Statistical hypothesis test](statistical-hypothesis-test-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2022/3/solution.md)
