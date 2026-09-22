# Exact-shift diagonalization of a two-state swap matrix

↑ **Parent:** [QR algorithm](qr-algorithm.md)

For $A=\left(\begin{smallmatrix}0&1\\1&0\end{smallmatrix}\right)$, one shifted [QR algorithm](qr-algorithm.md) step with real [QR shift](qr-shift.md) $\mu$ gives, with a consistent choice of factor signs,

$$
A_1=\frac1{1+\mu^2}\begin{pmatrix}-2\mu&\mu^2-1\\\mu^2-1&2\mu\end{pmatrix}.
$$

To verify this, factor $A-\mu I=QR$ with $Q=(1+\mu^2)^{-1/2}\left(\begin{smallmatrix}-\mu&-1\\1&-\mu\end{smallmatrix}\right)$. Its columns are [orthonormal](orthonormal-set.md), and $R=Q^T(A-\mu I)$ is upper triangular. Then $A_1=Q^TAQ$. Thus $A_1$ is diagonal exactly when $\mu=\pm1$, the two [eigenvalues](eigenvalue.md). The bottom-right-entry shift is zero and leaves the [matrix](matrix.md) unchanged under the positive-diagonal factor convention. This illustrates why a poorly chosen [QR shift](qr-shift.md) can stall even a two-by-two symmetric [eigenvalue](eigenvalue.md) computation.

## ↑ Ancestors (6)

1. [QR algorithm](qr-algorithm.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2014/1/f/solution.md)
- [QR shift](qr-shift.md)
