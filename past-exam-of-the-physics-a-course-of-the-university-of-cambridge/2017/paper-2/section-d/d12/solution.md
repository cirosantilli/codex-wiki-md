<h1 id="section-d/d12/solution">Solution</h1>

↑ **Parent:** [D12](../d12.md)

**Circular [apertures](../../../../../aperture.md) and circular obstructions illustrate both the usefulness and the limits of geometric shadow arguments.** In [scalar diffraction theory](../../../../../scalar-diffraction-theory.md), each point of a transmitted [wavefront](../../../../../wavefront.md) contributes a complex secondary field. Their coherent sum, described by the [Huygens-Fresnel principle](../../../../../huygens-fresnel-principle.md), determines the intensity. Circular symmetry simplifies the integral, but the answer depends on whether propagation is in the [Fraunhofer diffraction](../../../../../fraunhofer-diffraction.md) or [Fresnel diffraction](../../../../../fresnel-diffraction.md) regime.

For [aperture](../../../../../aperture.md) radius $a$ and axial propagation distance $z$, the [Fresnel number](../../../../../fresnel-number.md) $N_F=a^2/(\lambda z)$ measures the importance of quadratic [phase](../../../../../phase-waves.md) across the [aperture](../../../../../aperture.md). The far-field condition is $N_F\ll1$; a lens can produce the same angular spectrum in its back focal plane. Fresnel propagation retains that quadratic [phase](../../../../../phase-waves.md). For an axial point source a distance $s$ before the object and an observer a distance $r$ after it, the [phase](../../../../../phase-waves.md) uses the effective distance $z_{\rm eff}=sr/(s+r)$, because both incident and outgoing spherical paths contribute curvature. Scalar, paraxial propagation and an opening large compared with wavelength are assumed throughout.

**A circular hole in the far field gives an Airy pattern.** For uniform plane illumination the field is the two-dimensional [Fourier transform](../../../../../fourier-transform-split.md) of the [aperture](../../../../../aperture.md). In polar coordinates, let $Q=k\sin\theta$; the angular integral gives the [Bessel function](../../../../../bessel-function-split.md) $J_0$:

$$
U(\theta)\propto\int_0^a r\,dr\int_0^{2\pi}e^{-iQr\cos\phi}\,d\phi
=2\pi\int_0^a rJ_0(Qr)\,dr
=\pi a^2\frac{2J_1(Qa)}{Qa}.
$$

Thus

$$
\boxed{\frac{I(\theta)}{I(0)}=\left[\frac{2J_1(ka\sin\theta)}{ka\sin\theta}\right]^2}.
$$

The limiting central value is one because $J_1(u)\simeq u/2$ near zero. A bright central [Airy disk](../../../../../airy-disk.md) is surrounded by progressively weaker concentric rings. The first dark ring has $ka\sin\theta=3.8317$, or $\sin\theta\simeq1.22\lambda/D$ with diameter $D=2a$. This scale gives the [Rayleigh criterion](../../../../../rayleigh-criterion.md) for a circular optical instrument. Larger [apertures](../../../../../aperture.md) narrow the angular pattern; a lens of focal length $f$ maps the first dark ring to radius $1.22\lambda f/D$ in its focal plane.

**In the Fresnel regime, the axial intensity oscillates as [aperture](../../../../../aperture.md) size or distance changes.** [Fresnel half-period zones](../../../../../fresnel-half-period-zone.md) have boundaries at path excesses $m\lambda/2$ and approximately opposite phases in successive zones. For a plane wave, their radii obey $r_m^2=m\lambda z$. A circular opening can therefore expose alternating constructive and cancelling zone contributions. More precisely, [Fresnel diffraction by a circular aperture](../../../../../fresnel-diffraction-by-a-circular-aperture.md) gives, normalized by the unobstructed field,

$$
\frac{U_a(0)}{U_0}=\frac{2\pi}{i\lambda z}\int_0^a r\exp\!\left(\frac{i\pi r^2}{\lambda z}\right)dr
=1-e^{i\pi N_F},\qquad
\boxed{\frac{I_a(0)}{I_0}=4\sin^2\!\left(\frac{\pi N_F}{2}\right)}.
$$

An odd integer number of zones gives a bright axial point with ideal intensity $4I_0$; an even number gives an axial zero. Intensity can locally exceed the unobstructed value because interference redistributes [energy](../../../../../energy-split.md); total transmitted [power](../../../../../power.md) still obeys [conservation of energy](../../../../../conservation-of-energy.md). The relative normalisation here differs from the Airy expression, which normalises each far-field pattern by its own central intensity.

Off axis, the circular Fresnel field is

$$
\frac{U_a(\rho)}{U_0}=\frac{2\pi}{i\lambda z}e^{ik\rho^2/(2z)}
\int_0^a r\,e^{ikr^2/(2z)}J_0(k\rho r/z)\,dr.
$$

Its concentric structure evolves with $N_F$ and includes fringes near the geometrical edge. The axial zone argument does not determine the complete off-axis pattern.

**Complementary holes and opaque disks are related at the field level.** [Babinet's principle](../../../../../babinet-s-principle.md) states $U_a+U_d=U_0$ for complementary [aperture](../../../../../aperture.md) and disk transmissions under the same illumination. In the Fraunhofer region away from the direct transmitted beam, the background field is absent and the diffracted fields are opposite in sign. Their scattered intensity profiles therefore have the same Airy angular dependence. Exactly in the forward direction the unobstructed field must be retained; subtracting intensities is incorrect. Finite incident beams also give a finite-width direct beam rather than an ideal angular delta function.

For [Fresnel diffraction by an opaque disk](../../../../../fresnel-diffraction-by-an-opaque-disk.md), the axial complement is particularly striking:

$$
\frac{U_d(0)}{U_0}=1-\frac{U_a(0)}{U_0}=e^{i\pi N_F},\qquad
\boxed{I_d(0)=I_0}.
$$

The ideal circular disk has an [Arago spot](../../../../../arago-spot.md) at the centre of its geometric shadow. Circular edge contributions reach the axial point with the same [phase](../../../../../phase-waves.md). This does not mean the whole shadow is illuminated: off-axis cancellation produces the surrounding shadow and rings, and the axial spot becomes narrower for larger obstruction or shorter propagation distance. An [aperture](../../../../../aperture.md)'s axial intensity oscillates, while its complementary disk's axial intensity stays constant in this ideal paraxial model.

<a id="section-d/d12/image-original-computed-circular-diffraction-profiles-airy-far-field-and-fresnel-aperture-and-complementary-disk-intensities"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2-d12-circular-diffraction.png)

**[Figure 6](#section-d/d12/image-original-computed-circular-diffraction-profiles-airy-far-field-and-fresnel-aperture-and-complementary-disk-intensities). Original computed circular diffraction profiles: Airy far field and Fresnel aperture and complementary-disk intensities**.

A practical observation uses a compact coherent source, an accurately circular hole or disk, and an aligned screen or camera. Varying the propagation distance or [aperture](../../../../../aperture.md) radius reveals the transition between regimes. A point source, or spatial filtering, prevents different source positions from washing out the fine structure. Finite source size, incomplete coherence, edge roughness, misalignment, vector effects for wavelength-sized objects and lens aberrations reduce the ideal contrast. These experimental limitations explain why a geometrically unexpected axial bright point requires a suitable setup even though its scalar derivation is simple.

## ↑ Ancestors (14)

1. [D12](../d12.md)
2. [Section D](../../section-d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
