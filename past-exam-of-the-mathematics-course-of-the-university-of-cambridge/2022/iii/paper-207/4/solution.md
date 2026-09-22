<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

At event time $t_j$, let $n_{Aj},n_{Bj}$ be the two [risk set](../../../../../risk-set.md) sizes, $n_j=n_{Aj}+n_{Bj}$, and let $d_{Aj},d_{Bj}$ be the event counts with $d_j=d_{Aj}+d_{Bj}$. Under the null hypothesis of equal hazards, conditioning on the risk set and total number of events gives a [hypergeometric distribution](../../../../../hypergeometric-distribution.md), so

$$
e_{Aj}=\mathbb E(d_{Aj})=d_j\frac{n_{Aj}}{n_j},
$$

and

$$
v_{Aj}=\operatorname{Var}(d_{Aj})
=\frac{n_{Aj}n_{Bj}d_j(n_j-d_j)}
{n_j^2(n_j-1)}.
$$

The [log-rank statistic](../../../../../log-rank-statistic.md) and its estimated null variance are

$$
U=\sum_j(d_{Aj}-e_{Aj}),
\qquad
V=\sum_jv_{Aj}.
$$

Under the null, $U/\sqrt V$ is asymptotically standard normal, or $U^2/V$ is asymptotically chi-squared with one degree of freedom.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 207](../../paper-207-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
