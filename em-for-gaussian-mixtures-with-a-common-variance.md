# EM for Gaussian mixtures with a common variance

↑ **Parent:** [Finite Gaussian mixture with a common variance](finite-gaussian-mixture-with-a-common-variance.md)

The E-step computes [mixture responsibilities](mixture-responsibility.md) $\tau_{ij}$ from the old parameters. Put $N_j=\sum_i\tau_{ij}$. The M-step updates $\pi_j=N_j/n$, $\mu_j=\sum_i\tau_{ij}y_i/N_j$ and $\sigma^2=\sum_{i,j}\tau_{ij}(y_i-\mu_j^{\mathrm{new}})^2/n$. The variance uses new means and old responsibilities. [EM likelihood monotonicity](em-likelihood-monotonicity.md) guarantees nondecrease of the observed likelihood, not a global optimum.

## ↑ Ancestors (9)

1. [Finite Gaussian mixture with a common variance](finite-gaussian-mixture-with-a-common-variance.md)
2. [Finite mixture model](finite-mixture-model.md)
3. [Mixture model](mixture-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Finite Gaussian mixture with a common variance](finite-gaussian-mixture-with-a-common-variance.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/4/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/6/b/i/solution.md)
