<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a [proportional hazards model](../../../../../../proportional-hazards-model.md), individual $i$ has

$$
h_i(t)=h_0(t)\exp(x_i^T\beta).
$$

The exponential term is the hazard multiplier relative to the [baseline hazard](../../../../../../baseline-hazard.md) $h_0$. With $h_0$ unspecified, the [Cox partial likelihood](../../../../../../cox-partial-likelihood.md) multiplies, over event times, the failing subject's multiplier divided by the sum of multipliers in the current risk set. After estimating $\beta$, the [Breslow estimator](../../../../../../breslow-estimator.md) is

$$
\widehat H_0(t)=\sum_{t_j\leq t}
\frac{d_j}{\sum_{i\in R_j}\exp(x_i^T\widehat\beta)}.
$$

A [Stratified Cox model](../../../../../../stratified-cox-model.md) uses a separate baseline hazard $h_{0s}$ for each stratum but a common $\beta$. Its partial likelihood is the product of within-stratum partial likelihoods, and a separate integrated baseline hazard is estimated in each stratum.

In a matched pair, the only informative comparison occurs while both members remain at risk. If the exposed member fails first, the pair contributes $e^\beta/(1+e^\beta)$; if the unexposed member fails first, it contributes $1/(1+e^\beta)$. A censoring as the first recorded time gives no informative failure comparison, and any later one-person risk set contributes one. With only two observations per stratum, each stratum supplies almost no information about its arbitrary baseline hazard, so a useful common integrated baseline-hazard estimate is generally unavailable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
