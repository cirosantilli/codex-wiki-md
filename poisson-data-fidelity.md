# Poisson data fidelity

↑ **Parent:** [Variational regularization](variational-regularization.md)

For positive observations $y$ and positive predicted intensities $s$, this is the [generalized Kullback–Leibler divergence](generalized-kullback-leibler-divergence.md) with observation in the first argument. Its scalar derivative in $s$ is $1-y/s$ and its second derivative is $y/s^2>0$. It differs from the divergence of a reconstructed density from a reference density by which argument is varied. A linear prediction $s=Kx$ gives derivative $K^*(1-y/(Kx))$ through the [adjoint operator](adjoint-operator.md), on suitable admissible function spaces. This fidelity arises from the negative log likelihood of a [Poisson observation model](poisson-observation-model.md), after removal of terms depending only on observations.

**Table of contents**

- [Shifted Poisson data fidelity](shifted-poisson-data-fidelity.md)
  - [Existence for nonnegative shifted Poisson regularization](existence-for-nonnegative-shifted-poisson-regularization.md)
  - [Nonattainment under strict positivity for shifted Poisson fidelity](nonattainment-under-strict-positivity-for-shifted-poisson-fidelity.md)
- [Proximal operator of Poisson data fidelity](proximal-operator-of-poisson-data-fidelity.md)

## ↑ Ancestors (7)

1. [Variational regularization](variational-regularization.md)
2. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
3. [Inverse problem](inverse-problem-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326/3/ii/solution.md)
- [Poisson observation](poisson-observation.md)
- [Proximal operator of Poisson data fidelity](proximal-operator-of-poisson-data-fidelity.md)
