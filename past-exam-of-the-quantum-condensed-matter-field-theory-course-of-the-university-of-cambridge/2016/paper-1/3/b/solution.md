<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [trace](../../../../../matrix-trace.md) integrates the diagonal thermal kernel over a single fundamental interval, $Z=\int_0^{2\pi}d\phi_0\,\langle\phi_0|e^{-\beta\hat H}|\phi_0\rangle$. On the circle a closed path can wind an integer number $m$ of times. Lift it to the real covering coordinate so its endpoints are $\phi(0)=\phi_0$ and $\phi(\mathcal T)=\phi_0+2\pi m$, with $\mathcal T=\hbar\beta$.

Under [Wick rotation](../../../../../wick-rotation.md) $t=-i\tau$, $\dot\phi=i\partial_\tau\phi$, so the real-time phase $iS/\hbar$ becomes minus the [Euclidean action](../../../../../euclidean-action.md) divided by $\hbar$, with

$$
\boxed{S_E[\phi]=\int_0^{\mathcal T}d\tau\left[\frac I2(\partial_\tau\phi)^2-i\frac{e\Phi_B}{2\pi c}\partial_\tau\phi\right].}
$$

Thus sum the [path integral](../../../../../path-integral.md) $e^{-S_E/\hbar}$ over these lifted endpoint conditions and integrate $\phi_0$ from zero to $2\pi$. This gives the requested winding-sector representation of the [trace](../../../../../matrix-trace.md). The flux term is a total derivative, so it leaves the local classical equation unchanged, but its weight is $e^{i2\pi fm}$ and distinguishes different winding sectors. This is the [Aharonov-Bohm phase](../../../../../aharonov-bohm-effect.md) in a thermal [path integral](../../../../../path-integral.md), rather than a force from a magnetic field on the ring itself.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../../quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
