# Elimination multiplier

↑ **Parent:** [Gaussian elimination](gaussian-elimination.md)

For $i>k$, an [elimination multiplier](elimination-multiplier.md) is the [scalar](scalar.md) $l_{ik}=a_{ik}^{(k-1)}/a_{kk}^{(k-1)}$ used in the [elementary row operation](elementary-row-operation.md) $R_i\leftarrow R_i-l_{ik}R_k$. This creates a zero below the [pivot element](pivot-element.md). The remaining entries change by $a_{ij}\leftarrow a_{ij}-l_{ik}a_{kj}$ for $j>k$. Storing these [elimination multipliers](elimination-multiplier.md) gives the subdiagonal entries of $L$ in [LU decomposition](lu-decomposition.md); later row interchanges must also reorder the already stored coefficients.

## ↑ Ancestors (7)

1. [Gaussian elimination](gaussian-elimination.md)
2. [Numerical linear algebra](numerical-linear-algebra.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Computed three-by-three LU decomposition](computed-three-by-three-lu-decomposition.md)
- [Elimination multiplier](elimination-multiplier.md)
- [LU decomposition](lu-decomposition.md)
- [LU factorization and solve costs](lu-factorization-and-solve-costs.md)
- [Pivot element](pivot-element.md)
- [Pivoted LU decomposition](pivoted-lu-decomposition.md)
- [Tridiagonal elimination recurrences](tridiagonal-elimination-recurrences.md)
