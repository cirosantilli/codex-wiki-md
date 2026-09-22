<h1 id="section-b/b8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [Fresnel diffraction](../../../../../../fresnel-diffraction.md), the propagation [wave phase](../../../../../../phase-waves.md) varies quadratically across the aperture and that curvature must be retained. For a transverse scale $w$ at propagation distance $L$, its size is of order $\pi w^2/(\lambda L)$. In [Fraunhofer diffraction](../../../../../../fraunhofer-diffraction.md), that quadratic term is negligible, approximately $w^2/(\lambda L)\ll1$, while the linear phase encoding the observation angle remains. A lens can also form the far-field angular pattern in its [focal plane](../../../../../../focal-plane.md).

For a normally incident [plane wave](../../../../../../plane-wave.md) and aperture transmission $h(x,y)$, the far-field [complex amplitude](../../../../../../complex-amplitude.md) is its [Fourier transform](../../../../../../fourier-transform-split.md):

$$
\psi(q_x,q_y)\propto\iint h(x,y)e^{-i(q_xx+q_yy)}\,dx\,dy,
\qquad q_x=\frac{2\pi}{\lambda}\sin\theta_x.
$$

The detected [light intensity](../../../../../../light-intensity.md) is proportional to $|\psi|^2$. For identical parallel slits, write the transmission as a sum of shifted copies of one slit. The [Fourier shift theorem](../../../../../../fourier-shift-theorem.md) gives one single-slit transform multiplied by the sum of positional [phase factors](../../../../../../phase-factor.md):

$$
\psi(q)\propto a\operatorname{sinc}(qa/2)\sum_j e^{-iqx_j},\qquad
\operatorname{sinc}u=\frac{\sin u}{u}.
$$

The [single-slit diffraction](../../../../../../single-slit-diffraction.md) envelope sets the broad scale, while coherent interference between slit centres produces the finer array pattern. One sums [complex amplitudes](../../../../../../complex-amplitude.md) before squaring, rather than adding independent slit intensities.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
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
