<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The coefficients in the spherical [Laplacian](../../../../../../laplacian.md) are independent of $\phi$, so $[\Delta,\partial_\phi]=0$. Also $\partial_\phi$ is tangent to both boundary spheres; differentiating the zero boundary trace gives another zero trace. Therefore $w=\partial_\phi u$ satisfies $\Delta w=\partial_\phi f$ and the same homogeneous [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md).

In Cartesian coordinates $\partial_\phi=x_1\partial_2-x_2\partial_1$, a globally smooth rotation field even where angular coordinates are singular. Permuting coordinate axes gives $R_{12}$, $R_{23}$ and $R_{31}$. For each, the [rotational commutator for the Laplacian](../../../../../../rotational-commutator-for-the-laplacian.md) follows directly from $\Delta(x_i\partial_ju)=x_i\partial_j\Delta u+2\partial_i\partial_ju$; antisymmetrizing cancels the extra terms. Thus

$$
\boxed{\Delta(R_{ij}u)=R_{ij}f,\qquad R_{ij}u|_{\partial\Omega}=0.}
$$

If $f$ is radial, all these right-hand sides vanish. Uniqueness from the energy estimate makes every $R_{ij}u$ zero. At each point of a sphere the rotation fields span its tangent plane, so all tangential [derivatives](../../../../../../derivative.md) of $u$ vanish. Each sphere is connected, giving $\boxed{u(x)=U(|x|)}$. This proves radiality without assuming it as a separation-of-variables ansatz.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
