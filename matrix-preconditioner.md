# Matrix preconditioner

↑ **Parent:** [Matrix preconditioning](matrix-preconditioning.md)

A [matrix preconditioner](matrix-preconditioner.md) is an auxiliary [invertible matrix](invertible-matrix.md) whose [matrix inverse](matrix-inverse-split.md) is cheap to apply and whose use improves the [eigenvalues](eigenvalue.md) of a [linear system](system-of-linear-equations.md). In [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) problems, a [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) $M$ preserves that structure under the symmetric transformation $M^{-1/2}AM^{-1/2}$.

Applying $M^{-1}$ means solving $Mz=r$ for a supplied [vector](vector.md) $r$. This notation does not require forming a general [matrix inverse](matrix-inverse-split.md). A [diagonal matrix](diagonal-matrix.md) gives componentwise divisions; a factored [matrix](matrix.md) gives auxiliary solves such as [forward substitution](forward-substitution.md) and [back substitution](back-substitution.md).[Math 221, Matrix Computations, Fall 2009; Basic iterative methods, web lines 297–308, recurrence (\*) and cheap auxiliary-solve requirement](math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009.md)

Choosing $M=I$ makes the solve trivial but changes nothing; choosing $M=A$ gives the exact correction but asks us to solve the original [linear system](system-of-linear-equations.md).[Math 221, Matrix Computations, Fall 2023; Notes for Ma221 Lecture 15, Dec 1, 2023; PDF p. 1, contrasting M = I and M = A; p. 2, example (3), two triangular solves](math-221-matrix-computations-fall-2023/notes-for-ma221-lecture-15-dec-1-2023.md)

**Table of contents**

- [Jacobi preconditioner](jacobi-preconditioner.md)

## ↑ Ancestors (7)

1. [Matrix preconditioning](matrix-preconditioning.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Matrix preconditioner](matrix-preconditioner.md)
- [Matrix preconditioning](matrix-preconditioning.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/37e/b/solution.md)
