<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a [frailty model](../../../../../../frailty-model.md), an individual's unobserved susceptibility to an event is represented by a nonnegative [frailty random variable](../../../../../../frailty-random-variable.md) multiplying that individual's [hazard function](../../../../../../hazard-function.md). Conditional on its value, subjects with the same measured covariates can therefore have different event rates. The frailty is a persistent latent characteristic of the individual, not newly sampled noise at each time.

Here the conditional [hazard function](../../../../../../hazard-function.md) is $u e^{\beta z}h_0(t)$, with [baseline hazard](../../../../../../baseline-hazard.md) $h_0$. A multiplier $u>1$ raises susceptibility and $u<1$ lowers it. Normalization $\mathbb E U=1$ fixes the frailty scale: without it, multiplying every frailty by a constant and dividing the [baseline hazard](../../../../../../baseline-hazard.md) by that constant would give the same individual hazards. The [variance](../../../../../../variance-split.md) of $U$ measures unobserved heterogeneity. An atom at $U=0$, if allowed, would give a permanently zero conditional hazard.

The [hazard ratio](../../../../../../hazard-ratio.md) between groups is $e^\beta$ for individuals compared at the same frailty. It need not equal the population [hazard ratio](../../../../../../hazard-ratio.md), because [survival selection](../../../../../../survival-selection-in-a-heterogeneous-population.md) changes the frailty distribution among those still alive or event-free.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
