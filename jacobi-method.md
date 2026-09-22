# Jacobi method

↑ **Parent:** [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobi_method)

Writing $A=D+L+U$, where $D$ is diagonal and $L,U$ are strictly triangular, the Jacobi iteration is

$$
x^{(k+1)}=D^{-1}\left(b-(L+U)x^{(k)}\right).
$$

The [Jacobi method](jacobi-method.md) solves a [linear system](system-of-linear-equations.md) by updating every coordinate from the same old [vector](vector.md). It requires every diagonal entry $a_{ii}$ to be nonzero. Isolating coordinate $i$ in row $i$ gives the simultaneous rule

$$
x_i^{(k+1)}=\frac{b_i-\sum_{j\ne i}a_{ij}x_j^{(k)}}{a_{ii}},\qquad B=-D^{-1}(L+U)=I-D^{-1}A.
$$

Here $B$ is the [iteration matrix](iteration-matrix.md). A sweep computes a complete new [vector](vector.md) before replacing the old one, so its coordinate updates can run independently.[Math 221, Matrix Computations, Fall 2009; Jacobi: component loop and splitting immediately before Gauss-Seidel](math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009.md)

For a [sparse matrix](sparse-matrix.md), a sweep needs work proportional to the stored nonzero entries, while [Gaussian elimination](gaussian-elimination.md) may create [fill-in](fill-in.md). The [Jacobi method](jacobi-method.md) is therefore a simple starting point for large [linear systems](system-of-linear-equations.md), and the [weighted Jacobi method](weighted-jacobi-method.md) supplies a useful building block of a [multigrid method](multigrid-method-split.md). Its beauty is that a local row correction becomes a global [eigenvalue](eigenvalue.md) question: the [convergence criterion for a stationary iteration](convergence-criterion-for-a-stationary-iteration.md) is exactly $\rho(B)<1$.

**Table of contents**

- [Jacobi iteration for a three-variable tridiagonal system](jacobi-iteration-for-a-three-variable-tridiagonal-system.md)
  - [Error modes of a three-variable Jacobi iteration](error-modes-of-a-three-variable-jacobi-iteration.md)
- [Jacobi convergence from strict diagonal dominance](jacobi-convergence-from-strict-diagonal-dominance.md)
- [Skew-tridiagonal Jacobi and Gauss-Seidel iterations](skew-tridiagonal-jacobi-and-gauss-seidel-iterations.md)
- [Weighted Jacobi method](weighted-jacobi-method.md)
  - [Weighted Jacobi eigenvalues for a square Dirichlet grid](weighted-jacobi-eigenvalues-for-a-square-dirichlet-grid.md)
  - [Weighted Jacobi method for the one-dimensional Poisson equation](weighted-jacobi-method-for-the-one-dimensional-poisson-equation.md)
    - [High-frequency smoothing factor of weighted Jacobi](high-frequency-smoothing-factor-of-weighted-jacobi.md)
      - [Exact finite-grid high-frequency Jacobi smoothing optimum](exact-finite-grid-high-frequency-jacobi-smoothing-optimum.md)
- [Jacobi convergence for a three-by-three equicorrelation matrix](jacobi-convergence-for-a-three-by-three-equicorrelation-matrix.md)
- [Jacobi convergence for a symmetric positive-definite tridiagonal matrix](jacobi-convergence-for-a-symmetric-positive-definite-tridiagonal-matrix.md)

## ↑ Ancestors (7)

1. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (29)

- [Error modes of a three-variable Jacobi iteration](error-modes-of-a-three-variable-jacobi-iteration.md)
- [Exact error contraction of a two-variable Gauss-Seidel iteration](exact-error-contraction-of-a-two-variable-gauss-seidel-iteration.md)
- [Gauss-Seidel iteration for a two-variable positive-definite system](gauss-seidel-iteration-for-a-two-variable-positive-definite-system.md)
- [Gauss-Seidel method](gauss-seidel-method.md)
- [Jacobi convergence for a three-by-three equicorrelation matrix](jacobi-convergence-for-a-three-by-three-equicorrelation-matrix.md)
- [Jacobi convergence for the nine-point Dirichlet stencil](jacobi-convergence-for-the-nine-point-dirichlet-stencil.md)
- [Jacobi convergence from strict diagonal dominance](jacobi-convergence-from-strict-diagonal-dominance.md)
- [Jacobi iteration for a three-variable tridiagonal system](jacobi-iteration-for-a-three-variable-tridiagonal-system.md)
- [Jacobi method](jacobi-method.md)
- [Jacobi preconditioner](jacobi-preconditioner.md)
- [Matrix splitting](matrix-splitting.md)
- [Multigrid method](multigrid-method-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/16b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-3/19f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/38c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-1/6c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/39b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1/39a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/40a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/37e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/40c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3/40a/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4/40d/b/solution.md)
- [Positive definiteness of the grounded nine-point Poisson stencil](positive-definiteness-of-the-grounded-nine-point-poisson-stencil.md)
- [Semiconvergence of cyclic Poisson iterations](semiconvergence-of-cyclic-poisson-iterations.md)
- [Skew-tridiagonal Jacobi and Gauss-Seidel iterations](skew-tridiagonal-jacobi-and-gauss-seidel-iterations.md)
- [Weighted Jacobi method](weighted-jacobi-method.md)
