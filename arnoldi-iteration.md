# Arnoldi iteration

↑ **Parent:** [Krylov subspace](krylov-subspace.md)

Starting with $q_1=b/\|b\|_2$, the Arnoldi iteration constructs an [orthonormal basis](orthonormal-basis.md) of successive [Krylov subspaces](krylov-subspace.md). At step $j$, orthogonalize $Aq_j$ against $q_1,\ldots,q_j$, and normalize the remainder as $q_{j+1}$ if it is nonzero. The coefficients form an [upper Hessenberg matrix](upper-hessenberg-matrix.md) $\widetilde H_k$ and satisfy $AQ_k=Q_{k+1}\widetilde H_k$. A zero remainder means the current [Krylov subspace](krylov-subspace.md) is invariant under $A$.

**Table of contents**

- [Lanczos algorithm](lanczos-algorithm.md)
- [Arnoldi decomposition](arnoldi-decomposition.md)

## ↑ Ancestors (8)

1. [Krylov subspace](krylov-subspace.md)
2. [Conjugate gradient method](conjugate-gradient-method.md)
3. [Gradient descent](gradient-descent-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Arnoldi decomposition](arnoldi-decomposition.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/a/4/b/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2025/3/b/i/solution.md)
