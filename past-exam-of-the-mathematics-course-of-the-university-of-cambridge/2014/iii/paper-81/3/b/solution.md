<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The propagator is the quantum amplitude for evolving from one angular position to another. It evolves a wavefunction by $\Psi(\phi_F,t)=\int_0^{2\pi}d\phi_I\,K(\phi_F,\phi_I;t)\Psi(\phi_I,0)$. The [path integral](../../../../../../path-integral.md) weights each trajectory by $e^{iS/\hbar}$, with $S=\int dt\,I(\partial_t\phi)^2/2$. Since the configuration space is a circle, paths must include all possible lifts of the final angle to the real line.

Take $t=-i\hbar\beta$ by [Wick rotation](../../../../../../wick-rotation.md). Let $\tau=t_E/\hbar$, which runs from zero to $\beta$, and let the dot denote $d/d\tau$. The dimensionless Euclidean exponent is then $I\int_0^\beta\dot\phi^2d\tau/(2\hbar^2)$. Tracing the kernel identifies final and initial angles modulo $2\pi$, while the lift can change by $2\pi m$. Thus the [rotor winding-sector path integral](../../../../../../rotor-winding-sector-path-integral.md) is

$$
\boxed{\mathcal Z=\int_0^{2\pi}d\phi_0\sum_{m\in\mathbb Z}
\int_{\phi(0)=\phi_0}^{\phi(\beta)=\phi_0+2\pi m}\mathcal D\phi\,
\exp\left[-\frac{I}{2\hbar^2}\int_0^\beta d\tau\,\dot\phi^2\right].}
$$

The integration measure is fixed by the short-time free-rotor kernel. The dot on $\phi$ is essential; it is present in the PDF but lost in the TeX aid.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
