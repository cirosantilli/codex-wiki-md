# Likelihood-power annealing

↑ **Parent:** [Simulated annealing](simulated-annealing.md)

To maximize a [log-likelihood](log-likelihood.md), use energy $-\ell$ and [Boltzmann distribution](boltzmann-distribution.md) proportional to $e^{\ell/T}=L^{1/T}$ at temperature $T>0$. Reversing this sign favors [likelihood](likelihood-function.md) minima and can make the [probability density function](probability-density-function.md) nonnormalizable. For Poisson observations with total $s$ and sample size $m$, with respect to $d\lambda$ the normalized [probability density function](probability-density-function.md) is

$$
\lambda\sim\operatorname{Gamma}(s/T+1,m/T).
$$

Its [mean](expected-value.md) is $(s+T)/m$ and [variance](variance-split.md) $(sT+T^2)/m^2$, so it concentrates at the [maximum-likelihood estimate](maximum-likelihood-estimator.md) $s/m$ as $T\downarrow0$. Cooling of equilibrium laws and convergence of a particular changing-temperature chain are different statements; the latter requires mixing or a direct chain argument.

**Table of contents**

- [Binomial likelihood-power annealing](binomial-likelihood-power-annealing.md)
- [Gaussian likelihood Gibbs annealing](gaussian-likelihood-gibbs-annealing.md)

## ↑ Ancestors (6)

1. [Simulated annealing](simulated-annealing.md)
2. [Heuristic optimization](heuristic-optimization.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/4/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/6/solution.md)
