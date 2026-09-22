<h1 id="2a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expanding the [characteristic polynomial](../../../../../../characteristic-polynomial.md) gives

$$
\det(\lambda I-A)=\lambda^3-2\lambda^2-\lambda+2
=(\lambda+1)(\lambda-1)(\lambda-2).
$$

Solving the three nullspace systems gives **the [eigenvalues](../../../../../../eigenvalue.md) and [eigenspaces](../../../../../../eigenspace.md)**

$$
\boxed{E_{-1}=\operatorname{span}\{(1,1,1)^T\},\quad
E_1=\operatorname{span}\{(1,1,0)^T\},\quad
E_2=\operatorname{span}\{(0,1,-1)^T\}.}
$$

For example, at $\lambda=1$ the first two equations force $z=0$ and $x=y$; at $\lambda=2$ they force $x=0$ and $y=-z$; at $\lambda=-1$ they force $x=y=z$.

Putting these [eigenvectors](../../../../../../eigenvector.md) in columns proves their [linear independence](../../../../../../linear-independence.md):

$$
P=\begin{pmatrix}1&1&0\\1&1&1\\1&0&-1\end{pmatrix},\qquad\det P=1,\qquad
P^{-1}AP=\operatorname{diag}(-1,1,2).
$$

Hence **$A$ is a [diagonalizable matrix](../../../../../../diagonalizable-matrix.md) over the reals**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2A](../../2a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
