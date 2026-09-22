# Generalized minimal residual method

↑ **Parent:** [Krylov subspace](krylov-subspace.md)

With zero initial guess, the generalized minimal residual method minimizes the [Euclidean norm](euclidean-norm.md) of the [linear-system residual](linear-system-residual.md) over each [Krylov subspace](krylov-subspace.md). The [Arnoldi decomposition](arnoldi-decomposition.md) reduces this to $\min_y\|\widetilde H_ky-\|b\|_2e_1\|_2$, followed by $x_k=Q_ky$. [Givens rotations](givens-rotation.md) solve the small problem in $O(k^2)$ operations once the decomposition is available. For an [invertible matrix](invertible-matrix.md) $A$, the same iterate minimizes the error in the [weighted norm](weighted-norm.md) induced by $A^TA$, because $\|Ax-b\|_2=\|x-x_*\|_{A^TA}$.

**Table of contents**

- [One-step restarted GMRES stagnation example](one-step-restarted-gmres-stagnation-example.md)

## ↑ Ancestors (8)

1. [Krylov subspace](krylov-subspace.md)
2. [Conjugate gradient method](conjugate-gradient-method.md)
3. [Gradient descent](gradient-descent-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2025/3/a/i/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2025/3/a/iii/solution.md)
