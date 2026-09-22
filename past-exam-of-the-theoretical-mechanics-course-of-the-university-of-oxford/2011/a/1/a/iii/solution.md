<h1 id="a/1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Insert the [traction](../../../../../../traction.md) formula into the material-[volume](../../../../../../volume.md) balance and apply the [divergence theorem](../../../../../../divergence-theorem.md) to each row of the [stress tensor](../../../../../../cauchy-stress-tensor.md):

$$
\int_{V(t)}\rho\frac{Du_i}{Dt}\,dV=\int_{\partial V(t)}\sigma_{ij}n_j\,dS=\int_{V(t)}\partial_j\sigma_{ij}\,dV.
$$

The [volume](../../../../../../volume.md) is arbitrary, so continuity of the fields gives the local [Cauchy momentum equation](../../../../../../cauchy-momentum-equation.md)

$$
\boxed{\rho\frac{D\mathbf u}{Dt}=\mathbf e_i\frac{\partial\sigma_{ij}}{\partial x_j}.}
$$

For an incompressible [Newtonian fluid](../../../../../../newtonian-fluid.md), the constitutive law is

$$
\boxed{\sigma_{ij}=-p\delta_{ij}+\mu(\partial_ju_i+\partial_iu_j).}
$$

Here the [pressure](../../../../../../pressure-split.md) enforces [incompressibility](../../../../../../incompressible-flow.md), and the viscous stress is twice the [viscosity](../../../../../../dynamic-viscosity-split.md) times the symmetric rate-of-strain [tensor](../../../../../../tensor.md). With constant $\mu$,

$$
\partial_j\sigma_{ij}=-\partial_ip+\mu\nabla^2u_i+\mu\partial_i(\partial_ju_j)=-\partial_ip+\mu\nabla^2u_i.
$$

Using $D/Dt=\partial_t+\mathbf u\cdot\nabla$ proves the stated [Navier-Stokes equations](../../../../../../navier-stokes-equation.md).

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../../split.md)
7. [Theoretical mechanics course of the University of Oxford](../../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
