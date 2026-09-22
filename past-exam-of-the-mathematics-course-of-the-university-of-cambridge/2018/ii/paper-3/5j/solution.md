<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

Treat the cell counts as independent [Poisson random variables](../../../../../poisson-distribution.md). Under independence of Month and Hospital, the [independence log-linear model for a two-way contingency table](../../../../../independence-log-linear-model-for-a-two-way-contingency-table.md) is

$$
\log\mu_{ij}=\lambda+\alpha_i+\beta_j,
$$

with no Month–Hospital interaction. Compare its [Poisson deviance](../../../../../poisson-deviance.md) with the appropriate upper quantile of a [chi-squared distribution](../../../../../chi-squared-distribution.md). This is the [likelihood-ratio test of independence in a contingency table](../../../../../likelihood-ratio-test-of-independence-in-a-contingency-table.md).

The approximation assumes independent counts with correctly specified Poisson means, identifiable parameters, and sufficiently large fitted cell means for the asymptotic chi-squared law to be accurate. Equivalently, one may condition on the margins and use the corresponding multinomial sampling formulation.

For the $12\times3$ month table there are $36$ cells and $1+11+2=14$ independent model parameters, so the residual [degrees of freedom](../../../../../degree-of-freedom.md) are

$$
(12-1)(3-1)=22.
$$

Since

$$
28.51836<\chi^2_{22,0.99}=40.29,
$$

**model 1 does not reject Month–Hospital independence at the $1\%$ level.**

After combining months into four quarters, the table is $4\times3$, giving

$$
(4-1)(3-1)=6
$$

degrees of freedom. Now

$$
17.9181>\chi^2_{6,0.99}=16.81,
$$

so **model 2 rejects Quarter–Hospital independence at the $1\%$ level.**

There is no contradiction. Relabelling twelve months as four quarters aggregates the [contingency table](../../../../../contingency-table.md), changes the null hypothesis, and reduces the degrees of freedom. The quarter-level hospital pattern is coherent enough to cross the much lower six-degree-of-freedom threshold even though the more detailed month-level omnibus test does not. This is an instance of how [aggregation can change a contingency-table independence test](../../../../../aggregation-can-change-a-contingency-table-independence-test.md).

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
