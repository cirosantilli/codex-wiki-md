<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a real square [matrix](../../../../matrix.md), a [QR factorization](../../../../qr-decomposition.md) writes $B=QR$ with $Q$ an [orthogonal matrix](../../../../orthogonal-matrix.md), $Q^TQ=I$, and $R$ an [upper triangular matrix](../../../../upper-triangular-matrix.md). If $B$ is invertible, so is $R$, and

$$
Bx=b\quad\Longleftrightarrow\quad Rx=Q^Tb.
$$

Compute $Q^Tb$ and use [back substitution](../../../../back-substitution.md); no [matrix inverse](../../../../matrix-inverse-split.md) needs to be formed.

Apply the [Gram-Schmidt process](../../../../gram-schmidt-process.md) to the columns $b_1,b_2,b_3$. The first column has [Euclidean norm](../../../../euclidean-norm.md) two, giving $q_1=(1,0,0)^T$ and $r_{11}=2$. For the second column,

$$
r_{12}=q_1^Tb_2=1,\qquad b_2-r_{12}q_1=(0,4,3)^T,
\qquad r_{22}=5,\qquad q_2=(0,4/5,3/5)^T.
$$

For the third column,

$$
r_{13}=q_1^Tb_3=0,\qquad r_{23}=q_2^Tb_3=7,
\qquad b_3-7q_2=(0,-3/5,4/5)^T.
$$

This residual already has [Euclidean norm](../../../../euclidean-norm.md) one. Set $q_3=(0,-3/5,4/5)^T$ and $r_{33}=1$. Thus

$$
\boxed{Q=\begin{pmatrix}1&0&0\\0&4/5&-3/5\\0&3/5&4/5\end{pmatrix},\qquad
R=\begin{pmatrix}2&1&0\\0&5&7\\0&0&1\end{pmatrix}.}
$$

The columns of $Q$ are [orthonormal](../../../../orthonormal-set.md), and [matrix multiplication](../../../../matrix-multiplication.md) verifies $QR=B$.

Using precisely this [QR factorization](../../../../qr-decomposition.md), transform the right-hand side:

$$
Q^T\begin{pmatrix}-3\\1\\2\end{pmatrix}
=\begin{pmatrix}-3\\(4+6)/5\\(-3+8)/5\end{pmatrix}
=\begin{pmatrix}-3\\2\\1\end{pmatrix}.
$$

[Back substitution](../../../../back-substitution.md) in $Rx=Q^Tb$ gives

$$
x_3=1,\qquad 5x_2+7=2\ \Longrightarrow\ x_2=-1,
\qquad 2x_1-1=-3\ \Longrightarrow\ x_1=-1.
$$

Therefore

$$
\boxed{x=(-1,-1,1)^T.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
