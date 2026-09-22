# Phase-conjugate ray retracing

↑ **Parent:** [Phase-conjugate mirror](phase-conjugate-mirror.md)

Consider an [optical point source](optical-point-source.md) at $(z,x)=(0,0)$, a uniform transparent medium, and a flat return surface $z=L$. A [light ray](light-ray.md) with slope $s$ reaches $(L,sL)$. A [phase-conjugate mirror](phase-conjugate-mirror.md) reverses its full direction and returns it to $(0,0)$. An ordinary mirror reverses only its normal direction; its returning [light ray](light-ray.md) reaches $x=2sL$ at $z=0$. Thus rays with $s=-1/4,0,1/4$ at $L=3$ return to $x=-3/2,0,3/2$ with ordinary [specular reflection](specular-reflection.md), but all return to $x=0$ under ideal [phase conjugation](phase-conjugation.md). These are stipulated geometric coordinates, not laboratory measurements.

<a id="phase-conjugate-wavefront-ray-retracing"></a>
![](phase-conjugate-wavefront-ray-retracing.png)

**[Figure 5](#phase-conjugate-wavefront-ray-retracing). Ordinary reflection and ideal phase conjugation: curved wavefronts and returning light rays**.

Solid blue curves mark outward [wavefronts](wavefront.md); dashed curves mark returning [wavefronts](wavefront.md). In the [phase-conjugate mirror](phase-conjugate-mirror.md) panel the returning curves coincide with the outward ones, and the arrows reverse on the same [light rays](light-ray.md). The diagram uses equal spatial scales. In [geometrical optics](geometrical-optics-split.md), reversing each [light ray](light-ray.md) in an unchanged medium with [wave reciprocity](wave-reciprocity.md) retraces its route. At the [optical point source](optical-point-source.md) itself, the ray construction becomes singular and [diffraction](diffraction.md) sets the physical focal size.

A wave-level proof outline applies to a stationary scalar medium with real [refractive index](refractive-index.md) $n(\mathbf r)$ and no [wave absorption](wave-absorption.md). Writing $c$ for the [vacuum](vacuum.md) [speed of light](speed-of-light.md), its [Helmholtz equation](helmholtz-equation.md) is

$$
\nabla^2U+k_0^2n(\mathbf r)^2U=0,\qquad k_0=\omega/c.
$$

All coefficients are real, so [complex conjugation](complex-conjugation.md) gives the same [Helmholtz equation](helmholtz-equation.md) for $U^*$. The conjugated outgoing boundary data select the incoming solution. This explains the connection between [phase conjugation](phase-conjugation.md) and retracing, provided the required incoming field is supplied over the necessary [aperture](aperture.md). It also exposes the limits: [wave reciprocity](wave-reciprocity.md) alone does not imply absence of [wave absorption](wave-absorption.md); conjugation of complex material coefficients would describe a different medium. Loss, an incomplete [aperture](aperture.md), a changing medium or failure of [wave reciprocity](wave-reciprocity.md) can prevent exact reconstruction. Intensity-dependent material changes need a separate analysis and are not covered by this linear proof.

## ↑ Ancestors (7)

1. [Phase-conjugate mirror](phase-conjugate-mirror.md)
2. [Phase conjugation](phase-conjugation.md)
3. [Physical optics](physical-optics-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
