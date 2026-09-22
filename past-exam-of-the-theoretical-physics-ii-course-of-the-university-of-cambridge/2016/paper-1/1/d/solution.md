<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define $\alpha=\hbar T/(2I)$. The free [propagator](../../../../../propagator.md) acts diagonally on each angular harmonic:

$$
U_Te^{im\theta}=e^{-i\alpha m^2}e^{im\theta}.
$$

The kick multiplies by the Jacobi-Anger series

$$
e^{i\eta\cos\theta}=\sum_{\ell\in\mathbb Z}i^\ell J_\ell(\eta)e^{i\ell\theta}.
$$

Multiply the two series and collect the output harmonic $n=m+\ell$. The one-step coefficient update is

$$
\boxed{c_n(t+T)=\sum_{m\in\mathbb Z}
i^{\,n-m}J_{n-m}(\eta)e^{-i\alpha m^2}c_m(t),}
$$

where both sampling times are just after their respective kicks. Free evolution supplies the input-index [phase](../../../../../phase-waves.md) before the kick mixes angular momenta.

The source uses the unnormalized basis functions $e^{im\theta}$. Thus a unit-norm [wavefunction](../../../../../wave-function-split.md) satisfies $2\pi\sum_m|c_m|^2=1$. If the basis is instead $e^{im\theta}/\sqrt{2\pi}$, its amplitudes have sum of squared moduli one and obey the same [matrix](../../../../../matrix.md) update. Mixing these normalization conventions would change an energy expectation incorrectly.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
