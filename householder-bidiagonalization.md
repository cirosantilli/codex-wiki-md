# Householder bidiagonalization

↑ **Parent:** [Householder transformation](householder-transformation.md)

Alternating right and left [Householder transformations](householder-transformation.md) reduce a real square matrix to a [bidiagonal matrix](bidiagonal-matrix.md). For a lower-bidiagonal result, first clear row $j$ beyond column $j$ using a right transformation on trailing columns. Then clear column $j$ below row $j+1$ using a left transformation on trailing rows. Previously completed rows and columns are preserved. Since $B^TB=Q^TA^TAQ$ is a symmetric [tridiagonal matrix](tridiagonal-matrix.md), its [eigenvalues](eigenvalue.md) are the squares of the [singular values](singular-value.md) of $A$. This explains the reduction structurally; explicitly forming $A^TA$ is unnecessary and can worsen numerical conditioning.

## ↑ Ancestors (6)

1. [Householder transformation](householder-transformation.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford/2008/1/d/solution.md)
