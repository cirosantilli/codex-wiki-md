# Grazing-incidence X-ray optics

↑ **Parent:** [X-ray astronomy](x-ray-astronomy.md)

[Grazing-incidence X-ray optics](grazing-incidence-x-ray-optics.md) redirect [X-rays](x-ray.md) by shallow [specular reflections](specular-reflection.md) along mirror surfaces. [Riccardo Giacconi](riccardo-giacconi.md)'s lecture describes coaxial paraboloidal and hyperboloidal mirrors using two reflections, and the later Einstein observatory's imaging capability. Focusing separates collecting area from detector area: the collected source signal can remain large while the detector background is drawn from a smaller region.[sections 3.2–4, pp. 123–124, Fig. 13](the-dawn-of-x-ray-astronomy-by-riccardo-giacconi.md)

An ideal lossless [geometrical optics](geometrical-optics-split.md) calculation explains the shallow angle. Take vacuum [refractive index](refractive-index.md) one and a material with real [refractive index](refractive-index.md) $n=1-\delta$, where $0<\delta\ll1$. Let $\theta$ be the grazing angle measured from the surface. [Snell's law](snell-s-law.md) written for angles from the normal requires $\cos\theta=n\sin\theta_t$. A propagating transmitted ray exists only if $\cos\theta\leq n$. Thus the ideal threshold is

$$
\theta_c=\arccos(1-\delta)\simeq\sqrt{2\delta}.
$$

The last step uses the [Taylor series](taylor-series.md) $\cos\theta=1-\theta^2/2+O(\theta^4)$. For a chosen $\delta=2\times10^{-5}$, $\theta_c\simeq0.006325$ [radians](radian.md), or $0.3624^\circ$. Absorption makes the [refractive index](refractive-index.md) complex and softens this ideal threshold; surface roughness and alignment errors also reduce throughput or worsen the [point spread function](point-spread-function-split.md). These are reasons to calibrate [X-ray effective area](x-ray-effective-area.md) and [angular resolution](angular-resolution.md), rather than assume that reflection is perfect.

The benefit can be quantified without specifying a historical telescope. Suppose a source retains fraction $f$ of its counts inside an extraction region, while a uniform detector background contributes $q a t$ counts over detector area $a$. In the background-dominated limit of the same independent on-off model,

$$
Z\simeq\frac{f F A_{\mathrm{eff}}\sqrt t}{\sqrt{(1+\alpha)q a}}.
$$

Reducing $a$ by a factor of 100 at fixed $f$ and [X-ray effective area](x-ray-effective-area.md) improves this ideal ratio tenfold. A [collimator](collimator.md) restricts admitted directions; focusing optics bring selected rays together. An image also separates nearby sources and identifies clean background regions, connecting optical design directly to a better constrained [inverse problem](inverse-problem-split.md).

## ↑ Ancestors (6)

1. [X-ray astronomy](x-ray-astronomy.md)
2. [Observational astronomy](observational-astronomy.md)
3. [Astrophysics](astrophysics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Grazing-incidence X-ray optics](grazing-incidence-x-ray-optics.md)
- [X-ray astronomy](x-ray-astronomy.md)
