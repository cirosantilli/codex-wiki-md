# Manometer height-to-pressure calibration

↑ **Parent:** [U-tube differential manometer](u-tube-differential-manometer.md)

The ideal [measurement calibration](measurement-calibration.md) is a straight line through the equal-pressure zero. For the stipulated [water](water.md) [mass density](density.md) and [gravitational acceleration](gravitational-acceleration.md) above, its slope is $9.81\,\mathrm{Pa}$ per vertical millimetre. A lower [liquid](liquid.md) [mass density](density.md) gives a larger [length](length.md) change for the same [pressure](pressure-split.md), improving the height-reading contribution to [measurement resolution](measurement-resolution.md) but requiring more vertical space for a given [pressure](pressure-split.md) range. The [pressure](pressure-split.md) scale depends on the actual [mass density](density.md), which depends on [temperature](temperature-split.md); $1000\,\mathrm{kg\,m^{-3}}$ here is a chosen model value, not an exact property of all [water](water.md) samples.

<a id="image-calculated-water-column-pressure-scale-and-a-two-meniscus-rounding-model"></a>
![](manometer-height-pressure-resolution.png)

**[Figure 4](#image-calculated-water-column-pressure-scale-and-a-two-meniscus-rounding-model). Calculated water-column pressure scale and a two-meniscus rounding model**. The left panel is the theoretical [measurement calibration](measurement-calibration.md) for $\rho=1000\,\mathrm{kg\,m^{-3}}$ and $g=9.81\,\mathrm{m\,s^{-2}}$. The right panel models two [liquid meniscus](meniscus-liquid-surface.md) heights read separately to the nearest millimetre: each rounding [measurement error](measurement-error.md) is assumed independently uniform between $-0.5$ and $0.5\,\mathrm{mm}$. Their difference gives a triangular [probability density function](probability-density-function.md) for the inferred [pressure](pressure-split.md) error. The bounds and [standard uncertainty](standard-uncertainty.md) describe this constructed model, not observed instrument data.

Suppose each [liquid meniscus](meniscus-liquid-surface.md) height is rounded to the nearest scale division $q=1\,\mathrm{mm}$. Each height [measurement error](measurement-error.md) lies within $q/2$, so the error in their difference lies within $q$. The resulting [pressure](pressure-split.md) error is bounded by $\rho gq=9.81\,\mathrm{Pa}$. To quantify a [standard uncertainty](standard-uncertainty.md), make the additional model assumption that the two rounding errors are [independent random variables](independent-random-variables.md), each having a [continuous uniform distribution](continuous-uniform-distribution.md) on $[-q/2,q/2]$. Each then has [variance](variance-split.md) $q^2/12$; adding the two [variances](variance-split.md) gives

$$
u(\Delta h)=\frac{q}{\sqrt6},\qquad
u(\Delta p)=\frac{\rho gq}{\sqrt6}=4.0049\,\mathrm{Pa}.
$$

Here $u$ denotes [standard uncertainty](standard-uncertainty.md). The $9.81\,\mathrm{Pa}$ worst-case bound and $4.0049\,\mathrm{Pa}$ [standard uncertainty](standard-uncertainty.md) answer different questions. At $588.6\,\mathrm{Pa}$ they are respectively $1.67\%$ and $0.680\%$ of the reading. Shared reading bias or a different reading method can violate the assumed [independence](independent-random-variables.md).

If the [mass density](density.md), [gravitational acceleration](gravitational-acceleration.md) and height difference also have small independent [standard uncertainties](standard-uncertainty.md), a first-order estimate follows from the [partial derivatives](partial-derivative.md) of $\Delta p=\rho g\Delta h$:

$$
u^2(\Delta p)\simeq(g\Delta h)^2u^2(\rho)+(\rho\Delta h)^2u^2(g)+(\rho g)^2u^2(\Delta h).
$$

This displays why a finer scale does not remove uncertainty in [mass density](density.md) or [gravitational acceleration](gravitational-acceleration.md). A [pressure transducer](pressure-transducer.md) compared against the column needs its own [differential-pressure calibration](differential-pressure-calibration.md) to establish an electrical response.

## ↑ Ancestors (6)

1. [U-tube differential manometer](u-tube-differential-manometer.md)
2. [Manometer](manometer.md)
3. [Fluid mechanics](fluid-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Measurement resolution](measurement-resolution.md)
