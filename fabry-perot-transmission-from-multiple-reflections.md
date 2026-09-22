<h1 id="fabry-perot-transmission-from-multiple-reflections">Fabry–Pérot transmission from multiple reflections</h1>

↑ **Parent:** [Fabry–Pérot interferometer](fabry-perot-interferometer.md)

Consider two identical, lossless parallel mirrors with intensity reflectivity $0\leq R<1$, separation $d$, and a uniform transparent medium of [refractive index](refractive-index.md) $n$. Fix one [polarization of an electromagnetic wave](polarization-of-an-electromagnetic-wave.md) and an internal [angle of incidence](angle-of-incidence.md) $\theta$ measured from the mirror [normal vector](normal-vector.md). Illuminate with a [monochromatic wave](monochromatic-wave.md) having planar [wavefronts](wavefront.md); the emerging contributions must overlap coherently in the detected direction. Define $T=I_{\rm transmitted}/I_{\rm incident}$ using the same incident and exit media. Each mirror transmits a fraction $1-R$ of incident [power](power.md). Its reflected [wave amplitude](wave-amplitude.md) has magnitude $\sqrt R$, so two internal [specular reflections](specular-reflection.md) multiply the circulating [complex amplitude](complex-amplitude.md) by magnitude $R$, not $R^2$.

Let $\lambda$ be the [vacuum](vacuum.md) [wavelength](wavelength.md) and choose the reflection [wave phase](phase-waves.md) convention in which the product of the two internal amplitude reflection coefficients is real and positive. The [phase difference](phase-difference.md) between successive transmitted contributions, evaluated on a common outgoing [wavefront](wavefront.md), is

$$
\delta=\frac{4\pi nd\cos\theta}{\lambda}.
$$

With other mirror coatings or phase conventions, use the total $\delta=4\pi nd\cos\theta/\lambda+\phi_{\rm rt}$, where $\phi_{\rm rt}$ is the sum of the two internal reflection [wave phases](phase-waves.md). The stated resonance positions presume $\phi_{\rm rt}=0$ modulo $2\pi$; a constant nonzero $\phi_{\rm rt}$ shifts them, while a [frequency](frequency.md)-dependent one can also change their spacing.

Why does the [cosine](cosine.md) appear rather than its reciprocal? Inside the gap, the extra two legs have [optical path length](optical-path-length.md) $2nd/\cos\theta$. But the later emerging contribution starts $2d\tan\theta$ farther along the mirror. Comparing both on one outgoing [wavefront](wavefront.md) subtracts $2nd\tan\theta\sin\theta$ from that path difference, leaving $2nd\cos\theta$. Equivalently, a [plane wave](plane-wave.md)'s mirror-normal [wavevector](wavevector.md) component is $k_z=(2\pi n/\lambda)\cos\theta$, so the round-trip [wave phase](phase-waves.md) is $2k_zd$. The diagram uses the same medium outside and inside to show the common-[wavefront](wavefront.md) subtraction directly; at a refracting exit interface, tangential [wavevector](wavevector.md) matching in [Snell's law](snell-s-law.md) supplies the same result.

<a id="image-multiple-specular-reflections-become-a-coherent-sum-of-transmitted-complex-amplitudes"></a>
![](fabry-perot-multiple-reflection-phase-addition.png)

**[Figure 2](#image-multiple-specular-reflections-become-a-coherent-sum-of-transmitted-complex-amplitudes). Multiple specular reflections become a coherent sum of transmitted complex amplitudes**. Original ideal geometry and amplitude construction, not apparatus data. The oblique rays expose successive round trips and the common outgoing [wavefront](wavefront.md); $\theta$ is internal. The amplitude panels independently use $R=0.75$ at $\delta=0$ and $\delta=\pi/2$. Only the first five terms are drawn, with the infinite-sum endpoints marked. At [normal incidence](normal-incidence.md) the outgoing contributions overlap directly.

Absorb the common first-pass [wave phase](phase-waves.md) into the incident [complex amplitude](complex-amplitude.md) $E_{\rm in}$. Successive transmitted contributions are $(1-R)E_{\rm in}$, $(1-R)E_{\rm in}Re^{i\delta}$, and so on. The [superposition principle](superposition-principle.md) and the convergent [geometric series](geometric-series.md) give

$$
\frac{E_{\rm out}}{E_{\rm in}}=(1-R)\sum_{j=0}^{\infty}R^j e^{ij\delta}
=\frac{1-R}{1-Re^{i\delta}},\qquad
T=\left|\frac{E_{\rm out}}{E_{\rm in}}\right|^2
=\frac{(1-R)^2}{(1-R)^2+4R\sin^2(\delta/2)}.
$$

The last step expands the squared [complex modulus](complex-modulus.md) as $1+R^2-2R\cos\delta$. This transmission profile is often called the Airy transmission function; it is distinct from the [Airy disk](airy-disk.md), a [diffraction](diffraction.md) image of a circular [aperture](aperture.md). The University of Washington's lab handout gives the same transmission profile and distinguishes mirror reflectivity from other sources of peak broadening.[Fabry-Perot Interferometer, theory equation (2), Finesse discussion, equations (4)–(8)](fabry-perot-interferometer-university-of-washington-physics-331.md)

For an original example, set $R=3/4$. At $\delta=0$, the amplitudes add to $(1/4)/(1-3/4)=1$, so $T=1$. At $\delta=\pi$, they alternate in sign and add to $(1/4)/(1+3/4)=1/7$, so $T=1/49$. At $\delta=\pi/2$, the amplitude is $4/25+3i/25$ and $T=1/25$. Adding the individual intensities instead would give $(1-R)^2\sum_j R^{2j}=(1-R)/(1+R)=1/7$, independent of [wave phase](phase-waves.md); that discards the [wave interference](interference-wave-propagation.md) responsible for the peaks.

In general the maximum is $T_{\max}=1$ at $\delta=2\pi m$, with [integer](integer-split.md) $m$, and the minimum is $T_{\min}=[(1-R)/(1+R)]^2$ halfway between peaks. Perfect resonant transmission requires identical lossless mirrors, coherent illumination, and sufficient time to establish the steady field. Absorption, unequal mirror transmission, finite beams that fail to overlap, and fluctuations of $d$ can reduce it. The exactly reflecting case $R=1$ is excluded: no incident [power](power.md) enters through a perfectly reflecting mirror, and the resonant limit $R\to1^-$ is singular.

## ↑ Ancestors (6)

1. [Fabry–Pérot interferometer](fabry-perot-interferometer.md)
2. [Optical instrument](optical-instrument-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Fabry–Pérot resonance spacing](fabry-perot-resonance-spacing.md)
- [Finesse](finesse.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1/section-b/b9/solution.md)
