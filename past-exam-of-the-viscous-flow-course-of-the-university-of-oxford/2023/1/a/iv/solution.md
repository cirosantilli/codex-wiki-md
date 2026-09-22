<h1 id="1/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For an isotropic [Newtonian fluid](../../../../../newtonian-fluid.md) in [incompressible flow](../../../../../incompressible-flow.md), the [constitutive equation](../../../../../constitutive-equation.md) is

$$
\boxed{\sigma_{ij}=-p\delta_{ij}+2\mu E_{ij},
\qquad E_{ij}=\frac12(\partial_j u_i+\partial_i u_j).}
$$

Here $p$ is [pressure](../../../../../pressure-split.md), $\delta_{ij}$ is the [Kronecker delta](../../../../../kronecker-delta.md), $\mu$ is the constant [dynamic viscosity](../../../../../dynamic-viscosity-split.md), and $E$ is the [strain-rate tensor](../../../../../strain-rate-tensor.md). The more general compressible [constitutive equation](../../../../../constitutive-equation.md) can include a term proportional to $(\nabla\cdot\mathbf u)\delta_{ij}$; that term vanishes here.

Differentiate the [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md), retaining the constant [dynamic viscosity](../../../../../dynamic-viscosity-split.md) outside the [derivatives](../../../../../derivative.md):

$$
\partial_j\sigma_{ij}
=-\partial_i p+\mu\partial_j\partial_j u_i
+\mu\partial_i(\partial_j u_j)
=-\partial_i p+\mu\nabla^2u_i.
$$

The last equality uses [incompressibility](../../../../../incompressible-flow.md). Substitution into the [Cauchy momentum equation](../../../../../cauchy-momentum-equation.md) gives the [Navier-Stokes equation](../../../../../navier-stokes-equation.md)

$$
\boxed{\rho\left(\frac{\partial\mathbf u}{\partial t}
+(\mathbf u\cdot\nabla)\mathbf u\right)
=-\nabla p+\mu\nabla^2\mathbf u.}
$$

The [pressure gradient](../../../../../pressure-gradient.md) and the [Laplacian](../../../../../laplacian.md) of the [velocity field](../../../../../velocity-field.md) therefore give the two contact [force](../../../../../force-split.md) densities in this model.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the viscous flow course of the University of Oxford](../../../../split.md)
6. [Viscous flow course of the University of Oxford](../../../../../viscous-flow-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
