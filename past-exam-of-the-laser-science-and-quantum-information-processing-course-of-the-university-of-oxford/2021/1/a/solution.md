<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $s=z-z_0$. In the source's [complex beam parameter](../../../../complex-beam-parameter.md) convention,

$$
\frac1q=\frac{s+iz_R}{s^2+z_R^2}
=\frac1{R(z)}+i\frac{2}{kw(z)^2}.
$$

Substitution separates the transverse [wave amplitude](../../../../wave-amplitude.md) and [phase](../../../../phase-waves.md):

$$
U=\frac{U_0e^{i(kz-\omega t)}}{s-iz_R}
\exp\!\left[-\frac{\rho^2}{w(z)^2}\right]
\exp\!\left[i\frac{k\rho^2}{2R(z)}\right].
$$

Thus the [Gaussian beam](../../../../gaussian-beam.md) is circularly symmetric, has a [Gaussian function](../../../../gaussian-function.md) transverse [light intensity](../../../../light-intensity.md), and narrows to a [beam waist](../../../../beam-waist.md) at $z_0$ before spreading by [diffraction](../../../../diffraction.md). Its [wavefront](../../../../wavefront.md) is planar at the [beam waist](../../../../beam-waist.md), converging before it and diverging after it. The quadratic transverse [phase](../../../../phase-waves.md) identifies the signed [radius of curvature](../../../../radius-of-curvature.md):

$$
\boxed{R(z)=s+\frac{z_R^2}{s},\qquad R(z_0)=\infty.}
$$

Define spot size as the [wave amplitude](../../../../wave-amplitude.md) $1/e$ [radius](../../../../radius.md), equivalently the [light intensity](../../../../light-intensity.md) $1/e^2$ [radius](../../../../radius.md). Then

$$
\boxed{w(z)^2=\frac{2(s^2+z_R^2)}{kz_R}
=w_0^2\left(1+\frac{s^2}{z_R^2}\right),\qquad
w_0^2=\frac{2z_R}{k}=\frac{\lambda z_R}{\pi}.}
$$

The [Rayleigh range](../../../../rayleigh-length.md) is where $w=\sqrt2w_0$; the far-field [beam divergence](../../../../beam-divergence.md) half-angle is $\lambda/(\pi w_0)$. The factor $1/q$ also produces a longitudinal [phase](../../../../phase-waves.md) shift relative to a [plane wave](../../../../plane-wave.md), changing by $\pi$ across the [beam waist](../../../../beam-waist.md); its sign here follows the given $e^{i(kz-\omega t)}$ convention. The on-axis [light intensity](../../../../light-intensity.md) decreases as $1/(s^2+z_R^2)$ while transverse integration leaves the [power](../../../../power.md) constant. These are scalar [paraxial approximation](../../../../paraxial-approximation.md) results.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
