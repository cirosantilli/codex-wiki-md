<h1 id="41e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Each [QR decomposition](../../../../../../qr-decomposition.md) $A_k=Q_kR_k$ gives

$$
A_{k+1}=R_kQ_k=Q_k^TA_kQ_k.
$$

Induction therefore yields the first [Accumulated QR factorization identity](../../../../../../accumulated-qr-factorization-identity.md):

$$
\boxed{A_{k+1}=\overline Q_k^TA\overline Q_k},
\qquad
\overline Q_k=Q_0Q_1\cdots Q_k.
$$

We next prove the corresponding factorization of a [matrix power](../../../../../../matrix-power.md). The case $k=0$ is just $A=Q_0R_0$. If

$$
A^{k+1}=\overline Q_k\overline R_k,
\qquad
\overline R_k=R_kR_{k-1}\cdots R_0,
$$

then the similarity formula above implies

$$
A\overline Q_k=\overline Q_kA_{k+1}.
$$

Consequently,

$$
\begin{aligned}
A^{k+2}
&=A\overline Q_k\overline R_k\\
&=\overline Q_kA_{k+1}\overline R_k\\
&=\overline Q_kQ_{k+1}R_{k+1}\overline R_k\\
&=\overline Q_{k+1}\overline R_{k+1}.
\end{aligned}
$$

The product $\overline Q_k$ is [orthogonal](../../../../../../orthogonal-matrix.md), and the product $\overline R_k$ is [upper triangular](../../../../../../triangular-matrix.md). Hence

$$
\boxed{A^{k+1}=\overline Q_k\overline R_k}
$$

is a QR decomposition.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [41E](../../41e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
