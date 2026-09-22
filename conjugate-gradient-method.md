# Conjugate gradient method

↑ **Parent:** [Gradient descent](gradient-descent-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conjugate_gradient_method)

For a [positive-definite matrix](positive-definite-matrix.md) $A$, the conjugate gradient method chooses mutually $A$-conjugate search directions. Starting with $r_0=b-Ax_0$ and $p_0=r_0$, it uses

$$
\alpha_k=\frac{r_k^Tr_k}{p_k^TAp_k},\quad
x_{k+1}=x_k+\alpha_kp_k,\quad
r_{k+1}=r_k-\alpha_kAp_k,
$$

and $p_{k+1}=r_{k+1}+\beta_kp_k$ with  
$\beta_k=r_{k+1}^Tr_{k+1}/(r_k^Tr_k)$.

**Table of contents**

- [Spectral weighting of conjugate gradient error](spectral-weighting-of-conjugate-gradient-error.md)
- [Conjugate direction](conjugate-direction.md)
  - [Finite termination of conjugate directions](finite-termination-of-conjugate-directions.md)
- [Conjugate gradient convergence bound](conjugate-gradient-convergence-bound.md)
- [Linear-system residual](linear-system-residual.md)
  - [Linear-system residual norm](linear-system-residual-norm.md)
- [Conjugate-gradient residual orthogonality](conjugate-gradient-residual-orthogonality.md)
- [Preconditioned conjugate gradient method](preconditioned-conjugate-gradient-method.md)
  - [Exact inverse-square-root preconditioner](exact-inverse-square-root-preconditioner.md)
- [Krylov subspace](krylov-subspace.md)
  - [Generalized minimal residual method](generalized-minimal-residual-method.md)
    - [One-step restarted GMRES stagnation example](one-step-restarted-gmres-stagnation-example.md)
  - [Arnoldi iteration](arnoldi-iteration.md)
    - [Lanczos algorithm](lanczos-algorithm.md)
    - [Arnoldi decomposition](arnoldi-decomposition.md)
  - [Krylov dimension from spectral components](krylov-dimension-from-spectral-components.md)
- [Finite termination of the conjugate gradient method](finite-termination-of-the-conjugate-gradient-method.md)

## ↑ Ancestors (6)

1. [Gradient descent](gradient-descent-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (20)

- [Bounded two-dimensional capacitor field model](bounded-two-dimensional-capacitor-field-model.md)
- [Conjugate gradient convergence bound](conjugate-gradient-convergence-bound.md)
- [Finite termination of conjugate directions](finite-termination-of-conjugate-directions.md)
- [Krylov subspace method](krylov-subspace-method.md)
- [Left preconditioning](left-preconditioning.md)
- [Linear-system residual](linear-system-residual.md)
- [Matrix preconditioning](matrix-preconditioning.md)
- [Optimal fixed step for quadratic gradient descent](optimal-fixed-step-for-quadratic-gradient-descent.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/37e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/40e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/40c/a/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford/2008/4/b/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2010/a/3/e/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2025/3/b/iii/solution.md)
- [Preconditioned steepest descent](preconditioned-steepest-descent.md)
- [Spectral weighting of conjugate gradient error](spectral-weighting-of-conjugate-gradient-error.md)
- [Strict feasibility for conic duality](strict-feasibility-for-conic-duality.md)
- [Symmetric positive-definite preconditioning](symmetric-positive-definite-preconditioning.md)
