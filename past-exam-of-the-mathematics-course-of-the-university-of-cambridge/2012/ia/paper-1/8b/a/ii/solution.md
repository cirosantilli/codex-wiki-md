<h1 id="8b/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The quadratic expression is $\mathbf x^TA\mathbf x$. Normalize the preceding [eigenvectors](../../../../../../../eigenvector.md) to obtain an [orthonormal basis](../../../../../../../orthonormal-basis.md)

$$
\mathbf u_1=\frac{(1,-1,-1)^T}{\sqrt3},\quad
\mathbf u_2=\frac{(0,1,-1)^T}{\sqrt2},\quad
\mathbf u_3=\frac{(2,1,1)^T}{\sqrt6}.
$$

With the [orthogonal matrix](../../../../../../../orthogonal-matrix.md) $U=(\mathbf u_1\ \mathbf u_2\ \mathbf u_3)$ and coordinates $\mathbf y=U^T\mathbf x$, the surface equation becomes $y_1^2+2y_2^2+4y_3^2=1$. All coefficients are positive, so **it is an [ellipsoid](../../../../../../../ellipsoid.md)**, with principal semiaxes $1,1/\sqrt2,1/2$ along the respective [eigenvectors](../../../../../../../eigenvector.md). This is [principal-axis reduction of a quadric](../../../../../../../principal-axis-reduction-of-a-quadric.md).

A map to the unit [sphere](../../../../../../../sphere.md) is $\mathbf x\mapsto\operatorname{diag}(1,\sqrt2,2)U^T\mathbf x$. One explicit matrix is

$$
\boxed{B=\begin{pmatrix}1/\sqrt3&-1/\sqrt3&-1/\sqrt3\\0&1&-1\\4/\sqrt6&2/\sqrt6&2/\sqrt6\end{pmatrix}.}
$$

Indeed $B^TB=A$, so $|B\mathbf x|^2=\mathbf x^TA\mathbf x$. Since $B$ is invertible, every point on the unit [sphere](../../../../../../../sphere.md) has a preimage on the [ellipsoid](../../../../../../../ellipsoid.md); the map is onto, not merely into. The requested $B$ is not unique, since an additional [orthogonal matrix](../../../../../../../orthogonal-matrix.md) on the left preserves the unit [sphere](../../../../../../../sphere.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [8B](../../../8b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
