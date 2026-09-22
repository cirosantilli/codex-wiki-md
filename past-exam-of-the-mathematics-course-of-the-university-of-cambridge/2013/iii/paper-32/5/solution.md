<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [log-rank test](../../../../../log-rank-test.md) compares survival experience through the allocation of events within the successive [risk sets](../../../../../risk-set.md). Its null is equal [hazard functions](../../../../../hazard-function.md) between the groups over follow-up, with independent individuals and noninformative censoring within groups. At each distinct event time $t_j$, let $n_{Aj},n_{Bj}$ be the numbers at risk immediately before that time, and let $d_{Aj},d_{Bj}$ be event counts. Under the null, conditional on the total $d_j=d_{Aj}+d_{Bj}$, the expected number of A events is $e_{Aj}=d_jn_{Aj}/(n_{Aj}+n_{Bj})$.

The signed [log-rank statistic](../../../../../log-rank-statistic.md) is the observed-minus-expected score

$$
U_A=\sum_j(d_{Aj}-e_{Aj}).
$$

A positive score indicates relatively more A events than expected, hence a higher event hazard for A; B's score is its negative. Censoring times do not produce score terms, but remove people from all later [risk sets](../../../../../risk-set.md).

At each event time the conditional null allocation is [hypergeometric](../../../../../hypergeometric-distribution.md), as if the $d_j$ events were sampled without replacement from the [risk set](../../../../../risk-set.md). Its [variance](../../../../../variance-split.md) gives the score-increment [variance](../../../../../variance-split.md), with the finite-population correction for ties. Summing these conditional [variances](../../../../../variance-split.md) gives $V$, since distinct-time martingale score increments have zero cross covariance under the null. For sufficiently many informative events, $U_A/\sqrt V$ is approximately standard normal and $U_A^2/V$ approximately chi-squared with one degree of freedom. In the no-tie case, each [variance](../../../../../variance-split.md) contribution is $n_{Aj}n_{Bj}/(n_{Aj}+n_{Bj})^2$. A time at which only one group remains at risk contributes no comparative information.

The numerical parts below report signed-score and [variance](../../../../../variance-split.md) contributions after day 160. They cannot be added as separate chi-squared statistics to the earlier follow-up: **add the scores and [variances](../../../../../variance-split.md) first, and standardize once for the complete dataset**. The [log-rank test](../../../../../log-rank-test.md) is particularly effective for proportional hazards alternatives; crossing hazards can produce cancelling score contributions.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
