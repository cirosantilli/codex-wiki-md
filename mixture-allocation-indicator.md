# Mixture allocation indicator

↑ **Parent:** [Finite mixture model](finite-mixture-model.md)

Generate a [finite mixture model](finite-mixture-model.md) by drawing a [categorical variable](categorical-variable.md) $Z$ with $\mathbb P(Z=j)=\pi_j$, then drawing $X$ from the [mixture component](mixture-component.md) $P_j$. The [indicator random variables](indicator-random-variable.md) $I_j=\mathbf1_{\{Z=j\}}$ satisfy $\sum_jI_j=1$: exactly one [mixture component](mixture-component.md) generates each draw. The [joint probability distribution](joint-probability-distribution.md) obeys $\mathbb P(Z=j,X\in A)=\pi_jP_j(A)$, and the [law of total probability](law-of-total-probability.md) gives the [mixture distribution](mixture-distribution.md) after summing out $Z$.[§21.1.3, printed p. 443, equations (21.2)-(21.3), and §21.1.7, p. 446: choose a label, then sample its component](advanced-data-analysis-from-an-elementary-point-of-view-2015-draft-by-cosma-rohilla-shalizi/mixture-models.md)

For independent draws from this [statistical model](statistical-model-split.md), draw a fresh $Z_i$ for each $X_i$. Drawing one shared [latent variable](latent-variable-split.md) $Z$ for an entire collection is a different [joint probability distribution](joint-probability-distribution.md): its individual [marginal distributions](marginal-distribution.md) can match the same [mixture distribution](mixture-distribution.md) while its observations are dependent.

## ↑ Ancestors (8)

1. [Finite mixture model](finite-mixture-model.md)
2. [Mixture model](mixture-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [EM expectation step](em-expectation-step.md)
- [Responsibility curve for a two-Gaussian mixture](responsibility-curve-for-a-two-gaussian-mixture.md)
- [Two-Gaussian mixture example](two-gaussian-mixture-example.md)
