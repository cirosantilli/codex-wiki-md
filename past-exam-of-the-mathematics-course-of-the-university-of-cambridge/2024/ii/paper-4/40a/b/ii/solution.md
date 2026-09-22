<h1 id="40a/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Since $A_k=Q_kR_k$,

$$
A_{k+1}=R_kQ_k=Q_k^TA_kQ_k.
$$

Thus every step is an orthogonal similarity, so it preserves [eigenvalues](../../../../../../../eigenvalue.md) and symmetry.

For a symmetric $r$-banded [matrix](../../../../../../../matrix.md), its subdiagonal entries can be eliminated by Givens rotations ordered along the band. Each rotation creates only the next local bulge; multiplication in reverse order chases that bulge out without creating entries beyond the original upper band. Symmetry supplies the corresponding lower band. This is [symmetric bandwidth preservation under QR iteration](../../../../../../../symmetric-bandwidth-preservation-under-qr-iteration.md), and proves that $A_{k+1}$ is again $r$-banded.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [40A](../../../40a.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
