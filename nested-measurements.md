# Nested measurements

↑ **Parent:** [Replication in experimental design](replication-in-experimental-design.md)

[Nested measurements](nested-measurements.md) are responses grouped inside larger units, with each measured object belonging to just one such unit. Three [leaves](leaf.md) within each pot give [nested measurements](nested-measurements.md); repeatedly reading one [leaf](leaf.md) gives another level of repetition. Either can yield [clustered data](clustered-data.md). A common [random effect](random-effect.md) can describe the shared influence of the containing [experimental unit](experimental-unit.md).

For the constructed pot example, label [treatments](treatment.md) by $g\in\{A,B\}$, pots within each group by $i=1,\ldots,n$, and [leaves](leaf.md) within each pot by $j=1,\ldots,m$. Consider the [statistical model](statistical-model-split.md)

$$
Y_{gij}=\mu+\alpha_g+U_{gi}+\varepsilon_{gij},
\qquad
\mathbb E[U_{gi}]=\mathbb E[\varepsilon_{gij}]=0,
\qquad
\operatorname{Var}(U_{gi})=\tau^2,
\quad
\operatorname{Var}(\varepsilon_{gij})=\sigma^2.
$$

Here $Y_{gij}$ is a [leaf](leaf.md) [length](length.md), $\mu+\alpha_g$ is its group [expected value](expected-value-split.md), $U_{gi}$ is a pot [random effect](random-effect.md), and $\varepsilon_{gij}$ describes remaining variation among [leaves](leaf.md) and [measurement error](measurement-error.md). Assume that all pot [random effects](random-effect.md) are mutually [independent](independent-random-variables.md), all remaining errors are mutually [independent](independent-random-variables.md), and the two collections are [independent](independent-random-variables.md) of one another and of the [randomization](randomization.md). These are explicit modelling assumptions, conditional on the assigned [treatments](treatment.md); no [normal distribution](normal-distribution.md) assumption is needed for the following [variance](variance-split.md) calculation.

Two distinct [leaf](leaf.md) measurements in one pot share $U_{gi}$. Their [covariance](covariance.md) is $\tau^2$, their individual [variance](variance-split.md) is $\tau^2+\sigma^2$, and their [intraclass correlation coefficient](intraclass-correlation-coefficient.md) is

$$
\rho=\frac{\tau^2}{\tau^2+\sigma^2}
\qquad (\tau^2+\sigma^2>0).
$$

Measurements from different pots have zero [covariance](covariance.md) and are [independent](independent-random-variables.md) under the stated [statistical model](statistical-model-split.md). Statistical [independence](independent-random-variables.md) therefore concerns the whole response structure, not just the fact that the measured [leaves](leaf.md) are different objects.

**Table of contents**

- [Variance of nested measurements](variance-of-nested-measurements.md)

## ↑ Ancestors (8)

1. [Replication in experimental design](replication-in-experimental-design.md)
2. [Design of experiments](design-of-experiments-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Biological replicate](biological-replicate.md)
- [Nested measurements](nested-measurements.md)
- [Pseudoreplication](pseudoreplication.md)
- [Replication in experimental design](replication-in-experimental-design.md)
- [Variance of nested measurements](variance-of-nested-measurements.md)
