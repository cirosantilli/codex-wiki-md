<h1 id="section-b/b8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put the slit centres at $x_j=\pm D/2,\pm3D/2$. Each slit has the same width $a$ and illumination. Its contribution to the [Fraunhofer diffraction](../../../../../../fraunhofer-diffraction.md) [complex amplitude](../../../../../../complex-amplitude.md) is

$$
\int_{x_j-a/2}^{x_j+a/2}e^{-iqx}\,dx
=a\operatorname{sinc}(qa/2)e^{-iqx_j}.
$$

The four [phase factors](../../../../../../phase-factor.md) pair into cosines:

$$
\sum_j e^{-iqx_j}=e^{iqD/2}+e^{-iqD/2}+e^{3iqD/2}+e^{-3iqD/2}
=2\cos(qD/2)+2\cos(3qD/2).
$$

Therefore the [four-slit Fraunhofer diffraction](../../../../../../four-slit-fraunhofer-diffraction.md) field is

$$
\boxed{\psi(q)\propto2a[\cos(qD/2)+\cos(3qD/2)]\operatorname{sinc}(qa/2),\qquad
q=\frac{2\pi\sin\theta}{\lambda}.}
$$

The common factor $2a$ can be absorbed in the proportionality constant, giving the requested form. In particular $\psi(0)\propto4a$, as expected from four equal in-phase slits. Normalizing by the central intensity gives

$$
\boxed{\frac{I(q)}{I(0)}=\operatorname{sinc}^2(qa/2)\cos^2(qD/2)\cos^2(qD).}
$$

The last form follows from $\cos x+\cos3x=2\cos2x\cos x$ and avoids apparent singularities in the usual sine-ratio array formula.

## ↑ Ancestors (15)

1. [B](../b.md)
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
