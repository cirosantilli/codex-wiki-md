<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

$S=e/e_s^l$ is the ambient [saturation ratio](../../../../saturation-ratio.md) over a flat liquid-[water](../../../../water.md) surface; $S-1$ is the liquid [atmospheric supersaturation](../../../../atmospheric-supersaturation.md). Curvature increases the surface equilibrium vapour [pressure](../../../../pressure-split.md), producing the [Kelvin penalty](../../../../kelvin-equation.md) $A/r$, while dissolved solute lowers it and gives the opposing [Raoult contribution](../../../../raoult-s-law.md) $B/r^3$. Thus the dilute Köhler equilibrium curve is $S_{\rm eq}-1=A/r-B/r^3$, and the numerator is the [atmospheric supersaturation](../../../../atmospheric-supersaturation.md) available to drive growth beyond surface equilibrium.

$F_d^l$ describes the resistance of vapour [diffusion](../../../../diffusion.md) through the surrounding air. $F_k^l$ describes the [thermal-conduction](../../../../thermal-conduction.md) resistance to removing [latent heat](../../../../latent-heat.md) released by [condensation](../../../../condensation.md): a warmed droplet surface has a higher equilibrium vapour [pressure](../../../../pressure-split.md) and hence a weaker [mass](../../../../mass.md)-transfer drive. Common [continuum approximations](../../../../continuum-approximation.md) are $F_d^l\simeq R_vT/(D_ve_s^l)$ and $F_k^l\simeq L_v[k_{\rm air}T]^{-1}[L_v/(R_vT)-1]$, showing the roles of [diffusivity](../../../../diffusion-coefficient.md), conductivity, [saturation pressure](../../../../vapor-pressure.md) and [latent heat](../../../../latent-heat.md). Both resistances have the supplied units $\mathrm{s\,m\,kg^{-1}}$ and add for this coupled transport problem.

For a spherical droplet of constant [density](../../../../density.md), $m=4\pi\rho r^3/3$. Multiplying the [radius](../../../../radius.md) equation by $4\pi\rho r$ gives

$$
\frac{dm}{dt}=\frac{4\pi r}{F_k^l+F_d^l}
\left[(S-1)-\frac Ar+\frac B{r^3}\right].
$$

At sufficiently large [radius](../../../../radius.md), curvature and solute corrections are negligible, so

$$
\boxed{\frac{dm}{dt}\simeq4\pi r\frac{S-1}{F_k^l+F_d^l}.}
$$

This limit also requires sustained positive [atmospheric supersaturation](../../../../atmospheric-supersaturation.md). It need not describe the earliest submicrometre stage or an unactivated haze particle.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
