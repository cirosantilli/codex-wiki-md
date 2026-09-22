<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an [axisymmetric vector field](../../../../../../axisymmetric-vector-field.md), write $\mathbf B=B_R\mathbf e_R+B_\phi\mathbf e_\phi+B_z\mathbf e_z$. Pure [differential rotation](../../../../../../differential-rotation.md) gives

$$
\mathbf u\times\mathbf B=R\Omega B_z\mathbf e_R-R\Omega B_R\mathbf e_z.
$$

This vector has no azimuthal component and is independent of $\phi$, so its [curl](../../../../../../curl.md) has zero radial and vertical components. Its azimuthal component is

$$
\{\nabla\times(\mathbf u\times\mathbf B)\}_\phi=\partial_z(R\Omega B_z)+\partial_R(R\Omega B_R)
=R(B_z\partial_z\Omega+B_R\partial_R\Omega)+\Omega\{R\partial_zB_z+\partial_R(RB_R)\}.
$$

The final braces are $R\nabla\cdot\mathbf B=0$ by [Gauss's law for magnetism](../../../../../../gauss-s-law-for-magnetism.md). The [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) therefore yields [axisymmetric magnetic winding](../../../../../../axisymmetric-magnetic-winding.md):

$$
\boxed{\partial_t\mathbf B=R(\mathbf B_p\cdot\nabla\Omega)\mathbf e_\phi,\qquad\partial_t\mathbf B_p=0.}
$$

[Differential rotation](../../../../../../differential-rotation.md) creates a [toroidal magnetic field](../../../../../../toroidal-magnetic-field.md) from the fixed [poloidal magnetic field](../../../../../../poloidal-magnetic-field.md). A stationary field under the same purely rotational assumptions requires [Ferraro's law of isorotation](../../../../../../ferraro-s-law-of-isorotation.md), $\mathbf B_p\cdot\nabla\Omega=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
