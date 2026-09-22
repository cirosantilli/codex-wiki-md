<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The target liquid-[water](../../../../water.md) [mass](../../../../mass.md) is

$$
m_* =\frac{4\pi}{3}(10^3)(15\times10^{-6})^3
=1.414\times10^{-11}\,\mathrm{kg}.
$$

The [thin-plate ice-growth time](../../../../thin-plate-ice-growth-time.md) uses the prescribed ice [mass](../../../../mass.md) law, which therefore requires $r_{i*}=(m_*/\alpha)^{1/3}=45.31\,\mu\mathrm m$, not the same [radius](../../../../radius.md) as the [water](../../../../water.md) droplet. With $C=2r_i/\pi$ and $F_i=F_k^i+F_d^i$,

$$
3\alpha r_i^2\frac{dr_i}{dt}=\frac{8r_i(S^i-1)}{F_i},\qquad
\frac{d(r_i^2)}{dt}=\frac{16(S^i-1)}{3\alpha F_i}.
$$

Hence, for negligible seed [mass](../../../../mass.md) and constant conditions,

$$
\boxed{t_i=\frac{3\alpha F_i r_{i*}^2}{16(S^i-1)}
=\frac{3(152)(2.1\times10^7)(45.31\times10^{-6})^2}{16(0.05)}
\simeq24.6\,\mathrm s.}
$$

This is about $8.24$ times faster than the liquid estimate to the same [mass](../../../../mass.md). Both laws have $dm/dt\propto m^{1/3}$ under the given shape assumptions. Ice benefits here from five times the [atmospheric supersaturation](../../../../atmospheric-supersaturation.md) and a larger geometrical [capacitance](../../../../diffusion-capacitance-analogy.md) for the same [mass](../../../../mass.md), partly offset by its slightly greater transport resistance. The [mass](../../../../mass.md) coefficient $\alpha$ encodes the assumed plate shape; replacing it by bulk ice [density](../../../../density.md) would change the supplied model.

In a mixed-phase [cloud](../../../../cloud.md), saturation vapour [pressure](../../../../pressure-split.md) over ice is lower than over supercooled liquid [water](../../../../water.md). Air can therefore be subsaturated with respect to liquid yet supersaturated with respect to ice: droplets evaporate while ice crystals grow, transferring [water](../../../../water.md) through the vapour phase. This is the [Wegener–Bergeron–Findeisen mechanism](../../../../wegener-bergeron-findeisen-process.md). Subsequent aggregation, [riming](../../../../riming.md) and melting can produce [atmospheric precipitation](../../../../atmospheric-precipitation.md) much faster than [condensation](../../../../condensation.md) alone.

The large difference is not a universal fixed ice/liquid time ratio. [Atmospheric supersaturation](../../../../atmospheric-supersaturation.md) evolves, latent heating increases thermal resistance, crystal habits and [capacitance](../../../../diffusion-capacitance-analogy.md) change, and surface attachment or ventilation may matter. Ice nucleation and the availability of freezing nuclei also precede the calculated growth. The boxed time describes the specified already-present crystals under maintained conditions, not a complete prediction of the time until rain begins.

## ↑ Ancestors (12)

1. [D](../d.md)
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
