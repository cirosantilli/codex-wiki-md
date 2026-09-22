# Accumulated QR factorization identity

↑ **Parent:** [Unshifted QR algorithm](unshifted-qr-algorithm.md)

Let

$$
\overline Q_k=Q_0Q_1\cdots Q_k,
\qquad
\overline R_k=R_kR_{k-1}\cdots R_0.
$$

Then

$$
A_{k+1}=\overline Q_k^TA\overline Q_k,
\qquad
A^{k+1}=\overline Q_k\overline R_k.
$$

Thus $\overline Q_k\overline R_k$ is a [QR decomposition](qr-decomposition.md) of the matrix power $A^{k+1}$. In particular, the first $r$ columns of $\overline Q_k$ span the same subspace as the first $r$ columns of $A^{k+1}$ whenever those columns are independent.

## ↑ Ancestors (7)

1. [Unshifted QR algorithm](unshifted-qr-algorithm.md)
2. [Numerical linear algebra](numerical-linear-algebra.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/41e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/41e/b/solution.md)
