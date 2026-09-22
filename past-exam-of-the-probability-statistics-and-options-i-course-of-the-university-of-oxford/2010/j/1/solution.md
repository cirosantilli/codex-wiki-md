<h1 id="j/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a real potential, the [Time-dependent Schrödinger equation](../../../../time-dependent-schrodinger-equation.md) is

$$
i\hbar\partial_t\psi=-\frac{\hbar^2}{2m}\nabla^2\psi+V\psi.
$$

Multiply this equation by $\psi^*$, multiply its conjugate by $\psi$, and subtract. The potential terms cancel and the product rule converts the remaining terms into a divergence. Consequently

$$
\boxed{\partial_t|\psi|^2+\nabla\cdot\mathbf j=0,\qquad
\mathbf j=\frac{\hbar}{2mi}(\psi^*\nabla\psi-\psi\nabla\psi^*)
=\frac\hbar m\operatorname{Im}(\psi^*\nabla\psi).}
$$

This is the [probability current](../../../../probability-current.md) and its [continuity equation](../../../../continuity-equation.md).

Put $R(r)=\sin(kr)/r$. The supplied radial [Laplacian](../../../../laplacian.md) formula gives $\nabla^2R=-k^2R$ for $r>0$. Also $i\hbar\partial_t\psi=E\psi$. Therefore the free-particle equation is satisfied when

$$
\boxed{k=\sqrt{2mE}/\hbar.}
$$

The apparent singularity at zero is removable: $R(r)=k-k^3r^2/6+\cdots$ extends smoothly there and satisfies the same equation. Since $R$ is real and the time dependence is only a common phase, $\psi^*\nabla\psi=R\nabla R$ is real, so $\mathbf j=0$. The [density](../../../../density.md) $R^2$ is time-independent, proving the continuity equation explicitly. This is a standing spherical wave with zero net radial current.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [J](../../j.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
