# Positive diagonal symmetrization of a tridiagonal matrix

↑ **Parent:** [Positive diagonal symmetrization of a matrix](positive-diagonal-symmetrization-of-a-matrix.md)

Let a real [tridiagonal matrix](tridiagonal-matrix.md) have diagonal entries $a_i$, positive upper entries $b_i$, and positive lower entries $c_i$. Set $d_1=1$, $d_{i+1}=d_i\sqrt{c_i/b_i}$ and $D=\operatorname{diag}(d_i)$. Then $D^{-1}AD$ is a [symmetric matrix](symmetric-matrix.md) with diagonal $a_i$ and adjacent entries $\sqrt{b_ic_i}$. Indeed its two adjacent entries are $b_id_{i+1}/d_i$ and $c_id_i/d_{i+1}$, which are equal by construction. All other zeros are preserved. This [matrix similarity](matrix-similarity.md) implies real [eigenvalues](eigenvalue.md) and [diagonalizability](diagonalizable-matrix.md), by the [spectral theorem for real symmetric matrices](spectral-theorem-for-real-symmetric-matrices.md). No sign assumption on $a_i$ is needed. In the weighted formulation of [positive diagonal symmetrization of a matrix](positive-diagonal-symmetrization-of-a-matrix.md), the positive [diagonal matrix](diagonal-matrix.md) is $W=D^{-2}$.

## ↑ Ancestors (8)

1. [Positive diagonal symmetrization of a matrix](positive-diagonal-symmetrization-of-a-matrix.md)
2. [Similarity transformation](similarity-transformation.md)
3. [Matrix similarity](matrix-similarity.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/5/b/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/5/b/ii/solution.md)
