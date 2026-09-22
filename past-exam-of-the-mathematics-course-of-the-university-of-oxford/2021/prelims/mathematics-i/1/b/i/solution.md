<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

For the given [real matrix](../../../../../../../real-matrix.md) $M$, direct [matrix multiplication](../../../../../../../matrix-multiplication.md) gives the [eigenvectors](../../../../../../../eigenvector.md)

$$
M\begin{pmatrix}1\\0\\1\end{pmatrix}=0,\qquad
M\begin{pmatrix}0\\1\\1\end{pmatrix}=2\begin{pmatrix}0\\1\\1\end{pmatrix},\qquad
M\begin{pmatrix}1\\1\\0\end{pmatrix}=4\begin{pmatrix}1\\1\\0\end{pmatrix}.
$$

Put these [eigenvectors](../../../../../../../eigenvector.md) into the columns of

$$
P=\begin{pmatrix}1&0&1\\0&1&1\\1&1&0\end{pmatrix},\qquad
P^{-1}=\frac12\begin{pmatrix}1&-1&1\\-1&1&1\\1&1&-1\end{pmatrix}.
$$

Since $\det P=-2\ne0$, $P$ is an [invertible matrix](../../../../../../../invertible-matrix.md). The three column identities give $MP=PD$, so

$$
\boxed{D=P^{-1}MP=\operatorname{diag}(0,2,4),\qquad M=PDP^{-1}.}
$$

In particular, the [matrix similarity](../../../../../../../matrix-similarity.md) is established by an explicit [change-of-basis matrix](../../../../../../../change-of-basis-matrix.md).

## ↑ Ancestors (13)

1. [i](../i.md)
2. [b](../../b.md)
3. [1](../../../1.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
