<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the flat two-layer model, with thickness $h=30\,\mathrm{km}$, crustal shear [speed](../../../../../speed.md) $\beta_1=3.5\,\mathrm{km\,s^{-1}}$ and [mantle](../../../../../planetary-mantle.md) [speed](../../../../../speed.md) $\beta_2=4.5\,\mathrm{km\,s^{-1}}$. For [SH-wave travel times in a crustal waveguide](../../../../../sh-wave-travel-times-in-a-crustal-waveguide.md), unfolding each reflected path gives all [reflection](../../../../../reflection-mathematics.md) orders at once:

$$
\boxed{t_D=\frac x{3.5},\qquad
t_m=\frac{\sqrt{x^2+(60m)^2}}{3.5},\quad m=1,2,\ldots,}
$$

with $x$ in kilometres and times in seconds. The direct wave begins at the origin; reflected orders have intercepts $60m/3.5=17.14m\,\mathrm s$ and approach the direct-wave slope at large distance.

The critical angle, measured from the vertical, is $i_c=\arcsin(3.5/4.5)\simeq51.1^\circ$. Associated critical [refraction](../../../../../refraction.md) and its multiples give

$$
\boxed{t_{H,m}=\frac x{4.5}+2mh\sqrt{\beta_1^{-2}-\beta_2^{-2}}
=\frac x{4.5}+10.77m,\qquad
x\geq x_{c,m}=2mh\tan i_c\simeq74.25m\,\mathrm{km}.}
$$

Each head-wave line is tangent to its [reflection](../../../../../reflection-mathematics.md) curve at the critical distance. In particular the primary head wave exists before it becomes the first arrival; it overtakes the direct wave only around $170\,\mathrm{km}$.

The slope of a reflected travel-time curve is $p=dt_m/dx=\sin i/\beta_1$. For $x<x_{c,m}$, $p<1/\beta_2$, so the [mantle](../../../../../planetary-mantle.md) supports outgoing shear radiation and successive reverberations leak [energy](../../../../../energy-split.md). For $x>x_{c,m}$, $1/\beta_2<p<1/\beta_1$: the [mantle](../../../../../planetary-mantle.md) field is evanescent and ideal interface [reflection](../../../../../reflection-mathematics.md) is total. These [leaking and trapped SH-wave reverberations](../../../../../leaking-and-trapped-sh-wave-reverberations.md) explain the annotations in the original travel-time drawing below. A reflected ray is not itself a separate Love mode: constructive interference of the trapped contributions, including [reflection](../../../../../reflection-mathematics.md) phase, selects the [normal modes](../../../../../normal-mode.md).

For a horizontally propagating mode with $\beta_1<c<\beta_2$, define vertical [wavenumbers](../../../../../wavenumber.md)

$$
q=\omega\sqrt{\beta_1^{-2}-c^{-2}},\qquad
s=\omega\sqrt{c^{-2}-\beta_2^{-2}}.
$$

The free upper surface and welded interface impose the Love-wave [dispersion](../../../../../wave-dispersion.md) condition

$$
\tan(qh)=\frac{\mu_2s}{\mu_1q},\qquad
qh=n\pi+\arctan\frac{\mu_2s}{\mu_1q},\quad n=0,1,2,\ldots,
$$

where $\mu_j=\rho_j\beta_j^2$ are shear moduli. Each phase-velocity branch falls towards $3.5\,\mathrm{km\,s^{-1}}$ with increasing [frequency](../../../../../frequency.md). Higher branches join $4.5\,\mathrm{km\,s^{-1}}$ at their low-frequency cutoffs. At cutoff $s\to0$, so

$$
\boxed{f_{c,n}=\frac{n}{2h\sqrt{\beta_1^{-2}-\beta_2^{-2}}}
\simeq0.0928n\,\mathrm{Hz}.}
$$

Thus the first three [overtones](../../../../../overtone.md) have maximum [periods](../../../../../period-of-a-function.md) about $10.77$, $5.39$ and $3.59\,\mathrm s$. The [fundamental mode](../../../../../fundamental-mode.md) has $n=0$ and **no positive-frequency cutoff in this flat layer-over-half-space model**: it approaches $c=\beta_2$ as $f\to0$, with ever-deeper penetration. The phase-velocity sketch uses an explicitly illustrative equal-density choice, because the question gives [speeds](../../../../../speed.md) but no [density](../../../../../density.md) or rigidity ratio. That missing ratio changes detailed branch curvature, not the cutoff values or the requested branch topology.

For the actual finite spherical [Earth](../../../../../earth.md), the very-long-period continuation must instead be described by discrete toroidal [normal modes](../../../../../normal-mode.md), not a flat infinite [waveguide](../../../../../waveguide.md) at arbitrary [wavelength](../../../../../wavelength.md). The flat-model answer therefore does not assert a continuum of arbitrarily low-frequency global nonrigid oscillations. A global lowest oscillation [frequency](../../../../../frequency.md) cannot be computed from the supplied crust-and-half-space data alone.[§4.18, Love-wave trapping; §4.23, finite spherical Earth and discrete normal modes, especially printed pp. 184–187](../../../../../essentials-of-geophysics-seismology-by-r-d-van-der-hilst.md)

<a id="3/d/image-accurate-direct-reflected-and-critical-head-travel-times-with-illustrative-fundamental-and-first-three-overtone-love-wave-branches"></a>
![](../../../../../past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2013/paper-1-pep-sh-waveguide.png)

**[Figure 3](#3/d/image-accurate-direct-reflected-and-critical-head-travel-times-with-illustrative-fundamental-and-first-three-overtone-love-wave-branches). Accurate direct, reflected and critical-head travel times, with illustrative fundamental and first three overtone Love-wave branches**.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics of the Earth as a Planet course of the University of Cambridge](../../../../split.md)
6. [Physics of the Earth as a Planet course of the University of Cambridge](../../../../../physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
