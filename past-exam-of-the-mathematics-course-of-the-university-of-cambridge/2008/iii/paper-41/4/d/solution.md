<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For rare events, $\operatorname{Binomial}(N,\pi)$ is approximately $\operatorname{Poisson}(N\pi)$. The binomial [variance](../../../../../../variance-split.md) is $N\pi(1-\pi)$, close to the Poisson [variance](../../../../../../variance-split.md) $N\pi$, and $\log\{\pi/(1-\pi)\}$ is close to $\log\pi$. Even the largest observed proportion here is below $0.009$. Thus the binomial log-odds model and Poisson log-rate model should give similar fitted counts and tests, as their very similar deviances show.

**Both analyses indicate strong age and adjusted city associations, with no apparent large residual lack of fit.** The binomial model is natural when each person can contribute at most one case during a fixed period and the denominator counts people at risk. A Poisson count model is natural for event counts with an appropriate exposure or person-time denominator; population size is an approximation to such exposure if the observation periods are comparable. An [odds ratio](../../../../../../odds-ratio.md) and a rate ratio are different parameters despite being close in this rare-event setting.

The models both assume a common city effect across ages. An age-by-city [interaction](../../../../../../interaction-statistics.md) can be checked by comparing with the saturated model for the 15 observed cells, using the six additional [degrees of freedom](../../../../../../degree-of-freedom.md); the small final deviances offer no substantial evidence against the additive fits in that comparison. This cannot recover the missing city-by-age cell or eliminate unmeasured [confounding](../../../../../../confounding.md). Nor is choosing the lower of $5.1509$ and $5.21$ a valid model-selection rule: these deviances are measured against saturated models for different response distributions.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
