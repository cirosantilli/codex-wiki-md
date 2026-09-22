<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The original PDF has **absolute-value bars around both gradients**; they are missing from the transcription. The stability argument must respect the sign of the upward coordinate.

Displace a small parcel upward by $\xi$. Assume it remains in [pressure equilibrium](../../../../pressure-equilibrium.md) with its surroundings but exchanges negligible heat, so it follows an [adiabatic process](../../../../adiabatic-process.md). For a perfect gas with [adiabatic index](../../../../heat-capacity-ratio.md) $\gamma$, $T\propto p^{(\gamma-1)/\gamma}$ along that parcel's adiabat. Its [temperature](../../../../temperature-split.md) gradient is therefore

$$
T'_{\rm ad}=\frac{\gamma-1}{\gamma}\frac Tp\frac{dp}{dz}
=-\frac{g}{c_p},\qquad c_p=\frac{\gamma\mathcal R}{\gamma-1}.
$$

The last step uses [hydrostatic equilibrium](../../../../hydrostatic-equilibrium.md), and $c_p$ is the [specific heat capacity at constant pressure](../../../../specific-heat-capacity-at-constant-pressure.md). At its new height, the [temperature](../../../../temperature-split.md) difference between the parcel and the environment is $(T'_{\rm ad}-T')\xi$. At equal [pressure](../../../../pressure-split.md), its relative density excess is the negative of its relative [temperature](../../../../temperature-split.md) excess. The upward [buoyancy](../../../../buoyancy.md) acceleration is thus

$$
\ddot\xi=\frac gT(T'_{\rm ad}-T')\xi=-N^2\xi,\qquad
N^2=\frac gT\left(\frac{dT}{dz}+\frac g{c_p}\right).
$$

This is the squared [Brunt–Väisälä frequency](../../../../buoyancy-frequency.md). [Convective stability](../../../../convective-stability.md) requires $N^2>0$, or, in signed-gradient form,

$$
\boxed{\frac{dT}{dz}>\left(1-\frac1\gamma\right)\frac Tp\frac{dp}{dz}=-\frac g{c_p}.}
$$

For a [temperature](../../../../temperature-split.md) decreasing upward, this is exactly the PDF's [Schwarzschild criterion](../../../../schwarzschild-criterion.md)

$$
\boxed{\left|\frac{dT}{dz}\right|<\left(1-\frac1\gamma\right)\frac Tp
\left|\frac{dp}{dz}\right|.}
$$

The absolute-value condition is also sufficient more generally, although a sufficiently steep [temperature](../../../../temperature-split.md) inversion remains stable even when that stronger condition fails. Reversing the signed inequality, as the bar-free transcription does, would instead describe an unstable [temperature](../../../../temperature-split.md) decrease.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
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
