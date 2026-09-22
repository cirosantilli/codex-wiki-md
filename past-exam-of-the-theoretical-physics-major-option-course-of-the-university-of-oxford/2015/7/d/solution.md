<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

On the unbounded line the momentum density of states in a reference length $L$ is $L\,dk/(2\pi)$. Count both signs of $k$, each with [zero-point energy](../../../../zero-point-energy.md) $|k|/2$ and the same frequency regulator:

$$
\boxed{E_0(L,\Lambda)=\frac L2\int_{-\infty}^\infty\frac{dk}{2\pi}|k|e^{-|k|/(\pi\Lambda)}
=\frac L{2\pi}\int_0^\infty dk\,ke^{-k/(\pi\Lambda)}
=\frac{\pi L\Lambda^2}{2}.}
$$

The extensive divergent term agrees exactly with [c](../c.md). Subtract it before taking the cutoff away:

$$
E_{\rm Cas}(L)=\lim_{\Lambda\to\infty}[E_0^{\rm BC}(L,\Lambda)-E_0(L,\Lambda)]
=-\frac\pi{24L}.
$$

The force tending to change the interval length is

$$
\boxed{F_L=-\frac{dE_{\rm Cas}}{dL}=-\frac\pi{24L^2},\qquad
F_L=-\frac{\pi\hbar c}{24L^2}\ \text{with units restored}.}
$$

Its negative sign means attraction: separating the boundaries increases this negative vacuum-energy difference toward zero. The bulk subtraction must be made before interpreting the force, otherwise differentiating an unphysical cutoff-dependent bulk energy would contaminate it.

This is the one-dimensional scalar Dirichlet **Casimir force**. The source's name “Casimir-Polder” normally refers to a retarded atom–atom or atom–surface dispersion force, whose geometry and power law differ. No atom polarizability or electromagnetic mode multiplicity enters the scalar result derived here.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
