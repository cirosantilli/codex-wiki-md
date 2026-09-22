# Stokes settling velocity

↑ **Parent:** [Settling velocity](settling-velocity.md)

<a id="image-sphere-settling-in-water-terminal-speed-grows-as-radius-squared-while-reynolds-number-grows-as-radius-cubed"></a>
![](stokes-settling-size-scaling.png)

**[Figure 1](#image-sphere-settling-in-water-terminal-speed-grows-as-radius-squared-while-reynolds-number-grows-as-radius-cubed). Sphere settling in water: terminal speed grows as radius squared while Reynolds number grows as radius cubed**.

Take downward as positive and let [gravity](gravity.md) have magnitude $g$. For a rigid [sphere](sphere.md) of [density](density.md) $\rho_p$ in otherwise stationary [fluid](fluid.md) of [density](density.md) $\rho_f$, its weight minus [buoyancy](buoyancy.md) is $\tfrac43\pi a^3(\rho_p-\rho_f)g$. At [terminal velocity](terminal-velocity.md), this balances the [Stokes drag law](stokes-s-law.md):

$$
6\pi\mu aU_s=\frac43\pi a^3(\rho_p-\rho_f)g,\qquad
U_s=\frac{2(\rho_p-\rho_f)ga^2}{9\mu}.
$$

This signed downward [settling velocity](settling-velocity.md) is negative for a buoyantly rising [sphere](sphere.md) and zero for equal [densities](density.md). For fixed [density](density.md) contrast and [dynamic viscosity](dynamic-viscosity-split.md), the submerged weight grows as $a^3$ while [linear drag](linear-drag.md) at fixed [speed](speed.md) grows as $a$; their balance gives the [settling-velocity radius scaling](settling-velocity-radius-scaling.md) $U_s\propto a^2$. Meanwhile,

$$
\mathrm{Re}_d=\frac{2a\rho_f|U_s|}{\mu}
=\frac{4\rho_f|\rho_p-\rho_f|ga^3}{9\mu^2}.
$$

Thus doubling the radius multiplies the predicted [Stokes settling speed](stokes-settling-velocity.md) by four and the [particle Reynolds number](particle-reynolds-number.md) by eight. This makes the formula useful for separating particles by size, while also providing its own check against extrapolation to large particles.

For a computed water example, take $\rho_f=1000\ \mathrm{kg\,m^{-3}}$, $\mu=1.00\times10^{-3}\ \mathrm{Pa\,s}$, $\rho_p=2500\ \mathrm{kg\,m^{-3}}$, $g=9.81\ \mathrm{m\,s^{-2}}$, and $a=10.0\ \mathrm{\mu m}$. These are specified rounded inputs rather than a claim of exact water properties at every [temperature](temperature-split.md). They give

$$
U_s=3.27\times10^{-4}\ \mathrm{m\,s^{-1}}=0.327\ \mathrm{mm\,s^{-1}},\qquad
\mathrm{Re}_d=\frac{1000(3.27\times10^{-4})(20.0\times10^{-6})}{10^{-3}}=0.00654.
$$

The diameter is $20.0\ \mathrm{\mu m}$, and both the net downward weight and the upward [drag force](drag-physics.md) are $6.16\times10^{-11}\ \mathrm N$. At this [terminal velocity](terminal-velocity.md), falling $1.00\ \mathrm{mm}$ takes $3.06\ \mathrm s$. At $a=20.0\ \mathrm{\mu m}$ the prediction is $1.308\ \mathrm{mm\,s^{-1}}$ with $\mathrm{Re}_d=0.05232$; at $a=50.0\ \mathrm{\mu m}$ it is $8.175\ \mathrm{mm\,s^{-1}}$ with $\mathrm{Re}_d=0.8175$, which is no longer a convincing small-[Reynolds number](reynolds-number.md) case. The figure labels these as predictions of the [Stokes settling velocity](stokes-settling-velocity.md) formula and shows where its [inertia](inertia.md) check fails.

The calculation describes the eventual [terminal velocity](terminal-velocity.md), not the release transient governed by particle [acceleration](acceleration.md) and possibly the [Unsteady Stokes equation](unsteady-stokes-equation.md). Walls, [hydrodynamic interactions](hydrodynamic-interaction.md), departures from a rigid [sphere](sphere.md), or a different surface condition require a different resistance. For sufficiently small particles, [Brownian motion](brownian-motion-split.md) can obscure individual settling trajectories; the formula still specifies the gravitational drift within its assumptions. The balancing argument already appears in article 43 of [Stokes's original investigation, collected-paper reprint](https://mural.uv.es/daroig/documentos/stokes1850.pdf).

## ↑ Ancestors (6)

1. [Settling velocity](settling-velocity.md)
2. [Suspension (chemistry)](suspension-chemistry-split.md)
3. [Fluid mechanics](fluid-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-80/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-345/1/a/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2016/paper-1/1/c/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2018/section-a/1/b/solution.md)
- [Perrin sedimentation experiment](perrin-sedimentation-experiment.md)
- [Stokes equation](stokes-equation.md)
- [Stokes's law](stokes-s-law.md)
- [Stokes settling velocity](stokes-settling-velocity.md)
- [Wall hindrance in Brownian diffusion](wall-hindrance-in-brownian-diffusion.md)
