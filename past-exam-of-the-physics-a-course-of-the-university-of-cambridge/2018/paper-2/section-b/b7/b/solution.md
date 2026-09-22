<h1 id="section-b/b7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the [aperture](../../../../../../aperture.md) occupy the $z=0$ plane, with coordinates $(x,y)$ and opening $\Sigma$. Write $\psi_\Sigma(x,y)$ for the incident scalar [complex amplitude](../../../../../../complex-amplitude.md) and $h(x,y)$ for its dimensionless amplitude transmission, including any imposed [phase](../../../../../../phase-waves.md). The observation point has transverse coordinates $(X,Y)$, corresponding to the PDF's $(x_0,y_0)$, and axial distance $R$. Also $k=2\pi/\lambda$ is the [wavenumber](../../../../../../wavenumber.md) and $i^2=-1$.

The [Huygens-Fresnel principle](../../../../../../huygens-fresnel-principle.md) expresses the propagated field, up to common prefactors and an approximately constant obliquity factor, as

$$
\psi_P\propto\iint_\Sigma \psi_\Sigma h\,\frac{e^{ikr}}r\,dx\,dy,\qquad
r=\sqrt{R^2+(X-x)^2+(Y-y)^2}.
$$

In the [paraxial approximation](../../../../../../paraxial-approximation.md), expand the path as

$$
r\simeq R+\frac{X^2+Y^2}{2R}-\frac{Xx+Yy}{R}+\frac{x^2+y^2}{2R}.
$$

The last term is negligible in the [Fraunhofer diffraction](../../../../../../fraunhofer-diffraction.md) limit, while the first two terms and $1/r\simeq1/R$ are common across the [aperture](../../../../../../aperture.md). Factoring them out leaves

$$
\boxed{\psi_P\propto\iint_\Sigma\psi_\Sigma(x,y)h(x,y)e^{-ik(Xx+Yy)/R}\,dx\,dy}.
$$

It is the two-dimensional [Fourier transform](../../../../../../fourier-transform-split.md) of the transmitted [aperture](../../../../../../aperture.md) field, evaluated at transverse [wavevector](../../../../../../wavevector.md) $(kX/R,kY/R)$. For appreciable observation angles the corresponding exact directional components are used rather than $X/R,Y/R$.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [B7](../../b7.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
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
