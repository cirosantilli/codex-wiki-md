# Etendue concentration limit

↑ **Parent:** [Optical concentrator](optical-concentrator.md)

Suppose an extended source fills every position of the entrance [aperture](aperture.md) with a cone of half-[angle](angle.md) $\theta_{\rm in}$, and all these [light rays](light-ray.md) must reach a one-sided planar receiver. If the receiver accepts at most a cone of half-[angle](angle.md) $\theta_{\rm out}$, its available [etendue](etendue.md) bounds the admitted [etendue](etendue.md):

$$
n_{\rm in}^2A_{\rm in}\pi\sin^2\theta_{\rm in}
\leq n_{\rm out}^2A_{\rm out}\pi\sin^2\theta_{\rm out}.
$$

Consequently

$$
C\leq\frac{n_{\rm out}^2\sin^2\theta_{\rm out}}
{n_{\rm in}^2\sin^2\theta_{\rm in}}
\leq\frac{n_{\rm out}^2}{n_{\rm in}^2\sin^2\theta_{\rm in}}.
$$

This original derivation combines [conservation of etendue](conservation-of-etendue.md) with the exact cone [integral](integral.md); the second inequality allows the complete output [hemisphere](hemisphere.md). It bounds capacity and does not prove that a chosen shape attains the bound.

<a id="image-aperture-clipping-discards-etendue-full-flux-concentration-requires-a-larger-output-angular-range"></a>
![](etendue-aperture-truncation-concentration.png)

**[Figure 39](#image-aperture-clipping-discards-etendue-full-flux-concentration-requires-a-larger-output-angular-range). Aperture clipping discards etendue; full-flux concentration requires a larger output angular range**. Left: a $6\,\mathrm{mm}$ stop transmits $36\%$ of the spatial disk with unchanged directional acceptance. Right: endpoint geometry for the ideal air-to-air $30^\circ$ input-cone bound, $C\leq4$. Interior sides are only a symbolic connection between ports, not a designed reflector or a traced ray path.

For the $30^\circ$ input cone with $n_{\rm in}=n_{\rm out}=1$, $C\leq4$: a $10\,\mathrm{mm}$ entrance cannot deliver the entire filled bundle to a circular receiver smaller than $5\,\mathrm{mm}$ in [diameter](diameter.md). If the output half-[angle](angle.md) is restricted to $60^\circ$, $C\leq3$ and the receiver [diameter](diameter.md) must be at least $10/\sqrt3\approx5.7735\,\mathrm{mm}$. For a receiver medium with model [refractive index](refractive-index.md) $n_{\rm out}=1.5$, the full-[hemisphere](hemisphere.md) capacity bound instead gives $C\leq9$; that larger value also depends on transmitting the bundle into that medium.

Attempting $C=10$ in the air-to-air example forces rejection of some input. For the uniform [radiance](radiance.md) already specified, even filling the entire output [hemisphere](hemisphere.md) gives

$$
\eta=\frac{\Phi_{\rm out}}{\Phi_{\rm in}}
\leq\frac{G_{\rm out,capacity}}{G_{\rm in}}=\frac4{10}=0.4.
$$

The maximum mean [irradiance](irradiance.md) gain remains $\eta C\leq4$. With nonuniform [radiance](radiance.md), rejecting a given fraction of geometric [etendue](etendue.md) need not reject the same fraction of [radiant flux](radiant-flux.md).

These bounds use a filled extended-source bundle in passive reversible [geometrical optics](geometrical-optics.md), comparing the same [wavelength](wavelength.md) and the same radiation channels. An ideal [optical point source](optical-point-source.md) does not fill that four-dimensional set. [Diffraction](diffraction.md), [optical coherence](optical-coherence.md), or coupling a [Gaussian beam](gaussian-beam.md) into an [optical fiber](optical-fiber.md) require a [physical optics](physical-optics.md) calculation; the cone bound is not a universal guarantee for a single wave mode. Likewise, [optical gain](optical-gain.md) or [fluorescence](fluorescence.md) changes the propagation assumptions.

## ↑ Ancestors (7)

1. [Optical concentrator](optical-concentrator.md)
2. [Etendue](etendue.md)
3. [Geometrical optics](geometrical-optics.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
