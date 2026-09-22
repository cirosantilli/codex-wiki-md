# Etendue of a circular aperture and cone

↑ **Parent:** [Etendue](etendue.md)

Consider a planar circular [aperture](aperture.md) of [diameter](diameter.md) $D$ in constant [refractive index](refractive-index.md) $n$. Suppose every position in its [area](surface-area.md) $A=\pi D^2/4$ is filled with directions inside the same rotationally symmetric cone about the [unit normal](unit-normal.md), with half-[angle](angle.md) $\theta_{\max}$. Using [spherical coordinates](spherical-coordinate-system.md), the exact [etendue](etendue.md) is

$$
G=n^2A\int_0^{2\pi}\!\int_0^{\theta_{\max}}
\cos\theta\sin\theta\,d\theta\,d\phi
=n^2A\pi\sin^2\theta_{\max}=\pi A\,\mathrm{NA}^2,
$$

where $\mathrm{NA}=n\sin\theta_{\max}$ is the appropriate side's [numerical aperture](numerical-aperture.md). The ordinary cone [solid angle](solid-angle.md) is $2\pi(1-\cos\theta_{\max})$; its [cosine](cosine.md)-weighted value is $\pi\sin^2\theta_{\max}$. A full forward [hemisphere](hemisphere.md) therefore gives $G=n^2A\pi$, rather than $2\pi n^2A$. [Section 22, slides 22-3–22-4, solid-angle element and exact cone solid angle; slide 22-7, projected-area hemisphere factor](radiative-transfer-lecture-notes-by-john-e-greivenkamp.md)

For an original model example, choose $n=1$, $D=10\,\mathrm{mm}$, and $\theta_{\max}=30^\circ$. Then

$$
A=25\pi\,\mathrm{mm^2},\qquad
G=\frac{25\pi^2}{4}\,\mathrm{mm^2\,sr}
\approx61.685\,\mathrm{mm^2\,sr}.
$$

If the [radiance](radiance.md) is uniform across this filled bundle and equals $L=100\,\mathrm{W\,m^{-2}\,sr^{-1}}$, its [radiant flux](radiant-flux.md) is $\Phi=LG/n^2\approx6.1685\,\mathrm{mW}$. Neither the geometry nor the chosen [radiance](radiance.md) is an experimental measurement.

## ↑ Ancestors (6)

1. [Etendue](etendue.md)
2. [Geometrical optics](geometrical-optics.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Aperture truncation of etendue](aperture-truncation-of-etendue.md)
- [Area-angle tradeoff](area-angle-tradeoff.md)
