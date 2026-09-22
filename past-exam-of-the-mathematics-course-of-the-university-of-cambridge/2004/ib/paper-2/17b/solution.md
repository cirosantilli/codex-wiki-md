<h1 id="17b/solution">Solution</h1>

↑ **Parent:** [17B](../17b.md)

Use coordinates $\mathbf r$ measured from the [center of mass](../../../../../center-of-mass.md) $G$, so $\int\mathbf r\,dm=0$. The displacement from $P$ is $\mathbf r-\mathbf X$. Expand the defining [inertia tensor](../../../../../inertia-tensor.md):

$$
I_{ij}(P)=\int\left[|\mathbf r-\mathbf X|^2\delta_{ij}-(r_i-X_i)(r_j-X_j)\right]dm.
$$

All terms linear in $\mathbf r$ integrate to zero. The remaining constant terms give the [tensor parallel-axis theorem](../../../../../tensor-parallel-axis-theorem.md),

$$
\boxed{I_{ij}(P)=I_{ij}(G)+M\left(|\mathbf X|^2\delta_{ij}-X_iX_j\right).}
$$

For the uniform cube, let $M=8\rho a^3$. Symmetry makes the off-diagonal [inertia tensor](../../../../../inertia-tensor.md) entries zero. Direct integration gives $\int x_i^2\,dm=Ma^2/3$ for each coordinate, and therefore $I(G)=(2Ma^2/3)I_3$. With $\mathbf X=a(1,1,1)^T$, the [tensor parallel-axis theorem](../../../../../tensor-parallel-axis-theorem.md) gives

$$
\boxed{I(P)=Ma^2\begin{pmatrix}8/3&-1&-1\\-1&8/3&-1\\-1&-1&8/3\end{pmatrix}
=Ma^2\left(\frac{11}3I_3-\mathbf1\mathbf1^T\right).}
$$

The unit [eigenvector](../../../../../eigenvector.md) $u=(1,1,1)^T/\sqrt3$ has [eigenvalue](../../../../../eigenvalue.md) $2Ma^2/3$. Every vector in the plane $x+y+z=0$ is annihilated by $\mathbf1\mathbf1^T$ and hence has [eigenvalue](../../../../../eigenvalue.md) $11Ma^2/3$. One orthonormal [basis](../../../../../basis.md) of that eigenspace is

$$
v=\frac{(1,-1,0)^T}{\sqrt2},\qquad w=\frac{(1,1,-2)^T}{\sqrt6}.
$$

**The principal moments are $2Ma^2/3$ along the body diagonal and $11Ma^2/3$ twice in its perpendicular plane.** Any orthonormal pair in that plane supplies the remaining principal axes.

## ↑ Ancestors (10)

1. [17B](../17b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
