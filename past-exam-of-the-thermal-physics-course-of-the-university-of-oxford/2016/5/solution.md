<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Assume a stationary [temperature](../../../temperature-split.md) profile, spatially uniform [mass density](../../../density.md) and radioactive [heat generation rate](../../../heat-generation-rate.md), constant [thermal conductivity](../../../thermal-conductivity.md), isotropic solid [thermal conduction](../../../thermal-conduction.md), and blackbody emission into effectively cold surroundings. The volumetric source is

$$
q_v=\rho h=4.375\times10^{-7}\,\mathrm{W\,m^{-3}}.
$$

Total radiogenic [power](../../../power.md) equals the surface [blackbody radiation](../../../black-body-radiation.md) loss. The [Stefan–Boltzmann law](../../../stefan-boltzmann-law.md) gives

$$
\frac{4\pi R^3}{3}q_v=4\pi R^2\sigma_{\rm SB}T_S^4,\qquad
\boxed{T_S=\left(\frac{q_vR}{3\sigma_{\rm SB}}\right)^{1/4}=22.52\,\mathrm K.}
$$

For [steady radiogenic heating of a conducting sphere](../../../steady-radiogenic-heating-of-a-conducting-sphere.md), the interior [heat equation](../../../heat-equation.md) is

$$
\frac1{r^2}\frac d{dr}\left(r^2\kappa\frac{dT}{dr}\right)+q_v=0.
$$

Regularity at the centre removes the $1/r^2$ integration term and yields $dT/dr=-q_vr/(3\kappa)$. Matching $T(R)=T_S$ gives

$$
T(r)=T_S+\frac{q_v}{6\kappa}(R^2-r^2),\qquad
\boxed{T_C=T_S+\frac{q_vR^2}{6\kappa}=371.4\,\mathrm K.}
$$

The high central [temperature](../../../temperature-split.md) is compatible with a cold surface because finite [thermal conductivity](../../../thermal-conductivity.md) requires a large [temperature gradient](../../../temperature-gradient.md) to carry the accumulated interior [heat](../../../heat-split.md). A nonzero background radiation temperature $T_{\rm bg}$ replaces $T_S^4$ by $T_S^4-T_{\rm bg}^4$ in the surface balance. The calculation neglects convection, stored transient [heat](../../../heat-split.md), changing radioactive abundances, phase changes and any substantial external irradiation.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2016](../../2016-split.md)
3. [Past exam of the thermal physics course of the University of Oxford](../../split.md)
4. [Thermal physics course of the University of Oxford](../../../thermal-physics-course-of-the-university-of-oxford.md)
5. [Year 2 of the physics course of the University of Oxford](../../../year-2-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
