# Semidefinite relaxation of slab-constrained quadratic maximization

↑ **Parent:** [Semidefinite programming](semidefinite-programming.md)

Replacing $xx^T$ by a general [positive semidefinite matrix](positive-semidefinite-matrix.md) relaxes maximization of $\|x\|_2^2$ subject to $|a_i^Tx|\le1$. The relaxed value is an upper bound because $xx^T$ has trace $\|x\|_2^2$ and satisfies the same quadratic constraints. Both problems are unbounded if the $a_i$ fail to span the ambient space. If they span it, $H=\sum_i a_ia_i^T$ is positive definite and $\lambda_{\min}(H)\operatorname{tr}X\le\operatorname{tr}(HX)\le m$, proving boundedness and attainment of the relaxation.

**Table of contents**

- [Rademacher rounding for a semidefinite relaxation](rademacher-rounding-for-a-semidefinite-relaxation.md)
  - [Logarithmic approximation bound for slab-constrained quadratic maximization](logarithmic-approximation-bound-for-slab-constrained-quadratic-maximization.md)

## ↑ Ancestors (6)

1. [Semidefinite programming](semidefinite-programming.md)
2. [Convex optimization](convex-optimization-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-339/2/a/solution.md)
