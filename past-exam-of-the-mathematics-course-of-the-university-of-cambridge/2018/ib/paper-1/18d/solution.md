<h1 id="18d/solution">Solution</h1>

↑ **Parent:** [18D](../18d.md)

Let $P=uu^T/\|u\|^2$. This is an [orthogonal projection matrix](../../../../../orthogonal-projection-matrix.md), so $P^T=P$ and $P^2=P$. Therefore the [Householder transformation](../../../../../householder-transformation.md)

$$
H_u=I-2P
$$

satisfies $H_u^TH_u=(I-2P)^2=I$. If $\|a\|=\|b\|$ and $a\ne b$, then

$$
\|a-b\|^2=2(a-b)^Ta,
$$

and hence $H_{a-b}a=a-(a-b)=b$.

Apply a Householder transformation to the first column of $A$ to map it to a multiple of $e_1$, then apply transformations supported on the trailing coordinates to clear each later column below its diagonal. Their product is orthogonal and produces $R$; reversing the product gives $A=QR$.

For the displayed matrix, one resulting factorization is

$$
\boxed{
Q=\frac12\begin{pmatrix}
1&-1&1&1\\
1&1&-1&1\\
1&1&1&-1\\
1&-1&-1&-1
\end{pmatrix},
\qquad
R=\begin{pmatrix}
2&3&2\\
0&5&-2\\
0&0&4\\
0&0&0
\end{pmatrix}.}
$$

Direct multiplication gives the stated $A$, and $Q^TQ=I$.

## ↑ Ancestors (10)

1. [18D](../18d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
