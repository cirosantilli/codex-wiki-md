<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a [barotropic fluid](../../../../barotropic-fluid.md), define $h(\rho)=\int dp/\rho$. Dotting the steady [Euler equation](../../../../euler-equations-for-an-inviscid-fluid-split.md) with $\mathbf u$ gives

$$
\mathbf u\cdot\nabla\left(\frac{u^2}{2}+h+\psi\right)=0.
$$

Thus the [Bernoulli function](../../../../bernoulli-function.md) $H=u^2/2+h+\psi$ is constant along each [streamline](../../../../streamline.md). Different streamlines can have different constants; steady flow alone does not imply one spatially uniform $H$.

In a [quasi-one-dimensional flow](../../../../quasi-one-dimensional-flow.md) through area $A(z)$ with negligible [gravity](../../../../gravity.md), the axial [momentum](../../../../momentum-split.md) equation and $dp=c_s^2d\rho$ give

$$
u\frac{du}{dz}=-\frac{c_s^2}{\rho}\frac{d\rho}{dz},\qquad
u^2\frac{d\ln u}{dz}=-c_s^2\frac{d\ln\rho}{dz}.
$$

Meanwhile the [mass flow rate](../../../../mass-flow-rate.md) $\dot M=\rho uA$ is constant, so $d\ln\rho=-d\ln u-d\ln A$. Substitution proves the [nozzle area-velocity relation](../../../../nozzle-area-velocity-relation.md)

$$
\boxed{(u^2-c_s^2)\,d\ln u=c_s^2\,d\ln A.}
$$

A [subsonic flow](../../../../subsonic-flow.md) accelerates where $A$ decreases, whereas a [supersonic flow](../../../../supersonic-flow.md) accelerates where $A$ increases. A smooth accelerating [transonic branch](../../../../transonic-branch.md) in a [de Laval nozzle](../../../../de-laval-nozzle.md) therefore crosses $u=c_s$ at a minimum-area throat. Suitable reservoir and downstream [pressures](../../../../pressure-split.md) are also required: a converging-diverging shape by itself does not exclude a wholly subsonic solution or a downstream [shock](../../../../shock-wave.md).

<a id="3/image-choked-adiabatic-nozzle-minimum-area-sonic-crossing-and-continued-supersonic-acceleration"></a>
![](../../../../past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2013/paper-1-de-laval-nozzle.png)

**[Figure 3](#3/image-choked-adiabatic-nozzle-minimum-area-sonic-crossing-and-continued-supersonic-acceleration). Choked adiabatic nozzle: minimum area, sonic crossing and continued supersonic acceleration**.

For the stipulated constant-$K$ [polytropic flow](../../../../polytropic-flow.md), $c_s^2=\gamma K\rho^{\gamma-1}$. At the throat $u_m=c_{s,m}$, so

$$
\dot M=A_m\rho_m\sqrt{\gamma K\rho_m^{\gamma-1}},\qquad
\boxed{\rho_m=\left(\frac{\dot M}{A_m\sqrt{\gamma K}}\right)^{2/(\gamma+1)}.}
$$

The [specific enthalpy](../../../../specific-enthalpy.md) is $h=\gamma K\rho^{\gamma-1}/(\gamma-1)=c_s^2/(\gamma-1)$. Evaluating $H$ at the throat and substituting $\rho=\dot M/(Au)$ elsewhere gives

$$
\boxed{\frac{u^2}{2}+\frac{\gamma K}{\gamma-1}\left(\frac{\dot M}{Au}\right)^{\gamma-1}
=\frac{\gamma+1}{2(\gamma-1)}c_{s,m}^2.}
$$

On the outward supersonic branch, $A\sim Cr^2$ lets the gas expand and its [specific enthalpy](../../../../specific-enthalpy.md) tend to zero for $\gamma>1$. Consequently

$$
\boxed{u_\infty=\sqrt{\frac{\gamma+1}{\gamma-1}}\,c_{s,m},\qquad
\rho\sim\frac{\dot M}{Cu_\infty}\,r^{-2}.}
$$

For $\gamma=5/3$, $u_\infty=2c_{s,m}$. Also $T\propto\rho^{\gamma-1}\propto r^{-2(\gamma-1)}$. These are the [adiabatic nozzle terminal speed](../../../../adiabatic-nozzle-terminal-speed.md) and expansion laws for a lossless escaping branch; a subsonic branch could instead approach finite [pressure](../../../../pressure-split.md) with $u\propto A^{-1}$. A pressure-shaped [astrophysical jet](../../../../astrophysical-jet.md) is being approximated by a nozzle here: the assumed geometry does not by itself explain the confinement or account for magnetic [forces](../../../../force-split.md) or relativistic motion in an actual [active galactic nucleus](../../../../active-galactic-nucleus.md).

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
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
