# Tridiagonal matrix algorithm

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tridiagonal_matrix_algorithm)

The [Thomas algorithm](tridiagonal-matrix-algorithm.md) is [Gaussian elimination](gaussian-elimination.md) specialized to a [tridiagonal matrix](tridiagonal-matrix.md): each row couples an unknown only to its immediate neighbours. Eliminating one unknown changes just the next diagonal entry and right-hand side. Provided all [pivot elements](pivot-element.md) are nonzero, a forward sweep followed by [back substitution](back-substitution.md) solves an $n$-unknown [linear system](system-of-linear-equations.md) in $O(n)$ time and storage, using [Big O notation](big-o-notation.md). Treating the same entries as a full [matrix](matrix.md) wastes the zeros: classical dense [LU factorization and solve costs](lu-factorization-and-solve-costs.md) grow cubically for factorization and quadratically for storage.

A concrete reason to care is the [Dirichlet Poisson solution by tridiagonal elimination](dirichlet-poisson-solution-by-tridiagonal-elimination.md): a three-point [finite difference](finite-difference-split.md) for the [second derivative](second-derivative.md) couples adjacent points on a [mesh](finite-element-mesh.md), producing precisely this [tridiagonal matrix](tridiagonal-matrix.md). The same structure occurs in one-dimensional [Crank-Nicolson method](crank-nicolson-method.md) calculations. NPTEL's archived Lecture 13 introduces the [Thomas algorithm](tridiagonal-matrix-algorithm.md) from that time-stepping problem and labels the procedure “Thomas algorithm (1949)”.[Lecture 13, Thomas algorithm: opening historical attribution and Crank Nicolson motivation](thomas-algorithm-nptel-lecture-13.md)

**Table of contents**

- [Tridiagonal elimination recurrences](tridiagonal-elimination-recurrences.md)
- [Dirichlet Poisson solution by tridiagonal elimination](dirichlet-poisson-solution-by-tridiagonal-elimination.md)
- [Safe pivots for tridiagonal elimination](safe-pivots-for-tridiagonal-elimination.md)
- [Zero-pivot failure of tridiagonal elimination](zero-pivot-failure-of-tridiagonal-elimination.md)
- [Tridiagonal solve costs](tridiagonal-solve-costs.md)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
