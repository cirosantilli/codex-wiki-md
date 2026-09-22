<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the proposed [velocity field](../../../../velocity-field.md), $u_x+w_z=1-1=0$, so [incompressibility](../../../../incompressible-flow.md) holds. Its [convective acceleration](../../../../convective-acceleration.md) is

$$
u u_x+w u_z=x,\qquad u w_x+w w_z=z,
$$

and both components have zero [Laplacian](../../../../laplacian.md). The [Navier-Stokes equation](../../../../navier-stokes-equation.md) therefore requires $p_x=-x$ and $p_z=-z$. Hence

$$
\boxed{p(x,z)=p_* -\frac12(x^2+z^2),}
$$

where $p_*$ is an arbitrary constant reference [pressure](../../../../pressure-split.md). The same [pressure gradient](../../../../pressure-gradient.md) balances the same [convective acceleration](../../../../convective-acceleration.md) in the [Euler equations for an inviscid fluid](../../../../euler-equations-for-an-inviscid-fluid-split.md). Since the viscous terms vanish identically, this is an exact solution for every positive [Reynolds number](../../../../reynolds-number.md), as well as for the inviscid limit.

At $z=0$, the normal [velocity](../../../../velocity.md) is zero, and the prescribed dimensionless tangential [traction](../../../../traction.md) is

$$
\boxed{\mathbf e_1\cdot\mathbf t(\mathbf e_3)=u_z+w_x=0.}
$$

This [stagnation point](../../../../stagnation-point.md) flow therefore has **zero surface shear stress**, although its [strain-rate tensor](../../../../strain-rate-tensor.md) and its viscous [normal stresses](../../../../normal-stress.md) are nonzero.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the viscous flow course of the University of Oxford](../../../split.md)
5. [Viscous flow course of the University of Oxford](../../../../viscous-flow-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
