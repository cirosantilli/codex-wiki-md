<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [log-rank test](../../../../../log-rank-test.md) compares event counts with their conditional expectations under equal group [hazard functions](../../../../../hazard-function.md), using the individuals currently in each [risk set](../../../../../risk-set.md). Assume the usual [independent censoring](../../../../../independent-censoring.md) conditions and [independent](../../../../../independent-random-variables.md) strata. At pooled event time $t_j$, let $n_{Aj},n_{Bj}$ be the group numbers at risk, $n_j=n_{Aj}+n_{Bj}$, and let $d_{Aj},d_{Bj}$ be the event counts with total $d_j$. Under the [null hypothesis](../../../../../null-hypothesis.md), conditioning on the risk counts and total events gives the [hypergeometric distribution](../../../../../hypergeometric-distribution.md)

$$
\Pr(d_{Aj}=k\mid n_{Aj},n_{Bj},d_j)
=\frac{\binom{n_{Aj}}k\binom{n_{Bj}}{d_j-k}}{\binom{n_j}{d_j}}.
$$

Thus the null expected A count and its conditional [variance](../../../../../variance-split.md) are

$$
E_j=d_j\frac{n_{Aj}}{n_j},\qquad
V_j=\frac{d_j n_{Aj}n_{Bj}(n_j-d_j)}{n_j^2(n_j-1)}.
$$

When there is only one person at risk, the event allocation is deterministic and its variance is zero. The unstandardized [log-rank statistic](../../../../../log-rank-statistic.md) is $U=\sum_j(d_{Aj}-E_j)$, with variance estimate $V=\sum_jV_j$. Under standard large-sample conditions, $U/\sqrt V$ is approximately standard normal under the null; the test detects systematic group differences in event rates. It is particularly effective for proportional-hazards alternatives, while crossing effects can cancel in the score.

For a [stratified log-rank statistic](../../../../../stratified-log-rank-statistic.md), construct these [risk sets](../../../../../risk-set.md) and observed-minus-expected differences separately within each stratum $s$, then sum:

$$
U=\sum_s U_s,\qquad V=\sum_s V_s.
$$

This allows different baseline [hazard functions](../../../../../hazard-function.md) between strata and avoids comparing an event with individuals in another stratum. The null is equal A and B hazards within each stratum, together with a censoring mechanism that does not invalidate the within-risk-set comparison.

In a paired stratum, both individuals initially form the [risk set](../../../../../risk-set.md). A first event while both are still observed gives one nontrivial event allocation. After either individual leaves, every subsequent event is certain to belong to the only remaining group and has observed count equal to expected count. Therefore **each pair supplies at most one informative table**. A pair supplies none if the first exit is censoring before either observed event, if neither has an event during their joint follow-up, or if both fail simultaneously so that the tied event allocation is fixed. An event-censoring tie needs a specified convention; with events processed before same-time censoring, the other individual remains at risk for that event and the pair is informative. The untied continuous-time case avoids this ambiguity.

If A has the informative first event, the table at that time is

$$
\begin{array}{c|cc|c}
&\text{event}&\text{no event at this time}&\text{at risk}\\\hline
A&1&0&1\\
B&0&1&1\\\hline
\text{total}&1&1&2
\end{array}
$$

The phrase in the second column refers only to this event time; it does not mean that B can never fail. The expected A count is $1\cdot1/2=1/2$, so this table contributes $1-1/2=1/2$ to $U$, with [variance](../../../../../variance-split.md) $1/4$. An informative B-first pair contributes $-1/2$. All other tables contribute zero. Therefore the requested unnormalized score is

$$
\boxed{U=\frac{d_A-d_B}{2},\qquad V=\frac{d_A+d_B}{4}.}
$$

A positive score means more observed early events on A. There is no need to standardize it to answer the question.

To obtain an exact conditional law, put $m=d_A+d_B$. Under the within-pair equal-hazard null, conditional on an event while both are at risk, either subject supplies it with probability $1/2$. Equivalently, before the pair's first exit, the cause-specific event intensities for A and B are equal; integration over the common period of joint observation gives equal probabilities for the two informative outcomes. This argument requires noninformative observation of the failure process, not just equality of unadjusted marginal survival curves. Different [independent](../../../../../independent-random-variables.md) pairs then have independent fair signs when informative. Conditioning on the set of informative pairs gives $m$ independent Bernoulli outcomes with probability $1/2$; conditioning only on their count mixes identical binomial laws and gives the same result:

$$
\boxed{d_A=U+\frac m2\ \Bigm|\ m\ \sim\operatorname{Binomial}(m,1/2).}
$$

This proves the [paired log-rank reduction to a sign test](../../../../../paired-log-rank-reduction-to-a-sign-test.md). The conditional mass function is $\binom mk2^{-m}$, $0\leq k\leq m$, so an exact two-sided [p-value](../../../../../p-value.md) sums the masses for $k$ with $|2k-m|\geq|d_A-d_B|$. If $m=0$, there is no information for a treatment comparison. Failure-time distances beyond their ordering play no role in this paired score.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
