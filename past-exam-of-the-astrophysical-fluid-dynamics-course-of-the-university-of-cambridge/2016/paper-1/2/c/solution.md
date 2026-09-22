<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A small [pressure](../../../../../pressure-split.md) disturbance propagates because compression raises the [pressure](../../../../../pressure-split.md), the [pressure gradient](../../../../../pressure-gradient.md) accelerates nearby fluid, and the induced convergence compresses the next region. For a uniform fluid at rest, linearizing [mass](../../../../../mass.md) and [momentum conservation](../../../../../momentum-conservation.md) and using the adiabatic pressure-density response gives

$$
\frac{\partial\rho'}{\partial t}+\rho_0\nabla\cdot\mathbf u'=0,\qquad\rho_0\frac{\partial\mathbf u'}{\partial t}=-\nabla p',\qquad p'=c_s^2\rho',\qquad c_s^2=\left(\frac{\partial p}{\partial\rho}\right)_s.
$$

Eliminating $\rho'$ and $\mathbf u'$ gives $\partial_t^2p'=c_s^2\nabla^2p'$. A [plane wave](../../../../../plane-wave.md) has $\omega^2=c_s^2|\mathbf k|^2$ and longitudinal [velocity](../../../../../velocity.md) parallel to $\mathbf k$. In a [perfect gas](../../../../../ideal-gas-split.md),

$$
\boxed{c_s=\sqrt{\gamma p_0/\rho_0}=\sqrt{\gamma(R^*/\mu)T_0}}.
$$

The adiabatic response is appropriate when heat cannot diffuse appreciably out of each compressed region during a period; an isothermal response would give a different derivative. In a moving uniform medium, the acoustic characteristics travel at $U\pm c_s$ along the flow, rather than at $\pm c_s$ in the laboratory.

For a progressive wave, $p'=\rho_0c_su'_\parallel$; [pressure](../../../../../pressure-split.md), density and longitudinal [velocity](../../../../../velocity.md) are in phase. The [acoustic energy density](../../../../../acoustic-energy-density.md) is the sum of kinetic and compression energies,

$$
E_{\rm ac}=\frac12\rho_0|\mathbf u'|^2+\frac{p'^2}{2\rho_0c_s^2},\qquad\langle I\rangle=\frac{p_{\rm rms}^2}{\rho_0c_s}.
$$

**Sound transports [energy](../../../../../energy-split.md) while fluid elements execute small oscillations about their mean positions.** The ideal uniform-fluid acoustic mode is nondispersive. Spherical spreading reduces [pressure](../../../../../pressure-split.md) amplitude as $1/r$ when total power is conserved; [viscosity](../../../../../dynamic-viscosity-split.md) and [heat conduction](../../../../../thermal-conduction.md) attenuate waves, while sufficiently large compressions can steepen into shocks. In a stratified astrophysical gas the uniform result is local: [wavelengths](../../../../../wavelength.md) short compared with background scale heights justify it, whereas long waves can couple to [buoyancy](../../../../../buoyancy.md) and acoustic-cutoff behavior.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [2](../../2.md)
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
