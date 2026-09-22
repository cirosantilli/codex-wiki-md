<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [proportional hazards model](../../../../../../proportional-hazards-model.md) assigns individual $i$ the [hazard function](../../../../../../hazard-function.md) $h_i(t)=h_0(t)\phi_i$, where $h_0$ is the [baseline hazard](../../../../../../baseline-hazard.md) for multiplier one and $\phi_i>0$ is a time-constant [hazard multiplier](../../../../../../hazard-multiplier.md). In a [Cox proportional-hazards model](../../../../../../cox-proportional-hazards-model.md), $\phi_i=e^{x_i^T\beta}$ for a [covariate](../../../../../../covariate.md) vector $x_i$ and coefficient vector $\beta$; ratios $h_i(t)/h_k(t)=\phi_i/\phi_k$ are constant whenever the baseline is nonzero.

Assume [independent](../../../../../../independent-random-variables.md) individuals, [independent censoring](../../../../../../independent-censoring.md) conditional on the [covariates](../../../../../../covariate.md), and no tied events. Immediately before an event at $t$, condition on its observed [risk set](../../../../../../risk-set.md) $R(t)$ and one event in a small time interval. The individual event [probability](../../../../../../probability.md) is $h_0(t)\phi_i\,dt+o(dt)$, while the total is $h_0(t)\sum_{k\in R(t)}\phi_k\,dt+o(dt)$. Their limiting ratio is $\phi_i/\sum_{k\in R(t)}\phi_k$. Multiplication over observed events gives the [Cox partial likelihood](../../../../../../cox-partial-likelihood.md)

$$
L_p(\beta)=\prod_{j:\text{event}}\frac{\phi_{i_j}}{\sum_{k\in R(t_j)}\phi_k}.
$$

The unspecified [baseline hazard](../../../../../../baseline-hazard.md) cancels. This is the usual successive conditional event contribution defining the [partial likelihood](../../../../../../partial-likelihood.md), not the full event-time likelihood conditioned simultaneously on all event times.

For the four individuals the successive event [risk sets](../../../../../../risk-set.md) are $\{a,b,c,d\}$, $\{c,d\}$ and $\{d\}$. Individual $b$ leaves at its [right censoring](../../../../../../right-censoring.md) time and contributes no event numerator. Consequently

$$
\boxed{L_{a,b,c,d}=\frac{\phi_a}{\phi_a+\phi_b+\phi_c+\phi_d}\frac{\phi_c}{\phi_c+\phi_d}\frac{\phi_d}{\phi_d}=\frac{\phi_a\phi_c}{(\phi_a+\phi_b+\phi_c+\phi_d)(\phi_c+\phi_d)}.}
$$

The last event contributes one and carries no further relative-risk information.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
