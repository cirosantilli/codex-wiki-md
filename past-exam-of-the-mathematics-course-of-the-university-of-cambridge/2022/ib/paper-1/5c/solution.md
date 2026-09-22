<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

Let the columns of $A$ be $a_1,a_2,a_3$. The [Gram-Schmidt process](../../../../../gram-schmidt-process.md) gives

$$
q_1=\frac{a_1}{|a_1|}
=\frac12(1,1,1,-1)^T,
\qquad r_{11}=4.
$$

Next,

$$
r_{12}=q_1^Ta_2=2,
\qquad
a_2-r_{12}q_1=(1,-1,1,1)^T,
$$

so

$$
q_2=\frac12(1,-1,1,1)^T,
\qquad r_{22}=2.
$$

For the final column,

$$
r_{13}=q_1^Ta_3=-2,
\qquad
r_{23}=q_2^Ta_3=4,
$$

and

$$
a_3-r_{13}q_1-r_{23}q_2=(-1,-1,1,-1)^T.
$$

Thus $q_3=\frac12(-1,-1,1,-1)^T$ and $r_{33}=2$. The reduced [QR decomposition](../../../../../qr-decomposition.md) is

$$
\boxed{
Q=\frac12
\begin{pmatrix}
1&1&-1\\
1&-1&-1\\
1&1&1\\
-1&1&-1
\end{pmatrix},
\qquad
R=
\begin{pmatrix}
4&2&-2\\
0&2&4\\
0&0&2
\end{pmatrix}}.
$$

The columns of $Q$ are orthonormal, and direct multiplication gives $QR=A$.

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
