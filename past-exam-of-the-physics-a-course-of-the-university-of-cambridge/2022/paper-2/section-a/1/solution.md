<h1 id="section-a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [Fresnel diffraction](../../../../../fresnel-diffraction.md), since the detector moves along the axis through successive near-field [interference](../../../../../interference-wave-propagation.md) extrema. Write $z$ for its distance from the opening and $\rho$ for the integration coordinate within the opening. For a uniform incident [plane wave](../../../../../plane-wave.md), the on-axis [complex amplitude](../../../../../complex-amplitude.md), in the [paraxial approximation](../../../../../paraxial-approximation.md), is proportional to

$$
\frac{e^{ikz}}{i\lambda z}\int_0^r e^{i\pi\rho^2/(\lambda z)}2\pi\rho\,d\rho
=e^{ikz}\left(1-e^{i\pi r^2/(\lambda z)}\right).
$$

Thus the [light intensity](../../../../../light-intensity.md) relative to the incident value is

$$
\frac{I(z)}{I_{\rm inc}}=4\sin^2\left(\frac{\pi r^2}{2\lambda z}\right).
$$

The [Fresnel number](../../../../../fresnel-number.md) $F=r^2/(\lambda z)$ is an odd integer at a maximum and an even integer at a minimum. It decreases as the detector moves away. Adjacent extrema therefore differ by one:

$$
\frac{r^2}{\lambda}\left(\frac1{1.00\,\mathrm m}-\frac1{1.25\,\mathrm m}\right)=1.
$$

Consequently

$$
\boxed{r^2=2.25\times10^{-6}\,\mathrm{m^2},\qquad r=1.50\times10^{-3}\,\mathrm m=1.50\,\mathrm{mm}.}
$$

As a check, $F=5$ at $z=1\,\mathrm m$ and $F=4$ at $z=1.25\,\mathrm m$, so these are indeed a maximum followed by the next minimum. Also $r/z\simeq1.5\times10^{-3}$, consistent with the [paraxial approximation](../../../../../paraxial-approximation.md).

## ↑ Ancestors (14)

1. [1](../1.md)
2. [Section A](../../section-a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
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
