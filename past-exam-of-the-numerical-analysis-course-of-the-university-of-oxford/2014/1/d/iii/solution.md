<h1 id="1/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

With $A_0=A$, repeat the shifted [QR algorithm](../../../../../qr-algorithm.md):

$$
\boxed{A_k-\mu_kI=Q_kR_k,\qquad A_{k+1}=R_kQ_k+\mu_kI.}
$$

The [QR shift](../../../../../qr-shift.md) $\mu_k$ is chosen from $A_k$, for example its bottom-right entry or an [eigenvalue](../../../../../eigenvalue.md) of a trailing two-by-two block. Explicitly using the [orthogonality](../../../../../orthogonal-vectors.md) of $Q_k$ gives

$$
A_{k+1}=Q_k^T(A_k-\mu_kI)Q_k+\mu_kI=Q_k^TA_kQ_k.
$$

Thus each update is a [matrix similarity](../../../../../matrix-similarity.md) preserving [eigenvalues](../../../../../eigenvalue.md). Accumulate $Q_0Q_1\cdots Q_k$ if [eigenvectors](../../../../../eigenvector.md) or the full reduction are wanted. Once a subdiagonal entry is negligible, [block deflation in the QR algorithm](../../../../../block-deflation-in-the-qr-algorithm.md) separates the corresponding blocks and iteration continues on the active block.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
