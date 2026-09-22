# LU decomposition

↑ **Parent:** [Numerical linear algebra](numerical-linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/LU_decomposition)

An [LU decomposition](lu-decomposition.md) writes a [square matrix](square-matrix.md) as $A=LU$, with $L$ a [lower triangular matrix](lower-triangular-matrix.md) and $U$ an [upper triangular matrix](upper-triangular-matrix.md). We use a [unit triangular matrix](unit-triangular-matrix.md) $L$, meaning $l_{ii}=1$. The factors record [Gaussian elimination](gaussian-elimination.md): $U$ contains the reduced equations, while $L$ stores the [elimination multipliers](elimination-multiplier.md) needed to reconstruct the original equations. This makes [Reusing LU factors for multiple right-hand sides](reusing-lu-factors-for-multiple-right-hand-sides.md) inexpensive.[§2.4.3, Definition 2.4.2 and equation (2.4.7): unit lower triangular L and upper triangular U](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others.md)

For an [invertible matrix](invertible-matrix.md), unpivoted [LU decomposition](lu-decomposition.md) requires nonzero [pivot elements](pivot-element.md) at every elimination step; invertibility alone does not guarantee this. In general use [Pivoted LU decomposition](pivoted-lu-decomposition.md), with the explicit convention $PA=LU$ and a [permutation matrix](permutation-matrix.md) $P$. Once the factors exist, solving a [linear system](system-of-linear-equations.md) $Ax=b$ needs [forward substitution](forward-substitution.md) followed by [back substitution](back-substitution.md), rather than forming a [matrix inverse](matrix-inverse.md).

**Table of contents**

- [Computed three-by-three LU decomposition](computed-three-by-three-lu-decomposition.md)
- [Unit triangular matrix](unit-triangular-matrix.md)
- [Triangular solves for LU decomposition](triangular-solves-for-lu-decomposition.md)
  - [Forward substitution](forward-substitution.md)
- [Pivoted LU decomposition](pivoted-lu-decomposition.md)
- [Reusing LU factors for multiple right-hand sides](reusing-lu-factors-for-multiple-right-hand-sides.md)
- [LU factorization and solve costs](lu-factorization-and-solve-costs.md)

## ↑ Ancestors (6)

1. [Numerical linear algebra](numerical-linear-algebra.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Columnwise partial pivoting](columnwise-partial-pivoting.md)
- [Computed three-by-three LU decomposition](computed-three-by-three-lu-decomposition.md)
- [Elimination multiplier](elimination-multiplier.md)
- [LU decomposition](lu-decomposition.md)
- [LU factorization and solve costs](lu-factorization-and-solve-costs.md)
- [Matrix inverse](matrix-inverse.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/5e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-2/5b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1/6d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/5c/a/solution.md)
- [Rank-one matrix update](rank-one-matrix-update.md)
- [Reusing LU factors for multiple right-hand sides](reusing-lu-factors-for-multiple-right-hand-sides.md)
- [Sherman–Morrison formula](sherman-morrison-formula.md)
- [Triangular solves for LU decomposition](triangular-solves-for-lu-decomposition.md)
- [Tridiagonal elimination recurrences](tridiagonal-elimination-recurrences.md)
- [Tridiagonal solve costs](tridiagonal-solve-costs.md)
- [Unit triangular matrix](unit-triangular-matrix.md)
