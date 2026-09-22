<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under the [null hypothesis](../../../../../../null-hypothesis.md) of consistency, $\widehat\delta_D-\widehat\delta_I$ has approximately zero [expectation](../../../../../../expected-value.md) and [variance](../../../../../../variance-split.md) $v_D+v_I$, since the displayed trials are [independent](../../../../../../independent-random-variables.md). Thus a two-sided [Wald test](../../../../../../wald-test.md) uses

$$
\boxed{Z=\frac{\widehat\delta_D-\widehat\delta_I}{\sqrt{v_D+v_I}}\ \dot\sim\ N(0,1),\qquad Z^2\ \dot\sim\ \chi^2_1.}
$$

The observed difference is $-0.07$, and $Z=-0.07/\sqrt{0.29}\simeq-0.130$. Its two-sided [p-value](../../../../../../p-value.md) is approximately $0.897$, so there is no detectable discrepancy here. Failure to reject is not proof of consistency: this test has limited [statistical power](../../../../../../statistical-power.md), and [transitivity in network meta-analysis](../../../../../../transitivity-in-network-meta-analysis.md) also needs substantive assessment. If evidence sources overlap, replace $v_D+v_I$ by $v_D+v_I-2\operatorname{Cov}(\widehat\delta_D,\widehat\delta_I)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
