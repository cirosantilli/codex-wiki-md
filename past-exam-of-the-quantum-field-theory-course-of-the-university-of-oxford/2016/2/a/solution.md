<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\int_{\mathbf p}=\int d^3p/(2\pi)^3$ and $E_{\mathbf p}=\sqrt{\mathbf p^2+m^2}$. Insert the [mode expansion of a free field](../../../../mode-expansion-of-a-free-field.md) for each quantity into the [commutator](../../../../commutator.md). Only the mixed [creation operator](../../../../creation-operator.md) and [annihilation operator](../../../../annihilation-operator.md) terms survive. The [Dirac delta function](../../../../dirac-delta-function.md) in their [canonical commutation relation](../../../../canonical-commutation-relation.md) sets the two [momenta](../../../../momentum-split.md) equal, so the square-root factors multiply to $1/2$:

$$
[\phi(\mathbf x),\pi(\mathbf y)]
=\frac i2\int_{\mathbf p}\left[e^{i\mathbf p\cdot(\mathbf x-\mathbf y)}+e^{-i\mathbf p\cdot(\mathbf x-\mathbf y)}\right]
=\boxed{i\delta^3(\mathbf x-\mathbf y)}.
$$

In the second equality, each [Fourier transform](../../../../fourier-transform-split.md) is the same [Dirac delta function](../../../../dirac-delta-function.md), since the integration domain is invariant under $\mathbf p\mapsto-\mathbf p$. This is the equal-time [canonical commutation relation](../../../../canonical-commutation-relation.md). The analogous calculation gives $[\phi(\mathbf x),\phi(\mathbf y)]=[\pi(\mathbf x),\pi(\mathbf y)]=0$, because their two mixed terms have opposite signs.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
