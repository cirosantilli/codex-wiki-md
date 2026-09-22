# Optical fiber acceptance angle

↑ **Parent:** [Step-index optical fiber](step-index-optical-fiber.md)

The [optical fiber acceptance angle](optical-fiber-acceptance-angle.md) is the largest launch half-[angle](angle.md) admitted by the specified guide model. For a flat entrance face perpendicular to the [optical axis](optical-axis.md), external [refractive index](refractive-index.md) $n_0$, and a straight [step-index optical fiber](step-index-optical-fiber.md), [Snell's law](snell-s-law.md) at the entrance gives

$$
n_0\sin\theta=n_1\sin\phi.
$$

At the core–cladding interface, the [critical angle for total internal reflection](critical-angle-for-total-internal-reflection.md) $i_c$ satisfies

$$
\sin i_c=\frac{n_2}{n_1},\qquad i=\frac{\pi}{2}-\phi.
$$

For a [meridional ray](meridional-ray.md), strict [total internal reflection](total-internal-reflection.md) requires $i>i_c$. At the limiting geometry $i=i_c$, the refracted [light ray](light-ray.md) is tangent to the interface, so

$$
n_0\sin\theta_{\max}
=n_1\cos i_c
=\sqrt{n_1^2-n_2^2}
\equiv\mathrm{NA}.
$$

This identifies the [numerical aperture](numerical-aperture.md) with an entrance cone under these assumptions. With $n_0=1$ for air, the conventional inclusive boundary condition is

$$
\sin\theta\leq\sqrt{n_1^2-n_2^2},
$$

for a nonnegative launch [angle](angle.md) $\theta$; a practical launch stays inside the boundary. If $\mathrm{NA}>n_0$, this ideal model imposes no further restriction within the forward hemisphere, and $\arcsin(\mathrm{NA}/n_0)$ must not be used. The [light ray](light-ray.md) must also intersect the [optical fiber core](optical-fiber-core.md): a suitable [angle](angle.md) alone does not correct a misplaced beam.

For an original example, take $n_1=1.50$, $n_2=1.48$ and air at the entrance. Then

$$
\mathrm{NA}=\sqrt{2.25-2.1904}=\sqrt{0.0596}\simeq0.244131,
\qquad
\theta_{\max}=\arcsin(0.244131)\simeq14.13^\circ.
$$

The internal limiting [angle](angle.md) is only $\phi_{\max}\simeq9.37^\circ$, while the [critical angle for total internal reflection](critical-angle-for-total-internal-reflection.md) is $i_c\simeq80.63^\circ$. A $10^\circ$ launch has $\phi\simeq6.65^\circ$ and $i\simeq83.35^\circ$, so it satisfies [total internal reflection](total-internal-reflection.md). A $20^\circ$ launch has $\phi\simeq13.18^\circ$ and $i\simeq76.82^\circ$, so it fails this test.

This cone is a [geometrical optics](geometrical-optics-split.md) result for [meridional rays](meridional-ray.md). A [single-mode optical fiber](single-mode-optical-fiber.md) requires the spatial overlap of the incident [electromagnetic wave](electromagnetic-wave-split.md) with its guided [normal mode](normal-mode.md); its [numerical aperture](numerical-aperture.md) does not impose an exact angular cutoff on arbitrary beams. [Diffraction](diffraction.md), finite cladding, and bends require a [physical optics](physical-optics-split.md) description.[Insights into Optical Fiber, When does NA provide a good estimate of the fiber's acceptance angle?, Geometry Defines the Relationship and Single Mode Fibers are Different; revised January 20, 2020](when-does-na-provide-a-good-estimate-of-the-fiber-s-acceptance-angle-by-thorlabs.md)

## ↑ Ancestors (7)

1. [Step-index optical fiber](step-index-optical-fiber.md)
2. [Optical fiber](optical-fiber.md)
3. [Optical instrument](optical-instrument-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Meridional ray](meridional-ray.md)
- [Optical fiber](optical-fiber.md)
- [Optical fiber acceptance angle](optical-fiber-acceptance-angle.md)
