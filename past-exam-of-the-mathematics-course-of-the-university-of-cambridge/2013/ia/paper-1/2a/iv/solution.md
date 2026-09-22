<h1 id="2a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Each plane rotation satisfies $R_j^TR_j=I$. Hence $U=R_3R_2R_1$ is an [orthogonal matrix](../../../../../../orthogonal-matrix.md) and $D=UA$ is an [upper triangular matrix](../../../../../../upper-triangular-matrix.md). Multiplication by $U^T$ gives the [QR decomposition](../../../../../../qr-decomposition.md)

$$
\boxed{A=QD,\qquad Q=R_1^TR_2^TR_3^T,\qquad Q^TQ=I.}
$$

The zero-pair cases already handled make this construction valid for every real $3\times3$ matrix, including rank-deficient matrices. Orthogonality follows from the product identity, not from any invertibility assumption on $A$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2A](../../2a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
