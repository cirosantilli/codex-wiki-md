<h1 id="section-b/b6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Find the potential from $\mathbf E=-\nabla\phi$ and $\nabla\cdot(\epsilon\nabla\phi)=-\rho_f$. One must specify boundary data: a potential on each Dirichlet boundary, a normal displacement on each Neumann boundary, or an appropriate mixture. Conductors are equipotentials; at [dielectric](../../../../../../dielectric.md) interfaces $\phi$ is continuous and the normal displacement jumps by the specified free surface charge. With no singular dipole sheet, tangential [electric field](../../../../../../electric-field-split.md) is continuous.

To establish [uniqueness of Poisson equation](../../../../../../uniqueness-of-poisson-equation.md), subtract two solutions with the same charge and boundary data, writing their difference as $u$. [Integration by parts](../../../../../../integration-by-parts.md) gives

$$
\int_V\epsilon|\nabla u|^2\,dV
=\int_{\partial V}u\epsilon\partial_nu\,dA,
$$

since $\nabla\cdot(\epsilon\nabla u)=0$. The right side vanishes for identical Dirichlet data, identical Neumann data, or their usual mixed combination. Interface terms cancel under the homogeneous difference conditions. With positive [permittivity](../../../../../../permittivity-split.md), $\nabla u=0$: **the field is unique**, and the potential is unique if any suitable reference potential is fixed. For a pure Neumann problem an additive constant remains, and the prescribed outward displacement flux must equal the enclosed free charge. This theorem justifies image-charge solutions once their boundary data have been checked.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
