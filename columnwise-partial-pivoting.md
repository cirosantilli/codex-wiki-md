# Columnwise partial pivoting

↑ **Parent:** [Gaussian elimination](gaussian-elimination.md)

At each step of [Gaussian elimination](gaussian-elimination.md), select the largest absolute entry in the uneliminated part of the current column and interchange rows to put it on the diagonal. A nonsingular trailing [Schur complement](schur-complement.md) has a nonzero entry in its first column, so this procedure always finds a nonzero pivot in exact arithmetic. The [permutation matrix](permutation-matrix.md) $P$ records row interchanges; earlier multipliers must be interchanged too when assembling the lower-triangular factor. This yields the [LU decomposition](lu-decomposition.md) $PA=LU$ with unit diagonal in $L$. Searching within columns and interchanging rows is distinct from interchanging columns.

## ↑ Ancestors (7)

1. [Gaussian elimination](gaussian-elimination.md)
2. [Numerical linear algebra](numerical-linear-algebra.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1/6d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1/6d/b/solution.md)
