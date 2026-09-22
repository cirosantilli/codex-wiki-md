<h1 id="39c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Navier-Stokes equation](../../../../../../navier-stokes-equation.md) for constant [mass density](../../../../../../density.md) $\rho$, [dynamic viscosity](../../../../../../dynamic-viscosity.md) $\mu$, and [body force](../../../../../../body-force.md) per unit mass $\mathbf f$ is

$$
\rho\left(\partial_t\mathbf u+\mathbf u\mathbin{\cdot}\nabla\mathbf u\right)
=\nabla\mathbin{\cdot}\boldsymbol\sigma+\rho\mathbf f,
\qquad
\nabla\mathbin{\cdot}\mathbf u=0,
$$

where the [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md) is

$$
\boldsymbol\sigma=-p\mathbf I+2\mu\mathbf e,
\qquad
\mathbf e=\frac12\left(\nabla\mathbf u+(\nabla\mathbf u)^T\right).
$$

Taking the [dot product](../../../../../../inner-product.md) with $\mathbf u$ gives

$$
\rho\mathbf u\mathbin{\cdot}
\left(\partial_t\mathbf u+\mathbf u\mathbin{\cdot}\nabla\mathbf u\right)
=\nabla\mathbin{\cdot}(\boldsymbol\sigma\mathbf u)
-\boldsymbol\sigma:\nabla\mathbf u
+\rho\mathbf f\mathbin{\cdot}\mathbf u.
$$

Incompressibility implies

$$
\boldsymbol\sigma:\nabla\mathbf u=2\mu\mathbf e:\mathbf e,
$$

and converts the left side into a local time derivative plus the divergence of kinetic-energy flux. The [divergence theorem](../../../../../../divergence-theorem.md) therefore gives the [kinetic-energy balance for an incompressible Newtonian fluid](../../../../../../kinetic-energy-balance-for-an-incompressible-newtonian-fluid.md)

$$
\boxed{
\begin{aligned}
\frac d{dt}\int_\Omega\frac12\rho|\mathbf u|^2\,dV
={}&-\int_{\partial\Omega}\frac12\rho|\mathbf u|^2
\mathbf u\mathbin{\cdot}\mathbf n\,dS\\
&+\int_{\partial\Omega}
\mathbf u\mathbin{\cdot}\boldsymbol\sigma\mathbf n\,dS
+\int_\Omega\rho\mathbf f\mathbin{\cdot}\mathbf u\,dV
-2\mu\int_\Omega\mathbf e:\mathbf e\,dV.
\end{aligned}}
$$

The four terms are respectively outward advective transport of kinetic energy, mechanical power supplied by surface traction, power supplied by the body force, and irreversible viscous dissipation into heat.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [39C](../../39c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
