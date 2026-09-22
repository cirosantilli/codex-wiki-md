<h1 id="14e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Full column rank makes $B=A^TA$ positive definite: for nonzero $v$, $v^TBv=\|Av\|^2>0$. Let $B=R^TR$ be its unique upper-triangular [Cholesky decomposition](../../../../../../cholesky-decomposition.md) with positive diagonal. Defining $Q=AR^{-1}$ gives

$$
Q^TQ=R^{-T}A^TAR^{-1}=I,\qquad A=QR.
$$

Thus the skinny [QR decomposition](../../../../../../qr-decomposition.md) exists. If $A=\widetilde Q\widetilde R$ is another such decomposition, orthonormality gives $A^TA=\widetilde R^T\widetilde R$. Cholesky uniqueness forces $\widetilde R=R$, and then $\widetilde Q=AR^{-1}=Q$. Therefore **the skinny factorization with positive diagonal is unique**. This is the [thin QR factorization from Cholesky decomposition](../../../../../../thin-qr-factorization-from-cholesky-decomposition.md); no inverse of the rectangular $Q$ is assumed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14E](../../14e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
