<h1 id="section-b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Start with the [Schrödinger equation](../../../../../schrodinger-equation.md) $i\hbar\partial_t|\psi\rangle=(H_0+V)|\psi\rangle$ and differentiate the definition of the [interaction picture](../../../../../interaction-picture.md) state:

$$
\begin{aligned}
i\hbar\frac{d}{dt}\left(e^{iH_0t/\hbar}|\psi\rangle\right)
&=-H_0e^{iH_0t/\hbar}|\psi\rangle
+e^{iH_0t/\hbar}(H_0+V)|\psi\rangle\\
&=e^{iH_0t/\hbar}Ve^{-iH_0t/\hbar}|\psi_I\rangle.
\end{aligned}
$$

The free [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) terms cancel because $H_0$ commutes with its own [matrix exponential](../../../../../matrix-exponential.md). Therefore

$$
\boxed{i\hbar\frac{d}{dt}|\psi_I(t)\rangle=V_I(t)|\psi_I(t)\rangle,
\qquad V_I(t)=e^{iH_0t/\hbar}V(t)e^{-iH_0t/\hbar}.}
$$

This [interaction picture](../../../../../interaction-picture.md) transformation is exact.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [4](../../4.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Physics course of the University of Cambridge](../../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
