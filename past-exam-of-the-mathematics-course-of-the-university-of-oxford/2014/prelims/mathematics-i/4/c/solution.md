<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the given symmetric [matrix](../../../../../../matrix.md), $(1,1)^T$ is an [eigenvector](../../../../../../eigenvector.md) with [eigenvalue](../../../../../../eigenvalue.md) $1$, and $(1,-1)^T$ is an [eigenvector](../../../../../../eigenvector.md) with [eigenvalue](../../../../../../eigenvalue.md) $27$. Normalize them to obtain

$$
P=\frac1{\sqrt2}\begin{pmatrix}1&1\\1&-1\end{pmatrix},\qquad
A=P\begin{pmatrix}1&0\\0&27\end{pmatrix}P^T.
$$

Take the real cube roots of the two diagonal entries and transform back:

$$
\boxed{C=P\begin{pmatrix}1&0\\0&3\end{pmatrix}P^T
=\begin{pmatrix}2&-1\\-1&2\end{pmatrix}.}
$$

It is a real [symmetric matrix](../../../../../../symmetric-matrix.md), and $C^3=P\operatorname{diag}(1,27)P^T=A$ because $P^TP=I$. Direct multiplication also gives $C^2=\begin{pmatrix}5&-4\\-4&5\end{pmatrix}$ and then $C^3=\begin{pmatrix}14&-13\\-13&14\end{pmatrix}$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
