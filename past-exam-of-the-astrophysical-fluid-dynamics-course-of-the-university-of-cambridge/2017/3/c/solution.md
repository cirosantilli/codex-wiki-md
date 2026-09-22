<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $a_T^2=k_BT/(\mu m_u)$ be the constant [isothermal sound speed](../../../../isothermal-sound-speed.md) squared. The stationary galactic gas obeys [hydrostatic equilibrium](../../../../hydrostatic-equilibrium.md) in the specified [gravitational potential](../../../../newtonian-potential-of-a-point-mass.md):

$$
a_T^2\frac{d\rho}{dr}=-\rho\frac{d\psi}{dr},\qquad
\frac{d\ln\rho}{dr}=-\frac{1}{a_T^2}\frac{d\psi}{dr}.
$$

Integrating from the pressure-matching radius $r_0$ gives $\rho(r)=\rho(r_0)\exp[-(\psi(r)-\psi(r_0))/a_T^2]$. Since $\rho(r_0)=p_0/a_T^2$ and $\psi=-Ar^{-1/2}$,

$$
\boxed{\rho(r)=\frac{\mu m_up_0}{k_BT}
\exp\!\left[\frac{A\mu m_u}{k_BT}
\left(r^{-1/2}-r_0^{-1/2}\right)\right],\qquad0<r\leq r_0.}
$$

The exponent is dimensionless: the quantity in parentheses times $A$ is a difference of [gravitational potential](../../../../newtonian-potential-of-a-point-mass.md), of units $\mathrm{m^2\,s^{-2}}$. Density increases inward, as expected. The idealized potential is singular at the centre, so this formal profile should not be extrapolated into a region where the prescribed potential or the neglect of gas self-gravity fails.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../split.md)
5. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
