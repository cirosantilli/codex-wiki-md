<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Treat the gas as a smooth [quasi-one-dimensional flow](../../../../../quasi-one-dimensional-flow.md) through a rigid passage, neglecting axial body forces and heat input. It is the confining medium that is incompressible; the flowing gas must remain compressible. With area $\mathcal A(x)$ and axial speed $u$, continuity and inviscid momentum balance give

$$
\rho u\mathcal A=\dot M,\qquad u\,du=-\frac{dp}{\rho},\qquad dp=c_s^2\,d\rho.
$$

Combining their logarithmic differentials yields the [nozzle area-velocity relation](../../../../../nozzle-area-velocity-relation.md)

$$
\frac{d\mathcal A}{\mathcal A}=(\mathcal M^2-1)\frac{du}{u},\qquad\mathcal M=\frac u{c_s}.
$$

A smooth crossing of $\mathcal M=1$ requires an area extremum. The given radius is positive and has derivative $r'(x)=16r_0x\exp[-16x^2/L^2]/L^2$, which vanishes only at $x=0$ within the slab and changes from negative to positive there. Thus this station is the unique throat, with $r_s=r_0/2$ and $\mathcal A_s=\pi r_0^2/4$. The specified subsonic inlet and supersonic outlet select the smooth accelerating branch, so

$$
\boxed{x_s=0}.
$$

A throat by itself does not guarantee transonic flow for arbitrary reservoir and back [pressures](../../../../../pressure-split.md); that branch is specified here. Before the throat a converging section accelerates [subsonic flow](../../../../../subsonic-flow.md); beyond it a diverging section accelerates [supersonic flow](../../../../../supersonic-flow.md).[Supersonic and Subsonic Flow, continuity/momentum derivation of the area-velocity relation and choked throat](../../../../../nozzle-design-by-nasa-glenn-research-center.md)

For the [temperature](../../../../../temperature-split.md) task, evaluate the [mass](../../../../../mass.md) flux and [sound speed](../../../../../speed-of-sound.md) at the throat using $p=K\rho^\gamma$:

$$
\dot M=\mathcal A_s\rho_sc_s=\mathcal A_s\sqrt{\gamma K}\,\rho_s^{(\gamma+1)/2},\qquad\rho_s=\left(\frac{\dot M}{\mathcal A_s\sqrt{\gamma K}}\right)^{2/(\gamma+1)}.
$$

The ideal-gas relation then gives

$$
\boxed{T_{x_s}=\frac{\mu K}{R^*}\left(\frac{4\dot M}{\pi r_0^2\sqrt{\gamma K}}\right)^{2(\gamma-1)/(\gamma+1)}}.
$$

This expresses the sonic [temperature](../../../../../temperature-split.md) in terms of the [entropy](../../../../../entropy-split.md) constant, geometry, [mass](../../../../../mass.md) flux and composition; no numerical value of $K$ or $\dot M$ is provided. Equivalently $c_s^{\gamma+1}=\gamma K(\dot M/\mathcal A_s)^{\gamma-1}$ and $T_s=\mu c_s^2/(\gamma R^*)$. The slab length drops out because the sonic thermodynamic state depends on the minimum area, not on the axial distance over which a lossless smooth [nozzle](../../../../../nozzle.md) contracts. As a check, conserved stagnation enthalpy gives $T_s=2T_{\rm stag}/(\gamma+1)$.[equations 1–10 and 19, sonic mass-flow maximum and temperature/Mach relation](../../../../../mass-flow-choking-by-nasa-glenn-research-center.md)

The result assumes cross-sectional thermodynamic uniformity and negligible transverse [kinetic energy](../../../../../kinetic-energy.md). Exact multidimensional flow through a sharply varying passage can have a curved sonic surface; the radius profile alone does not solve that boundary-value problem. The original numerical plot below computes the standard quasi-one-dimensional branch, rather than reproducing the supplied passage sketch.

<a id="4/b/image-calculated-area-mach-number-and-temperature-along-the-smooth-transonic-nozzle-branch"></a>
![](../../../../../past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2016/paper-1-transonic-flow.png)

**[Figure 4](#4/b/image-calculated-area-mach-number-and-temperature-along-the-smooth-transonic-nozzle-branch). Calculated area, Mach number and temperature along the smooth transonic nozzle branch**.

## ↑ Ancestors (14)

1. [B](../b.md)
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
