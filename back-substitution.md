# Back substitution

↑ **Parent:** [Triangular matrix](triangular-matrix.md)

An upper [triangular matrix](triangular-matrix.md) system with nonzero diagonal is solved from the last row upward. Once $x_{i+1},\ldots,x_n$ are known, use $x_i=(b_i-\sum_{j>i}a_{ij}x_j)/a_{ii}$. The nonzero diagonal guarantees a unique solution; this is the final solve after a [QR factorization](qr-decomposition.md).

## ↑ Ancestors (6)

1. [Triangular matrix](triangular-matrix.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (25)

- [Block elimination](block-elimination.md)
- [Block matrix inverse](block-matrix-inverse.md)
- [Dirichlet Poisson solution by tridiagonal elimination](dirichlet-poisson-solution-by-tridiagonal-elimination.md)
- [Forward substitution](forward-substitution.md)
- [Gaussian elimination](gaussian-elimination.md)
- [Gaussian elimination with a row swap](gaussian-elimination-with-a-row-swap.md)
- [Householder reduction of an overdetermined consistent system](householder-reduction-of-an-overdetermined-consistent-system.md)
- [LU decomposition](lu-decomposition.md)
- [LU factorization and solve costs](lu-factorization-and-solve-costs.md)
- [Matrix decomposition](matrix-decomposition.md)
- [Matrix preconditioner](matrix-preconditioner.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1/18c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/11/a/i/solution.md)
- [Pivoted LU decomposition](pivoted-lu-decomposition.md)
- [QR decomposition](qr-decomposition.md)
- [QR decomposition by Givens rotations](qr-decomposition-by-givens-rotations.md)
- [Reusing LU factors for multiple right-hand sides](reusing-lu-factors-for-multiple-right-hand-sides.md)
- [Row echelon form](row-echelon-form.md)
- [Sparse Gaussian elimination](sparse-gaussian-elimination.md)
- [Tiny-pivot roundoff in Gaussian elimination](tiny-pivot-roundoff-in-gaussian-elimination.md)
- [Triangular solves for LU decomposition](triangular-solves-for-lu-decomposition.md)
- [Tridiagonal elimination recurrences](tridiagonal-elimination-recurrences.md)
- [Tridiagonal matrix algorithm](tridiagonal-matrix-algorithm.md)
- [Tridiagonal solve costs](tridiagonal-solve-costs.md)
- [Zero-pivot failure of tridiagonal elimination](zero-pivot-failure-of-tridiagonal-elimination.md)
