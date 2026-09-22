# Forward substitution

↑ **Parent:** [Triangular solves for LU decomposition](triangular-solves-for-lu-decomposition.md)

[Forward substitution](forward-substitution.md) solves a [linear system](system-of-linear-equations.md) $Ly=c$ with a [lower triangular matrix](lower-triangular-matrix.md) $L$ and nonzero diagonal, from the first row downward:

$$
y_i=\frac{c_i-\sum_{j=1}^{i-1}l_{ij}y_j}{l_{ii}},\qquad i=1,\ldots,n.
$$

The first [sum](sum.md) is empty, so $y_1=c_1/l_{11}$. Each subsequent row uses only components already found. For a [unit triangular matrix](unit-triangular-matrix.md) $L$, omit the division because $l_{ii}=1$. The complementary procedure, [back substitution](back-substitution.md), solves an [upper triangular matrix](upper-triangular-matrix.md) system from the last row upward.[§2.3.2, equations (2.3.7)–(2.3.9), and §2.3.3, Algorithms 2.3.1–2.3.2: forward and backward substitution](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others.md)

## ↑ Ancestors (8)

1. [Triangular solves for LU decomposition](triangular-solves-for-lu-decomposition.md)
2. [LU decomposition](lu-decomposition.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Cholesky decomposition](cholesky-decomposition.md)
- [Forward substitution](forward-substitution.md)
- [Gauss-Seidel method](gauss-seidel-method.md)
- [LU decomposition](lu-decomposition.md)
- [LU factorization and solve costs](lu-factorization-and-solve-costs.md)
- [Matrix decomposition](matrix-decomposition.md)
- [Matrix preconditioner](matrix-preconditioner.md)
- [Matrix splitting](matrix-splitting.md)
- [Reusing LU factors for multiple right-hand sides](reusing-lu-factors-for-multiple-right-hand-sides.md)
- [Sparse Gaussian elimination](sparse-gaussian-elimination.md)
- [Triangular solve](triangular-solve.md)
- [Triangular solves for LU decomposition](triangular-solves-for-lu-decomposition.md)
- [Tridiagonal elimination recurrences](tridiagonal-elimination-recurrences.md)
- [Tridiagonal solve costs](tridiagonal-solve-costs.md)
- [Unit triangular matrix](unit-triangular-matrix.md)
