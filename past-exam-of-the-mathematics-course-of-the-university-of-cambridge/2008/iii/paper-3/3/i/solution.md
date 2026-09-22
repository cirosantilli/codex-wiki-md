<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Preserving the symmetric [bilinear form](../../../../../../bilinear-form.md) infinitesimally means $Z^TM+MZ=0$. In blocks of sizes $2,2,1$, write $Z$ as a general block matrix and multiply by the given $M$. The condition says that $MZ$ is skew-symmetric. It forces the lower-right entry to be zero, the middle diagonal block to be the negative transpose of the upper-left block, and the two off-diagonal two-by-two blocks to be skew-symmetric. Thus the general element of the [Special orthogonal Lie algebra](../../../../../../special-orthogonal-lie-algebra.md) is

$$
\boxed{Z=\begin{pmatrix}
A&B&p\\
C&-A^T&q\\
-q^T&-p^T&0
\end{pmatrix},\qquad B^T=-B,\ C^T=-C,}
$$

where $A$ is an arbitrary two-by-two [matrix](../../../../../../matrix.md) and $p,q$ are arbitrary two-component columns. More explicitly, using ten independent complex parameters,

$$
Z=\begin{pmatrix}
a&b&0&e&p_1\\
c&d&-e&0&p_2\\
0&f&-a&-c&q_1\\
-f&0&-b&-d&q_2\\
-q_1&-q_2&-p_1&-p_2&0
\end{pmatrix}.
$$

Conversely, substituting this matrix into $Z^TM+MZ$ gives zero, so there are no further restrictions. In particular $\dim\mathfrak{so}_5=4+1+1+2+2=10$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
