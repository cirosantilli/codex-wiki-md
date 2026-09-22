<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $\alpha=\log\{\beta^{(1)}/\beta^{(0)}\}$ and absorb the common multiplier into $h_0(t)=m(t)\beta^{(0)}$. The model becomes

$$
h_j(t)=h_0(t)e^{\alpha g_j}.
$$

It is a [Cox proportional-hazards model](../../../../../../cox-proportional-hazards-model.md); the unknown baseline does not need a parametric form. The equality hypothesis is precisely $\alpha=0$. The absolute multipliers and $m$ have a scale ambiguity, but their [hazard ratio](../../../../../../hazard-ratio.md) $e^\alpha$ is identifiable when both groups supply information.

For an untied event at $a_k$, let $R_k$ be the [risk set](../../../../../../risk-set.md) just before the event, and let $i_k$ be the subject who fails. The conditional event [probability](../../../../../../probability.md) is proportional to that subject's hazard, so the common baseline cancels:

$$
P_\alpha(i_k\mid R_k,\text{one event})
=\frac{e^{\alpha g_{i_k}}}{\sum_{i\in R_k}e^{\alpha g_i}}.
$$

Multiply these factors to form the [Cox partial likelihood](../../../../../../cox-partial-likelihood.md). One can maximize it and compare its maximum with its value at $\alpha=0$ using a [partial likelihood-ratio test](../../../../../../partial-likelihood-ratio-test.md), or use the corresponding [score test](../../../../../../score-test.md).

Explicitly, with group risk-set sizes $r_{k0},r_{k1}$ and observed event indicator $d_{k1}$ for group 1, the score at zero and its information are

$$
U=\sum_k\left(d_{k1}-\frac{r_{k1}}{r_{k0}+r_{k1}}\right),\qquad
V=\sum_k\frac{r_{k0}r_{k1}}{(r_{k0}+r_{k1})^2}.
$$

Under the null the event label has exactly this [Bernoulli distribution](../../../../../../bernoulli-distribution.md) conditional on its current [risk set](../../../../../../risk-set.md). Hence **$U^2/V$ is the usual one-degree-of-freedom log-rank test statistic**, with an asymptotic [chi-squared distribution](../../../../../../chi-squared-distribution.md) when $V>0$ and enough informative events are observed. Censoring can differ between groups, provided it is independent of event time within the conditioning model. If there are recorded ties, use the appropriate tied-risk-set version: for $d_k$ events the null variance contribution is $d_k(r_k-d_k)r_{k0}r_{k1}/[r_k^2(r_k-1)]$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
