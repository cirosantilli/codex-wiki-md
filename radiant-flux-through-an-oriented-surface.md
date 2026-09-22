# Radiant flux through an oriented surface

↑ **Parent:** [Radiant flux](radiant-flux.md)

In [geometrical optics](geometrical-optics-split.md), suppose radiation has a nonnegative [radiance](radiance.md) $L(\mathbf x,\mathbf s)$ whose directional contributions add as [power](power.md). Here $\mathbf s$ is the actual propagation [unit vector](unit-vector.md), $d\Omega$ is a [solid angle](solid-angle.md) element, and the collecting [oriented surface](oriented-surface.md) $A$ has chosen [unit normal](unit-normal.md) $\mathbf n(\mathbf x)$. Assume the following [integrals](integral-split.md) exist. The outward and inward [radiant fluxes](radiant-flux.md) are

$$
\Phi_+=\int_A\!\int_{\mathbf n\cdot\mathbf s>0}
L(\mathbf x,\mathbf s)(\mathbf n\cdot\mathbf s)\,d\Omega\,dA,
\qquad
\Phi_-=\int_A\!\int_{\mathbf n\cdot\mathbf s<0}
L(\mathbf x,\mathbf s)(-\mathbf n\cdot\mathbf s)\,d\Omega\,dA.
$$

Both quantities are nonnegative; their difference is the signed net [radiant flux](radiant-flux.md). The [dot product](dot-product.md) supplies the [cosine](cosine.md) of the [angle](angle.md) with the [unit normal](unit-normal.md), hence the [projected area](projected-area.md). For incoming radiation the outward [unit normal](unit-normal.md) gives a negative [dot product](dot-product.md); the minus sign makes the collected [power](power.md) positive. Measuring the incoming [angle](angle.md) from a source-facing [unit normal](unit-normal.md) instead gives the familiar positive $\cos\theta$. The units check is $\mathrm{W\,m^{-2}\,sr^{-1}}\times\mathrm{m^2}\times\mathrm{sr}=\mathrm W$.

Equivalently, the incoming [surface integral](surface-integral.md) is $\Phi_-=\int_A E\,dA$ with local [irradiance](irradiance.md) $E$; the emitted part of $\Phi_+$ is $\int_A M\,dA$ with [radiant exitance](radiant-exitance.md) $M$. For a small flat patch and a narrow accepted cone, nearly constant [radiance](radiance.md) and [angle](angle.md) give $\Phi\simeq LA\cos\theta\,\Delta\Omega$. This approximation requires uniformity across the patch and cone. Direction-independent outgoing [radiance](radiance.md) over a whole [hemisphere](hemisphere.md) gives the different exact result $\Phi_+=\pi LA$, by [Lambert's cosine law](lambert-s-cosine-law.md) and the [spherical coordinates](spherical-coordinate-system.md) calculation in [radiant exitance](radiant-exitance.md). Replacing the [cosine](cosine.md)-weighted [integral](integral-split.md) by the [hemisphere](hemisphere.md)'s $2\pi$ [solid angle](solid-angle.md) would double the answer.[Radiometry and Photometry](radiometry-and-photometry.md)

These [radiance](radiance.md) formulas presume a description in additive directional [power](power.md); they do not reconstruct arbitrary coherent [wave interference](interference-wave-propagation.md) from separate ray contributions. For general [electromagnetic fields](electromagnetic-field.md), the signed instantaneous [power](power.md) crossing an [oriented surface](oriented-surface.md) is $\int_A\mathbf S\cdot\mathbf n\,dA$, using the [Poynting vector](poynting-vector.md) $\mathbf S$; optical measurements commonly average over many [wave periods](wave-period.md). A zero net [radiant flux](radiant-flux.md) can conceal equal nonzero incoming and outgoing [radiant fluxes](radiant-flux.md).

## ↑ Ancestors (6)

1. [Radiant flux](radiant-flux.md)
2. [Radiometry](radiometry-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
