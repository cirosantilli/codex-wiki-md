<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First lift the angle to the real line. The [time-sliced configuration-space path integral](../../../../../time-sliced-configuration-space-path-integral.md) for a free coordinate with inertia I has kinetic action $\int dt\,I\dot\phi^2/2$. The rotor kernel sums lifted endpoints separated by $\phi_F-\phi_I+2\pi m$, because all such endpoints represent the same final angle on the circle.

Continue real time as $t=-i\hbar\tau$. Then $e^{-iHt/\hbar}=e^{-H\tau}$ and the end of the thermal interval is $\tau=\beta$, in inverse-energy units. Thus

$$
\frac{S_E}{\hbar}=\frac{I}{2\hbar^2}\int_0^\beta d\tau\,\dot\phi^2.
$$

The [trace](../../../../../matrix-trace.md) integrates the initial angle over one copy of the circle, not the whole lifted line. It yields the [rotor winding-sector path integral](../../../../../rotor-winding-sector-path-integral.md)

$$
\boxed{Z=\int_0^{2\pi}d\phi\sum_{m\in\mathbb Z}
\int_{\phi(0)=\phi}^{\phi(\beta)=\phi+2\pi m}\mathcal D\phi\,
\exp\left[-\frac{I}{2\hbar^2}\int_0^\beta d\tau\,\dot\phi^2\right].}
$$

The integer m is temporal [winding number](../../../../../winding-number.md), not the angular-momentum label n. Locally the measure has the free-kernel normalization $[I/(2\pi\hbar^2\Delta\tau)]^{1/2}$ per time slice. Summing topological sectors and retaining this normalization are necessary for the correct thermal trace.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
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
