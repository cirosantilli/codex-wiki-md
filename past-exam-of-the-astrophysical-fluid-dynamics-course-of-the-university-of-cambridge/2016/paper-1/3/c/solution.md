<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the idealized fully developed, laminar cylindrical-flow model implied by the fixed cross-section and zero [velocity](../../../../../velocity.md) at its sides. Take the jet length to be $R$, as for a central source reaching the cloud boundary; if the source is off-centre, the actual path length must replace $R$. Let $s$ denote distance from the jet axis and write the axial [velocity](../../../../../velocity.md) as $u(s)$. Then $(\mathbf u\cdot\nabla)\mathbf u=0$, the [pressure gradient](../../../../../pressure-gradient.md) is $dp/dz=-p_0/R$, and the axial [Navier-Stokes equation](../../../../../navier-stokes-equation.md) reduces to

$$
0=\frac{p_0}{R}+\rho\nu\frac1s\frac d{ds}\left(s\frac{du}{ds}\right).
$$

Regularity at $s=0$ excludes a logarithmic term. The imposed [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) $u(r_0)=0$ gives the [Hagen-Poiseuille flow](../../../../../hagen-poiseuille-equation.md) profile

$$
u(s)=\frac{p_0}{4\rho\nu R}(r_0^2-s^2)=U_{\max}\left(1-\frac{s^2}{r_0^2}\right),\qquad U_{\max}=\frac{p_0r_0^2}{4\rho\nu R}.
$$

The [kinetic energy](../../../../../kinetic-energy.md) crossing each area element per unit time is $(\rho u^2/2)u\,dA$, so the [velocity](../../../../../velocity.md) must be cubed before integration. Thus

$$
P=\frac12\rho\int u^3\,dA=\pi\rho U_{\max}^3\int_0^{r_0}\left(1-\frac{s^2}{r_0^2}\right)^3s\,ds=\frac{\pi\rho U_{\max}^3r_0^2}{8}.
$$

Consequently

$$
\boxed{P=\frac{\pi p_0^3}{512\rho^2\nu^3R^3}\,r_0^8,\qquad A=\frac{\pi p_0^3}{512\rho^2\nu^3R^3}}.
$$

The [mean velocity](../../../../../mean-velocity-of-a-kinetic-distribution.md) is $\bar u=U_{\max}/2$. Replacing the profile by $\bar u$ in $\tfrac12\rho\pi r_0^2\bar u^3$ underestimates the flux by two; the [kinetic energy correction factor](../../../../../kinetic-energy-correction-factor.md) is two for this profile. The radius dependence follows from $u\propto r_0^2$ and cross-sectional area $\propto r_0^2$.

The specified $P$ is outgoing bulk kinetic-energy flux, not the pressure-work rate $p_0Q$, which scales as $r_0^4$. In a fully developed section the profile is independent of $z$ and [pressure](../../../../../pressure-split.md) work is dissipated as heat; entrance acceleration and [energy](../../../../../energy-split.md) supply establish the profile. A turbulent or freely entraining astrophysical jet need not have this no-slip parabolic structure. The model assumes a long enough, laminar confined region and neglects entrance losses and [gravity](../../../../../gravity.md).

<a id="3/c/image-parabolic-hagen-poiseuille-flow-and-its-cubic-velocity-weighting-in-kinetic-energy-flux"></a>
![](../../../../../past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2016/paper-1-jet-profile.png)

**[Figure 3](#3/c/image-parabolic-hagen-poiseuille-flow-and-its-cubic-velocity-weighting-in-kinetic-energy-flux). Parabolic Hagen-Poiseuille flow and its cubic velocity weighting in kinetic-energy flux**.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
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
