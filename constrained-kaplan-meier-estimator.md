<h1 id="constrained-kaplan-meier-estimator">Constrained Kaplan–Meier estimator</h1>

↑ **Parent:** [Kaplan–Meier estimator](kaplan-meier-estimator.md)

The [Kaplan–Meier estimator](kaplan-meier-estimator.md) constrained to have [survivor function](survival-function.md) value $p\in(0,1)$ at $t$ maximizes the right-[censoring](censoring-statistics.md) [log-likelihood](log-likelihood.md) $\sum_j[d_j\log q_j+(n_j-d_j)\log(1-q_j)]$ subject to the displayed constraint. Here $q_j$ is the [discrete hazard](discrete-hazard.md), $d_j$ the event count and $n_j$ the [risk set](risk-set.md) size. In an interior event-time solution, a [Lagrange multiplier](lagrange-multiplier.md) gives $q_j=d_j/(n_j+\lambda)$ before the constrained time, with $q_j=d_j/n_j$ afterwards. The multiplier is chosen to satisfy the product constraint. It is essential to allow a zero-event jump at the constrained time or another relevant cell boundary: a constraint can require mass outside observed event times. A general implementation instead maximizes the concave probability-mass [log-likelihood](log-likelihood.md) with total mass one and mass above $t$ equal to $p$, allowing all relevant cells and a terminal tail. This also handles unobserved tails and boundary solutions without imposing unjustified event-only support.

## ↑ Ancestors (6)

1. [Kaplan–Meier estimator](kaplan-meier-estimator.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-44/3/solution.md)
