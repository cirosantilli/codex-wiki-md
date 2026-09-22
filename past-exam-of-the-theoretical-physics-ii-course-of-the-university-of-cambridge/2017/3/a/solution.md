<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a time-independent [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md), the [time-evolution operator](../../../../time-evolution-operator.md) is $U(T)=e^{-iHT/\hbar}$, with $T=t-t'$. Insert its resolution of identity in normalized [energy eigenstates](../../../../energy-eigenstate.md):

$$
\langle x|U(T)|x'\rangle
=\sum_\alpha\langle x|\alpha\rangle e^{-iE_\alpha T/\hbar}\langle\alpha|x'\rangle.
$$

Since $\langle x|\alpha\rangle=\varphi_\alpha(x)$, the retarded [quantum propagator](../../../../quantum-propagator.md) in the question is

$$
\boxed{K(x,t|x',t')=\Theta(T)\sum_\alpha\varphi_\alpha(x)\varphi_\alpha^*(x')e^{-iE_\alpha T/\hbar}.}
$$

The [Heaviside step function](../../../../heaviside-step-function.md) imposes the chosen retarded convention. If the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) has a [continuous spectrum](../../../../continuous-spectrum.md), the spectral sum includes its continuum integral; it must not be restricted to [bound states](../../../../bound-state.md). The [spectral resolution of a quantum propagator](../../../../spectral-resolution-of-a-quantum-propagator.md) also shows that $K$ tends to $\delta(x-x')$ as $T\downarrow0$. With the step factor it obeys $(i\hbar\partial_t-H)K=i\hbar\delta(T)\delta(x-x')$; the corresponding [Green function](../../../../green-s-function-split.md) with a unit delta source is $K/(i\hbar)$.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the theoretical physics II course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics II course of the University of Cambridge](../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
