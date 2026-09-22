<h1 id="19d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The first column is $a=(2,1,2)^T$ with length three. Choose $v=a-3e_1=(-1,1,2)^T$, so $v^Tv=6$. Its [Householder reflection](../../../../../../householder-transformation.md) is

$$
H_1=I-\frac13vv^T=
\begin{pmatrix}2/3&1/3&2/3\\1/3&2/3&-2/3\\2/3&-2/3&-1/3\end{pmatrix}.
$$

Direct multiplication gives

$$
H_1A=\begin{pmatrix}3&3\\0&0\\0&3\end{pmatrix},\qquad
H_1b=\begin{pmatrix}3\\3\\-3\end{pmatrix}.
$$

To eliminate the remaining third-row entry in the second column, reflect the last two coordinates using $v_2=(0,1,-1)^T$. Then

$$
H_2=I-v_2v_2^T=\begin{pmatrix}1&0&0\\0&0&1\\0&1&0\end{pmatrix},
$$

and

$$
H_2H_1A=\begin{pmatrix}3&3\\0&3\\0&0\end{pmatrix},\qquad
H_2H_1b=\begin{pmatrix}3\\-3\\3\end{pmatrix}.
$$

Both steps are [Householder reflections](../../../../../../householder-transformation.md); the second happens to exchange two coordinates. Solve the leading triangular equations $3x_1+3x_2=3$ and $3x_2=-3$ to obtain

$$
\boxed{x^*=\begin{pmatrix}2\\-1\end{pmatrix},\qquad
\min_x\|Ax-b\|_2=3.}
$$

For an independent check, $Ax^*-b=(-1,-2,2)^T$, whose squared norm is nine and which is orthogonal to both columns of $A$. Thus $A^T(Ax^*-b)=0$, confirming the least-squares minimizer.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [19D](../../19d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
