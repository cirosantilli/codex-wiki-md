<h1 id="8f/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Over $\mathbb C$, the real [skew-symmetric matrix](../../../../../../../skew-symmetric-matrix.md) $A$ is normal because $A^*=-A$. Part (a) gives an orthonormal complex eigenbasis, and the nonzero eigenvalues are purely imaginary pairs $\pm i\lambda$.

For each $\lambda>0$, choose a unit real vector $x$ in the kernel of $A^2+\lambda^2I$ and put

$$
y=-\frac1\lambda Ax.
$$

Then $x\perp y$, $\|y\|=1$, and

$$
Ax=-\lambda y,\qquad Ay=\lambda x.
$$

Thus $A$ has matrix

$$
\begin{pmatrix}0&\lambda\\-\lambda&0\end{pmatrix}
$$

on the orthonormal basis $(x,y)$. Distinct such invariant planes are orthogonal; complete them by an orthonormal basis of $\ker A$. Taking these basis vectors as the columns of an [orthogonal matrix](../../../../../../../orthogonal-matrix.md) $R$ gives

$$
\boxed{R^TAR
=\operatorname{diag}\left(
\begin{pmatrix}0&\lambda_1\\-\lambda_1&0\end{pmatrix},
\ldots,
\begin{pmatrix}0&\lambda_r\\-\lambda_r&0\end{pmatrix},
0\right)}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8F](../../../8f.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ib](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
