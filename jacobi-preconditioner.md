# Jacobi preconditioner

↑ **Parent:** [Matrix preconditioner](matrix-preconditioner.md)

The [Jacobi preconditioner](jacobi-preconditioner.md) keeps only the diagonal entries of the [matrix](matrix.md) $A$. For a [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md), these entries are positive, so its auxiliary solve is $z_i=r_i/a_{ii}$. It rescales coordinates with very different diagonal sizes, but cannot remove arbitrary off-diagonal coupling.[Math 221, Matrix Computations, Fall 2023; Notes for Ma221 Lecture 15, Dec 1, 2023; PDF p. 1, example (1), diagonal or Jacobi preconditioning](math-221-matrix-computations-fall-2023/notes-for-ma221-lecture-15-dec-1-2023.md)

This shares a [diagonal matrix](diagonal-matrix.md) with the [Jacobi method](jacobi-method.md), but the roles differ. The [Jacobi method](jacobi-method.md) specifies a whole [stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md); a [Jacobi preconditioner](jacobi-preconditioner.md) supplies an auxiliary solve to another [iterative method](iterative-method.md), including the [Preconditioned conjugate gradient method](preconditioned-conjugate-gradient-method.md).

## ↑ Ancestors (8)

1. [Matrix preconditioner](matrix-preconditioner.md)
2. [Matrix preconditioning](matrix-preconditioning.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Diagonal scaling for a two-dimensional linear system](diagonal-scaling-for-a-two-dimensional-linear-system.md)
- [Jacobi preconditioner](jacobi-preconditioner.md)
- [Preconditioned steepest descent](preconditioned-steepest-descent.md)
