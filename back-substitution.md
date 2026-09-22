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

## ← Incoming links (2)

- [Householder reduction of an overdetermined consistent system](householder-reduction-of-an-overdetermined-consistent-system.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1/18c/solution.md)
