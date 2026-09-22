<h1 id="section-b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the background [mass density](../../../../../density.md) as $\bar\rho(z)=\rho_0+\rho'_0z$ and its [hydrostatic pressure](../../../../../hydrostatic-pressure.md) as $\bar p(z)$, where

$$
\bar p'(z)=-g\bar\rho(z),\qquad
\bar p(z)=p_* -g\rho_0z-\frac12g\rho'_0z^2.
$$

Apply an [Eulerian perturbation of a fluid variable](../../../../../eulerian-perturbation-of-a-fluid-variable.md) to the background fields:

$$
\rho_{\rm tot}=\bar\rho+\varrho,\qquad p_{\rm tot}=\bar p+\pi.
$$

Thus $\pi$ is the Eulerian [pressure](../../../../../pressure-split.md) perturbation, in pascals; it is not the background [hydrostatic pressure](../../../../../hydrostatic-pressure.md).

For [incompressible flow](../../../../../incompressible-flow.md), [mass conservation](../../../../../mass-conservation.md) becomes $D\rho_{\rm tot}/Dt=0$. Linearizing about rest gives

$$
\partial_t\varrho=-u_z\rho'_0.
$$

The [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid-split.md) are $\rho_{\rm tot}D\mathbf u/Dt=-\nabla p_{\rm tot}-\rho_{\rm tot}g\widehat{\mathbf z}$. The background [pressure gradient](../../../../../pressure-gradient.md) and weight cancel. Dropping products of perturbations gives

$$
\bar\rho\,\partial_t\mathbf u=-\nabla\pi-\varrho g\widehat{\mathbf z}.
$$

Under $|\rho'_0z|\ll\rho_0$, replace $\bar\rho$ by $\rho_0$ in inertia but retain the background [mass density](../../../../../density.md) gradient in the displacement-induced [buoyancy](../../../../../buoyancy.md). This is the [Boussinesq approximation](../../../../../boussinesq-approximation.md). Its linear [Boussinesq equations](../../../../../boussinesq-equations.md) here are

$$
\boxed{\begin{aligned}
\partial_xu_x+\partial_zu_z&=0,\\
\rho_0\partial_tu_x&=-\partial_x\pi,\\
\rho_0\partial_tu_z&=-\partial_z\pi-g\varrho,\\
\partial_t\varrho&=-\rho'_0u_z.
\end{aligned}}
$$

The absolute value makes explicit that the small-density-variation condition concerns magnitude, including the usual negative $\rho'_0$ of stable [density stratification](../../../../../density-stratification.md).

## ↑ Ancestors (14)

1. [B](../b.md)
2. [4](../../4.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../../split.md)
6. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
