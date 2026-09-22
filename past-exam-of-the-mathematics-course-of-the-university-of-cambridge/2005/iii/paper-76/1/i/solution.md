<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [resistive induction equation](../../../../../../resistive-induction-equation.md) with constant [magnetic diffusivity](../../../../../../magnetic-diffusivity.md),

$$
\partial_t\mathbf B_{\mathrm{tot}}=\nabla\times(\mathbf u\times\mathbf B_{\mathrm{tot}})+\eta\nabla^2\mathbf B_{\mathrm{tot}},\qquad\nabla\cdot\mathbf B_{\mathrm{tot}}=0.
$$

Seek $\mathbf B_{\mathrm{tot}}=B_0\mathbf e_z+B(s,z,t)\mathbf e_\phi$. The axisymmetric velocity $\mathbf u=s\omega(s,z)\mathbf e_\phi$ is incompressible, and the proposed field is [solenoidal](../../../../../../solenoidal-vector-field.md). The [toroidal magnetic field](../../../../../../toroidal-magnetic-field.md) is parallel to the velocity, so it does not contribute to their [cross product](../../../../../../cross-product.md). The remaining term is

$$
\mathbf u\times\mathbf B_{\mathrm{tot}}=s\omega B_0\mathbf e_s,\qquad\nabla\times(s\omega B_0\mathbf e_s)=sB_0\partial_z\omega\,\mathbf e_\phi.
$$

The uniform axial field has zero vector [Laplacian](../../../../../../laplacian.md). For the azimuthal part, differentiation of the cylindrical basis gives $\partial_\phi^2\mathbf e_\phi=-\mathbf e_\phi$. Consequently

$$
\nabla^2(B\mathbf e_\phi)=\left(\partial_s^2B+\frac1s\partial_sB+\partial_z^2B-\frac B{s^2}\right)\mathbf e_\phi.
$$

There is no source for a radial or axial perturbation, so zero initial values of those components remain zero. Equating the toroidal components proves

$$
\boxed{\partial_tB=s(\mathbf B_0\cdot\nabla)\omega+\eta\left(\nabla^2-\frac1{s^2}\right)B.}
$$

The last Laplacian is the scalar axisymmetric [Laplacian](../../../../../../laplacian.md). The additional $-B/s^2$ term is essential for a vector component in a rotating basis. The source is the [Omega effect](../../../../../../omega-effect.md): rotation that varies along an axial field line winds it into a [toroidal magnetic field](../../../../../../toroidal-magnetic-field.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
