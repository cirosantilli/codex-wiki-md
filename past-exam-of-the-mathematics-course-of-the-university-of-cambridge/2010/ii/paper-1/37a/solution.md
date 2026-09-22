<h1 id="37a/solution">Solution</h1>

↑ **Parent:** [37A](../37a.md)

For a constant-density incompressible fluid, the [Navier-Stokes equation](../../../../../navier-stokes-equation.md) and incompressibility constraint are

$$
\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u
=-\rho^{-1}\nabla p+\nu\nabla^2\mathbf u,\qquad\nabla\cdot\mathbf u=0.
$$

Scale length by $L_*$, velocity by $U_*$, time by $L_*/U_*$ and pressure by $\rho U_*^2$. In dimensionless variables they become

$$
\partial_{t'}\mathbf u'+(\mathbf u'\cdot\nabla')\mathbf u'
=-\nabla'p'+\operatorname{Re}^{-1}\nabla'^2\mathbf u',\quad
\operatorname{Re}=U_*L_*/\nu.
$$

A [rectilinear flow](../../../../../rectilinear-flow.md) has velocity $\mathbf u=U(y,z)\widehat x$, parallel everywhere to one fixed direction and independent of that direction. Its convective acceleration is identically zero. A steady such flow therefore satisfies the linear equation $\nu\Delta_\perp U=\rho^{-1}dp/dx$, with no inertial term and no Reynolds-dependent change of equation or spatial shape for fixed scaled boundary/forcing data. Relative changes in imposed pressure forcing can of course change the profile; Reynolds independence is not independence of the boundary data.

## ↑ Ancestors (10)

1. [37A](../37a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
