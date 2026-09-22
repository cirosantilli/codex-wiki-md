# Irreversible three-state disease model

↑ **Parent:** [Continuous-time multi-state model](continuous-time-multi-state-model.md)

An irreversible three-state [continuous-time multi-state model](continuous-time-multi-state-model.md) permits only $1\to2\to3$, with state 3 absorbing. For constant rates $\lambda=q_{12}$ and $\mu=q_{23}$,

$$
p_{11}(t)=e^{-\lambda t},\qquad
p_{12}(t)=\frac{\lambda(e^{-\lambda t}-e^{-\mu t})}{\mu-\lambda},\qquad
p_{13}(t)=1-p_{11}(t)-p_{12}(t).
$$

At equal rates use $p_{12}(t)=\lambda t e^{-\lambda t}$. A [panel-observed multi-state likelihood](panel-observed-multi-state-likelihood.md) uses these [transition probabilities](transition-probability.md), allowing unobserved intermediate visits between examinations.

**Table of contents**

- [Frozen-age approximation in a multi-state model](frozen-age-approximation-in-a-multi-state-model.md)

## ↑ Ancestors (6)

1. [Continuous-time multi-state model](continuous-time-multi-state-model.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Progressive illness-death model](progressive-illness-death-model.md)
