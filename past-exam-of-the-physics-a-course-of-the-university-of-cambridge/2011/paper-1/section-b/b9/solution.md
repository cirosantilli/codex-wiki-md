<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

The [wave impedance](../../../../../wave-impedance.md) is the travelling-wave field ratio $Z=E/H$; for the stated nonmagnetic media it is $Z_0/n$. A [reflection coefficient](../../../../../reflection-coefficient.md) is a reflected-to-incident [complex amplitude](../../../../../complex-amplitude.md) ratio with an explicitly chosen field orientation. With this [reflection-amplitude sign convention](../../../../../reflection-amplitude-sign-convention.md), using the question's formula for incidence inside silicon gives

$$
\boxed{r=\frac{Z_0/3.5-Z_0}{Z_0/3.5+Z_0}=-\frac59},\qquad R=|r|^2=\frac{25}{81}.
$$

With a common tangential electric-field direction, the usual electric-field [Fresnel equations](../../../../../fresnel-equations.md) instead give $r_E=(Z_2-Z_1)/(Z_2+Z_1)=+5/9$ for this incidence. The printed formula corresponds to the opposite reflected-field sign convention, for example the magnetic amplitude convention. It gives the same [reflectance](../../../../../reflectance.md) and the same round-trip factor $r^2$.

Each extra internal round trip multiplies the transmitted amplitude by $r^2e^{i\delta}$, with $\delta=4\pi nd/\lambda$. A [geometric series](../../../../../geometric-series.md) therefore gives

$$
A_{\rm out}=A_{\rm first}\sum_{j=0}^\infty(r^2e^{i\delta})^j=\frac{A_{\rm first}}{1-r^2e^{i\delta}},\qquad
\boxed{I\propto\frac1{1+R^2-2R\cos\delta}.}
$$

This is [Fabry–Pérot transmission from multiple reflections](../../../../../fabry-perot-transmission-from-multiple-reflections.md). Assuming lossless silicon with wavelength-independent $n$, the full [intensity](../../../../../intensity-physics.md) transmittance between air regions is

$$
T=\frac{(1-R)^2}{(1-R)^2+4R\sin^2(\delta/2)}.
$$

Maxima have $2nd/\lambda=j$, minima $2nd/\lambda=j+\tfrac12$. Here $2nd=7000\,\mathrm{nm}$, so within the specified tuning range the only maximum is **$1400\,\mathrm{nm}$**, and the two minima are **$1555.6\,\mathrm{nm}$** and **$1272.7\,\mathrm{nm}$**. The contrast is

$$
\boxed{\frac{I_{\max}}{I_{\min}}=\left(\frac{1+R}{1-R}\right)^2=\left(\frac{53}{28}\right)^2=3.583.}
$$

<a id="section-b/b9/image-transmission-contrast-and-resonance-narrowing-with-reflectivity"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1-etalon.png)

**[Figure 7](#section-b/b9/image-transmission-contrast-and-resonance-narrowing-with-reflectivity). Transmission contrast and resonance narrowing with reflectivity**. Original ideal lossless symmetric-etalon curves. The coating example uses chosen R=0.90, unchanged optical thickness and zero additional round-trip phase.

Identical highly reflecting coatings increase the [finesse](../../../../../finesse.md): transmission maxima become narrower and the [intensity](../../../../../intensity-physics.md) between them falls. Ideal symmetric lossless coatings retain $T_{\max}=1$; absorption or unequal mirrors reduce it. The illustrated maxima stay fixed only because additional reflection [wave phases](../../../../../phase-waves.md) are held unchanged. Real coating [wave phases](../../../../../phase-waves.md) can also shift the [resonances](../../../../../resonance.md).

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2011](../../../split.md)
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
