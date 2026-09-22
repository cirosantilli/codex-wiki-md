# QR shift

↑ **Parent:** [QR algorithm](qr-algorithm.md)

A [QR shift](qr-shift.md) is a scalar $\mu_k$ subtracted before the [QR factorization](qr-decomposition.md) in a [QR algorithm](qr-algorithm.md) step and restored after reversing the factors:

$$
A_k-\mu_kI=Q_kR_k,\qquad A_{k+1}=R_kQ_k+\mu_kI=Q_k^TA_kQ_k.
$$

The final identity uses the [orthogonality](orthogonal-vectors.md) of $Q_k$, proving that the [eigenvalues](eigenvalue.md) are preserved. Choosing a shift near an [eigenvalue](eigenvalue.md) can accelerate [block deflation in the QR algorithm](block-deflation-in-the-qr-algorithm.md). A common choice is the current bottom-right entry, but it can stall, as in [Exact-shift diagonalization of a two-state swap matrix](exact-shift-diagonalization-of-a-two-state-swap-matrix.md).

## ↑ Ancestors (6)

1. [QR algorithm](qr-algorithm.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Exact-shift diagonalization of a two-state swap matrix](exact-shift-diagonalization-of-a-two-state-swap-matrix.md)
- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2014/1/d/iii/solution.md)
- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2014/1/e/solution.md)
- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2014/1/f/solution.md)
- [QR shift](qr-shift.md)
