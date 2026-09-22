# Moment aliasing in a shared zero-inflated count model

↑ **Parent:** [Identifiability](identifiability.md)

In a [shared zero-inflated Gamma-Poisson count model](shared-zero-inflated-gamma-poisson-count-model.md), write $m_j=(1-\pi)\mu_j$ and $\kappa=(\tau+\pi)/(1-\pi)$. Its first two moments are $\operatorname{Var}(Y_j)=m_j+\kappa m_j^2$ and $\operatorname{Cov}(Y_j,Y_k)=\kappa m_jm_k$. These moments do not separately identify $\pi$, $\tau$, and the component-mean intercept: taking $\pi'=0$, $\tau'=\kappa$ and $\mu'_j=m_j$ gives the same first two moments. The full count distribution can carry information absent from the moments. A [consistent estimator](consistency-statistics.md) of a marginal mean ratio therefore need not consistently estimate a structural-zero fraction from a misspecified moment parameterization.

## ↑ Ancestors (6)

1. [Identifiability](identifiability.md)
2. [Statistical model](statistical-model-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37/6/d/solution.md)
