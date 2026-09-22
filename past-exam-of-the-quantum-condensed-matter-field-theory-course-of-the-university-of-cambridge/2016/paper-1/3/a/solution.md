<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Keep the electromagnetic units of the supplied [Lagrangian](../../../../../lagrangian.md), including its factor $c$, and regard $e$ as the signed coupling used there. Set $a_B=e\Phi_B/(2\pi c)$. The [canonical momentum](../../../../../canonical-momentum.md) is $p_\phi=I\dot\phi+a_B$, so the [Legendre transform](../../../../../convex-conjugate.md) gives

$$
H=\frac{(p_\phi-a_B)^2}{2I},\qquad \boxed{\hat H=\frac1{2I}\left(-i\hbar\partial_\phi-\frac{e\Phi_B}{2\pi c}\right)^2.}
$$

Single-valued periodic wavefunctions have normalized eigenstates $e^{in\phi}/\sqrt{2\pi}$ with integer $n$. Defining dimensionless flux $f=e\Phi_B/(hc)$ gives $E_n=\hbar^2(n-f)^2/(2I)$, and the [trace](../../../../../matrix-trace.md) is therefore

$$
\boxed{Z=\sum_{n\in\mathbb Z}\exp\left[-\frac{\beta\hbar^2}{2I}(n-f)^2\right].}
$$

The [flux-threaded quantum rotor](../../../../../flux-threaded-quantum-rotor.md) spectrum is periodic under $f\mapsto f+1$ after relabelling $n$, corresponding to flux period $hc/|e|$ in these units. A local gauge change can remove the [magnetic vector potential](../../../../../magnetic-vector-potential.md) from the differential operator but then imposes a [twisted boundary condition](../../../../../twisted-boundary-condition.md) with phase $e^{-2\pi if}$; it cannot remove the flux dependence from both the [Hamiltonian](../../../../../hamiltonian.md) and boundary condition simultaneously. In SI conventions the flux coupling has no $c$, so one must not mix the two unit systems.

## ↑ Ancestors (14)

1. [A](../a.md)
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
