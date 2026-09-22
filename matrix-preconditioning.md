# Matrix preconditioning

↑ **Parent:** [Numerical linear algebra](numerical-linear-algebra-split.md)

[Matrix preconditioning](matrix-preconditioning.md) transforms a [linear system](system-of-linear-equations.md) using an inexpensive auxiliary solve to improve its [eigenvalues](eigenvalue.md). For [symmetric positive-definite matrices](symmetric-positive-definite-matrix.md), a [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) $M$ produces $M^{-1/2}AM^{-1/2}$, preserving the symmetric structure needed by the [Conjugate gradient method](conjugate-gradient-method.md).

A useful [matrix preconditioner](matrix-preconditioner.md) combines a cheap solve with favorable transformed [eigenvalues](eigenvalue.md); neither property alone is enough.[Math 221, Matrix Computations, Fall 2023; Notes for Ma221 Lecture 15, Dec 1, 2023; PDF p. 1, opening transformation, goals (1) and (2), and example (1)](math-221-matrix-computations-fall-2023/notes-for-ma221-lecture-15-dec-1-2023.md)

The aim is to make each correction more effective without making it expensive. The example under [diagonal scaling for a two-dimensional linear system](diagonal-scaling-for-a-two-dimensional-linear-system.md) turns thin [ellipses](ellipse.md) into nearly circular ones and makes [preconditioned steepest descent](preconditioned-steepest-descent.md) effective.

**Table of contents**

- [Matrix preconditioner](matrix-preconditioner.md)
  - [Jacobi preconditioner](jacobi-preconditioner.md)
- [Left preconditioning](left-preconditioning.md)
- [Right preconditioning](right-preconditioning.md)
- [Symmetric positive-definite preconditioning](symmetric-positive-definite-preconditioning.md)
  - [Symmetric preconditioning as energy geometry](symmetric-preconditioning-as-energy-geometry.md)
- [Diagonal scaling for a two-dimensional linear system](diagonal-scaling-for-a-two-dimensional-linear-system.md)
- [Preconditioned steepest descent](preconditioned-steepest-descent.md)
  - [Condition-number bound for preconditioned steepest descent](condition-number-bound-for-preconditioned-steepest-descent.md)

## ↑ Ancestors (6)

1. [Numerical linear algebra](numerical-linear-algebra-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Matrix preconditioning](matrix-preconditioning.md)
- [Matrix splitting](matrix-splitting.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/37e/b/solution.md)
- [Preconditioned steepest descent](preconditioned-steepest-descent.md)
