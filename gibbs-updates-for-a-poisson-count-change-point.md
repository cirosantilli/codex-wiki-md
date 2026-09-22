# Gibbs updates for a Poisson count change point

↑ **Parent:** [Poisson count change-point model with gamma priors](poisson-count-change-point-model-with-gamma-priors.md)

The [full conditional distributions](full-conditional-distribution.md) are $\lambda\mid m,x\sim\operatorname{Gamma}(\alpha+S_m,\beta+m)$ and $\phi\mid m,x\sim\operatorname{Gamma}(\gamma+S_N-S_m,\delta+N-m)$, in shape-rate notation. Conditional on the two rates, $m$ has weights $w_j=\exp[j(\phi-\lambda)+S_j\log(\lambda/\phi)]$. A [Gibbs sampler](gibbs-sampler.md) cycles through these three draws. Each update preserves the joint [posterior distribution](bayesian-posterior.md); subtracting the largest log weight before exponentiation stabilizes the categorical draw. Averages of $\mathbf1_{\{m=N\}}$ estimate the posterior probability of no observed change.

## ↑ Ancestors (6)

1. [Poisson count change-point model with gamma priors](poisson-count-change-point-model-with-gamma-priors.md)
2. [Change-point detection](change-point-detection.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/5/b/ii/solution.md)
