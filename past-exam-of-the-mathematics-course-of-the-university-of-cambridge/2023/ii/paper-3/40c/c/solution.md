<h1 id="40c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $Ax^*=b$, the error $e^{(k)}=x^*-x^{(k)}$ obeys

$$
e^{(k+1)}
=((1+\beta)I-\alpha A)e^{(k)}
-\beta e^{(k-1)}.
$$

Thus the [heavy-ball error propagation matrix](../../../../../../heavy-ball-error-propagation-matrix.md) is

$$
\boxed{
\begin{pmatrix}e^{(k+1)}\\ e^{(k)}\end{pmatrix}
=
M\begin{pmatrix}e^{(k)}\\e^{(k-1)}\end{pmatrix},
\qquad
M=
\begin{pmatrix}
(1+\beta)I-\alpha A&-\beta I\\
I&0
\end{pmatrix}.}
$$

If $A=\operatorname{diag}(\lambda_1,\ldots,\lambda_n)$, permute the coordinates from

$$
(e_1^{(k)},\ldots,e_n^{(k)},e_1^{(k-1)},\ldots,e_n^{(k-1)})
$$

to

$$
(e_1^{(k)},e_1^{(k-1)},\ldots,e_n^{(k)},e_n^{(k-1)}).
$$

For the corresponding [permutation matrix](../../../../../../permutation-matrix.md) $P$,

$$
\boxed{
PMP^T=\operatorname{diag}(M_1,\ldots,M_n),
\qquad
M_i=
\begin{pmatrix}
1+\beta-\alpha\lambda_i&-\beta\\
1&0
\end{pmatrix}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [40C](../../40c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
