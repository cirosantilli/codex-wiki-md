<h1 id="section-b/b7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The expression is a [scalar diffraction theory](../../../../../../scalar-diffraction-theory.md) integral for a [monochromatic wave](../../../../../../monochromatic-wave.md). The complex quantity $\psi_P$ represents a field [complex amplitude](../../../../../../complex-amplitude.md), with physical field obtained by taking the real part after multiplication by $e^{-i\omega t}$. The [light intensity](../../../../../../light-intensity.md) is proportional to $|\psi_P|^2$. The coordinates $x,y$ label transverse positions in the aperture plane, $\Sigma$ is its transmitting region, and $h(x,y)$ is the incident field multiplied by the aperture's complex transmission. The [wavenumber](../../../../../../wavenumber.md) is $k=2\pi/\lambda$ in the propagation medium, and $R$ is the axial propagation distance if $h$ already includes the incident field.

To derive the [Fresnel diffraction](../../../../../../fresnel-diffraction.md), start from [Huygens-Fresnel principle](../../../../../../huygens-fresnel-principle.md) contributions with propagation factor $e^{iks}/s$. With the coordinate origin at the projection of $P$ into the aperture plane,

$$
s=\sqrt{R^2+x^2+y^2}=R+\frac{x^2+y^2}{2R}-\frac{(x^2+y^2)^2}{8R^3}+\cdots.
$$

The [paraxial approximation](../../../../../../paraxial-approximation.md) requires $\rho/R\ll1$, where $\rho^2=x^2+y^2$. Replace the slowly varying $1/s$ and the obliquity factor by their axial values, but retain the quadratic variation of [wave phase](../../../../../../phase-waves.md). Neglect of the next [wave phase](../../../../../../phase-waves.md) term requires $k\rho^4/(8R^3)\ll1$ over the relevant aperture. Thus, apart from a common constant,

$$
\psi_P\simeq\frac{e^{ikR}}{i\lambda R}\iint_\Sigma h(x,y)e^{ik(x^2+y^2)/(2R)}\,dx\,dy.
$$

The quadratic [wave phase](../../../../../../phase-waves.md) may be of order one or much larger; setting it to zero would require the stronger conditions for [Fraunhofer diffraction](../../../../../../fraunhofer-diffraction.md). The scalar treatment also neglects the detailed vector field at aperture edges and assumes dimensions large enough compared with [wavelength](../../../../../../wavelength.md) for this approximation to be useful.

For a finite-distance axial point source at distance $p$ and an observer at distance $q$, the incident field contributes its own quadratic [wave phase](../../../../../../phase-waves.md). If $h$ instead denotes only the aperture transmission, the combined curvature is described by an effective distance

$$
\boxed{\frac1{R_{\rm eff}}=\frac1p+\frac1q,\qquad R_{\rm eff}=\frac{pq}{p+q}.}
$$

These are two equivalent conventions for distributing the incident [wave phase](../../../../../../phase-waves.md) between $h$ and the exponential. Both distances must be included in the later calculation.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [B7](../../b7.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
