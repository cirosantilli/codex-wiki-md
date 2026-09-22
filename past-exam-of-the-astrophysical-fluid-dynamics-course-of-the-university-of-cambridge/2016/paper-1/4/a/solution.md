<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the polytropic law as $p=K\rho^{1+1/n}$, with constant $K$ and $n>0$. Its [pressure](../../../../../pressure-split.md) potential, or [polytropic enthalpy](../../../../../polytropic-enthalpy.md) relative to zero density, is

$$
H(\rho)=\int_0^\rho\frac1{\widetilde\rho}\frac{dp}{d\widetilde\rho}\,d\widetilde\rho=(n+1)K\rho^{1/n}.
$$

Hydrostatic balance is $dH/dr=-d\psi/dr$. If the surface has zero density and potential $\psi_0$, integration gives $H=\psi_0-\psi$. At the centre, $\Delta\psi\equiv\psi_0-\psi_c=(n+1)K\rho_c^{1/n}>0$. Therefore

$$
\theta=\frac H{\Delta\psi}=\left(\frac\rho{\rho_c}\right)^{1/n},\qquad r=\alpha\xi,\qquad\alpha^2=\frac{\Delta\psi}{4\pi G\rho_c}.
$$

Insert $\psi=\psi_0-\Delta\psi\theta$ and $\rho=\rho_c\theta^n$ into the spherical [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md):

$$
\frac1{r^2}\frac d{dr}\left(r^2\frac{d\psi}{dr}\right)=4\pi G\rho\quad\Longrightarrow\quad\boxed{\frac1{\xi^2}\frac d{d\xi}\left(\xi^2\frac{d\theta}{d\xi}\right)=-\theta^n}.
$$

The central conditions are $\theta(0)=1$ and $\theta'(0)=0$; the latter follows from a regular spherically symmetric centre. This reproduces the supplied coordinate and potential scaling rather than introducing an unrelated normalization.

For the sound-speed task, the [adiabatic sound speed](../../../../../adiabatic-sound-speed.md) of a perfect polytropic gas is

$$
c_s^2=\frac{dp}{d\rho}=\gamma K\rho^{\gamma-1}=(\gamma-1)H=(\gamma-1)(\psi_0-\psi),\qquad n=\frac1{\gamma-1}.
$$

A [diatomic gas](../../../../../diatomic-gas.md) with active rotational but frozen vibrational degrees of freedom has $\gamma=7/5$ and $n=5/2$. With the requested surface-potential gauge $\psi_0=0$,

$$
\boxed{c_s=\sqrt{-\frac25\psi}}.
$$

The interior potential is then negative. Choosing zero potential at the surface is legitimate; for a finite isolated sphere it is a different additive gauge from setting potential to zero at infinity. Both choices cannot generally be imposed simultaneously.

For the mass-radius task, let $\xi_1$ be the first zero of the regular [Lane-Emden function](../../../../../lane-emden-function.md) and $Y_n=-\xi_1^2\theta'(\xi_1)$. A finite-radius [polytrope](../../../../../polytrope.md) has

$$
R=\alpha\xi_1,\qquad M=4\pi\alpha^3\rho_cY_n,\qquad\frac{GM}{R}=\Delta\psi\frac{Y_n}{\xi_1}=(n+1)\frac{Y_n}{\xi_1}\frac{R^*T_c}{\mu}.
$$

Thus

$$
\boxed{M=\frac{(n+1)Y_n}{\xi_1}\frac{R^*T_c}{G\mu}\,R}.
$$

**At fixed central [temperature](../../../../../temperature-split.md), fixed composition and fixed [polytropic index](../../../../../polytropic-index.md), $M\propto R$.** These are [homologous polytropes at fixed central temperature](../../../../../homologous-polytropes-at-fixed-central-temperature.md). They do not in general have constant $K$; imposing constant [entropy](../../../../../entropy-split.md) instead gives a different polytropic mass-radius sequence. If $n$ or $\mu$ varies between stars, the displayed dimensionless structure factor and composition factor must be retained: equal $T_c$ alone is not a universal exact proportionality for arbitrary stellar models.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [4](../../4.md)
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
