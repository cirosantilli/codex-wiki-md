<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

Take the [aperture](../../../../../aperture.md) in $z=0$ and the observation point $P=(0,0,b)$, with $b>0$. Under [scalar diffraction theory](../../../../../scalar-diffraction-theory.md), the [Huygens-Fresnel principle](../../../../../huygens-fresnel-principle.md) sums [complex amplitudes](../../../../../complex-amplitude.md) from area elements, rather than summing their [intensities](../../../../../intensity-physics.md). Apart from a common normalization,

$$
\psi(P)\propto\iint h(x,y)K(\theta)\frac{e^{ikR}}R\,dx\,dy,
\qquad R=\sqrt{b^2+x^2+y^2},\quad k=2\pi/\lambda.
$$

Here $h$ is the complex [aperture](../../../../../aperture.md) transmission, $b$ is the axial distance, and $\theta$ is the angle of the secondary ray to the [aperture](../../../../../aperture.md) normal. The [obliquity factor](../../../../../obliquity-factor.md) $K$ describes the direction dependence of the secondary contribution; one Kirchhoff convention is $K=(1+\cos\theta)/2$ for normal illumination. Other scalar boundary approximations have slightly different angular weights, all tending to unity near the axis.

Put $r^2=x^2+y^2$. The [paraxial approximation](../../../../../paraxial-approximation.md) gives $R\simeq b+r^2/(2b)$ in the phase and $1/R\simeq1/b$ in the amplitude. Removing common $e^{ikb}/b$ yields

$$
\boxed{\psi(P)\propto\iint h(x,y)K(\theta)
\exp\left[\frac{i\pi(x^2+y^2)}{\lambda b}\right]dx\,dy.}
$$

Assumptions are uniform normally incident plane-wave illumination, coherent monochromatic propagation, [aperture](../../../../../aperture.md) dimensions large enough for the scalar description, $r/b\ll1$, and phase accuracy $kr^4/(8b^3)\ll1$ over the relevant [aperture](../../../../../aperture.md). The last condition justifies dropping the quartic distance term; geometric smallness alone does not guarantee phase accuracy.

<a id="section-b/b8/image-axial-fresnel-geometry-and-phasor-addition-with-alternate-half-period-zones-blocked"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-2-fresnel-zones.png)

**[Figure 2](#section-b/b8/image-axial-fresnel-geometry-and-phasor-addition-with-alternate-half-period-zones-blocked). Axial Fresnel geometry and phasor addition with alternate half-period zones blocked**.

For a circular [aperture](../../../../../aperture.md), $h=1$ for $r\leq a$ and zero elsewhere. Rotational symmetry and $s=r^2$ give $dx\,dy=r\,dr\,d\varphi$, $r\,dr=ds/2$, and

$$
\psi\propto2\pi\int_0^a K(\theta)e^{i\pi r^2/(\lambda b)}r\,dr
=\pi\int_0^{a^2}K(\theta)e^{i\pi s/(\lambda b)}ds.
$$

The constant $\pi$ can be absorbed into the proportionality factor, producing the required one-dimensional [integral](../../../../../integral-split.md).

At a focus a distance $f$ away, half-period-zone boundaries obey

$$
\sqrt{f^2+r_n^2}-f=\frac{n\lambda}{2},\qquad
r_n^2=n\lambda f+\frac{n^2\lambda^2}{4}\simeq n\lambda f.
$$

With slowly varying obliquity and illumination, each zone has almost the same area and its integrated [phasor](../../../../../phasor.md) has the opposite sign to its neighbour. A [zone plate](../../../../../zone-plate.md) blocks alternate zones, so the remaining [phasors](../../../../../phasor.md) add instead of nearly cancelling. Choosing an open central zone, the first three open regions have outer boundaries $n=1,3,5$:

$$
\boxed{r_1=0.100\,\mathrm{mm},\qquad r_3=0.173\,\mathrm{mm},\qquad r_5=0.224\,\mathrm{mm}.}
$$

These are outer radii, not zone widths; the second open region is the annulus between $r_2$ and $r_3$.

For the specified outer radius, $R^2/(\lambda f)=49$: there are approximately 49 half-period zones, of which 25 odd zones are open. Normalize to the field $\psi_0$ of the unobstructed [plane wave](../../../../../plane-wave.md). The normalized Fresnel [aperture](../../../../../aperture.md) [integral](../../../../../integral-split.md) is

$$
\frac{\psi}{\psi_0}=\frac{1}{i\lambda f}\int h\,e^{i\pi r^2/(\lambda f)}dA.
$$

For any odd open annulus this gives $2$, so the whole plate gives $\psi/\psi_0\simeq50$ and

$$
\boxed{I_{\rm focus}/I_{\rm unobstructed}\simeq4(25)^2=2.50\times10^3.}
$$

The [axial intensity gain of an amplitude zone plate](../../../../../axial-intensity-gain-of-an-amplitude-zone-plate.md) grows as the square of the number of open zones. Treating the number of zones continuously gives $49^2\simeq2.40\times10^3$, the same accuracy as an estimate. This large local [intensity](../../../../../intensity-physics.md) gain is consistent with [conservation of energy](../../../../../conservation-of-energy.md) because light is concentrated into a small focal spot. It is not a [power](../../../../../power.md) efficiency; the ideal first-order [power](../../../../../power.md) efficiency of a binary amplitude [zone plate](../../../../../zone-plate.md) is only $1/\pi^2$.[X-Ray Data Booklet, §4.4, first-order efficiency paragraph](../../../../../zone-plates-by-janos-kirz-and-david-attwood.md)

“Without the [zone plate](../../../../../zone-plate.md)” has here meant removing the finite plate and its outer stop, giving the unobstructed incident [wave](../../../../../wave-split.md). If instead a clear circular [aperture](../../../../../aperture.md) of radius $R$ is retained, its axial field is $\psi_{\rm clear}/\psi_0=1-e^{i49\pi}=2$, so **the ratio to that finite-aperture reference is $2500/4=625$**. The two reference experiments differ; neither ratio should be confused with total transmitted [power](../../../../../power.md).

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
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
