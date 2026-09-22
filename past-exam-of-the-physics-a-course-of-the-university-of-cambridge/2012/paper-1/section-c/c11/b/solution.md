<h1 id="section-c/c11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Time-dependent Schrödinger equation](../../../../../../time-dependent-schrodinger-equation.md) $i\hbar\partial_t|\psi\rangle=H(t)|\psi\rangle$ governs unitary evolution of a closed system. If $H$ is independent of time, expand in its [energy eigenstates](../../../../../../energy-eigenstate.md):

$$
\boxed{|\psi(t)\rangle=\sum_n c_ne^{-iE_nt/\hbar}|n\rangle}.
$$

An individual [energy eigenstate](../../../../../../energy-eigenstate.md) changes only by a [phase](../../../../../../phase-waves.md), so its [probability density](../../../../../../probability-density.md) and time-independent-observable expectations are stationary. Superpositions can have interference terms oscillating at $(E_n-E_m)/\hbar$; fixed [energy](../../../../../../energy-split.md) populations do not imply that every [observable](../../../../../../observable.md) is constant.

For general $H(t)$, $U(t,t_0)=\mathcal T\exp[-(i/\hbar)\int H(t')dt']$ requires [time ordering](../../../../../../time-ordering.md) unless [Quantum Hamiltonians](../../../../../../hamiltonian-quantum-mechanics.md) at different times commute. The equivalent Heisenberg description evolves [observables](../../../../../../observable.md) rather than the state, giving $d\langle A\rangle/dt=(i/\hbar)\langle[H,A]\rangle+\langle\partial_tA\rangle$. Explicit time dependence can transfer [energy](../../../../../../energy-split.md) from an applied perturbation.

For a weak perturbation $V(t)$ to a known $H_0$, the first-order transition amplitude from $n$ to $m\ne n$ is

$$
c_m^{(1)}(t)=-\frac i\hbar\int_{t_0}^t\langle m|V(t')|n\rangle e^{i(E_m-E_n)t'/\hbar}\,dt'.
$$

Its squared modulus gives the leading transition [probability](../../../../../../probability.md) while depletion remains small. A nearly monochromatic perturbation emphasizes [energy](../../../../../../energy-split.md) differences near its quantum of [frequency](../../../../../../frequency.md); a continuum and suitable long-time limit yield [Fermi's golden rule](../../../../../../fermi-s-golden-rule.md). These approximations have stated weak-coupling and time-resolution limits; they do not replace exact unitary dynamics in every regime.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [C11](../../c11.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2012](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
