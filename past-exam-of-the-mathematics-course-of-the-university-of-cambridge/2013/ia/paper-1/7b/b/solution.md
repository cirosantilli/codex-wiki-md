<h1 id="7b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Represent the [quadratic form](../../../../../../quadratic-form.md) by the [symmetric matrix](../../../../../../symmetric-matrix.md)

$$
H=\begin{pmatrix}2&-2&0\\-2&5&0\\0&0&-1\end{pmatrix}.
$$

The $xy$ block has [characteristic polynomial](../../../../../../characteristic-polynomial.md) $(2-\mu)(5-\mu)-4=(\mu-1)(\mu-6)$. Corresponding orthonormal [eigenvectors](../../../../../../eigenvector.md), together with the $z$ direction, are

$$
\boxed{\widetilde e_1=\frac1{\sqrt5}(2,1,0)^T,\qquad
\widetilde e_2=\frac1{\sqrt5}(-1,2,0)^T,\qquad
\widetilde e_3=(0,0,1)^T.}
$$

The [eigenvalues](../../../../../../eigenvalue.md) are $1,6,-1$. To eliminate the linear term, solve $H\widetilde O=-(0,3\sqrt5,0)^T$, obtaining

$$
\boxed{\widetilde O=(-\sqrt5,-\sqrt5,0)^T.}
$$

Indeed the first equation gives $x=y$, and the second then gives $3y=-3\sqrt5$. Define the new coordinates by $X=\widetilde O+\widetilde x\,\widetilde e_1+\widetilde y\,\widetilde e_2+\widetilde z\,\widetilde e_3$. The original polynomial takes the value $-15$ at the center, so its translated and orthogonally diagonalized form is

$$
\widetilde x^2+6\widetilde y^2-\widetilde z^2=15.
$$

Thus

$$
\boxed{\alpha=\frac1{15},\qquad\beta=\frac25,\qquad\gamma=-\frac1{15}.}
$$

The surface is an **elliptic [one-sheet hyperboloid](../../../../../../one-sheet-hyperboloid.md)**, centered at $\widetilde O$, with axis parallel to $\widetilde e_3$. Its waist at $\widetilde z=0$ is an ellipse with semiaxes $\sqrt{15}$ and $\sqrt{5/2}$. Every constant-$\widetilde z$ section is a nonempty ellipse, so the two signs of $\widetilde z$ belong to the same connected sheet. This is an application of [principal-axis reduction of a quadric](../../../../../../principal-axis-reduction-of-a-quadric.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7B](../../7b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
