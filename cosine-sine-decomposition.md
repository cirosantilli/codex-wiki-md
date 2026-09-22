# Cosine-sine decomposition

↑ **Parent:** [Singular value decomposition](singular-value-decomposition.md)

If a [matrix](matrix.md) with [orthonormal](orthonormal-set.md) columns is divided into two row blocks, each having at least as many rows as there are columns, it admits simultaneous thin factorizations $A_1=U_1CV^T$, $A_2=U_2SV^T$, with [orthonormal](orthonormal-set.md) $U_1,U_2$, an [orthogonal matrix](orthogonal-matrix.md) $V$, and nonnegative [diagonal matrices](diagonal-matrix.md) $C,S$ satisfying $C^2+S^2=I$. To prove this, apply the [spectral theorem](spectral-theorem.md) to $A_1^TA_1$; the same [orthonormal eigenbasis](orthonormal-eigenbasis.md) diagonalizes $A_2^TA_2=I-A_1^TA_1$. Normalize the nonzero columns of $A_iV$ and complete the zero columns to [orthonormal sets](orthonormal-set.md). The entries of $C,S$ can be written as cosines and sines of angles in $[0,\pi/2]$.

## ↑ Ancestors (6)

1. [Singular value decomposition](singular-value-decomposition.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2025/1/a/iii/solution.md)
