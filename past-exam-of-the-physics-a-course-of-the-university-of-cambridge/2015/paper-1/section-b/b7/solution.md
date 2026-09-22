<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

**Stationary states.** Inside the [infinite square well](../../../../../infinite-square-well.md), the [time-independent Schrödinger equation](../../../../../time-independent-schrodinger-equation.md) has sinusoidal solutions. The [boundary conditions](../../../../../boundary-condition.md) $\phi(0)=\phi(a)=0$ select $k_na=n\pi$; normalization then gives

$$
\boxed{\phi_n(x)=\sqrt{\frac2a}\sin\frac{n\pi x}{a},\quad
E_n=\frac{n^2\pi^2\hbar^2}{2ma^2}},\qquad n=1,2,\ldots.
$$

Each [wavefunction](../../../../../wave-function-split.md) vanishes outside the well. There is no nonzero $n=0$ state.

**Immediate [energy](../../../../../energy-split.md) measurement after expansion.** For the [one-sided sudden expansion of an infinite square well](../../../../../one-sided-sudden-expansion-of-an-infinite-square-well.md), take the original wall at $x=0$ as fixed, so the expanded well occupies $0<x<2a$. In the [sudden approximation](../../../../../sudden-approximation.md), the initial [wavefunction](../../../../../wave-function-split.md) remains $\sqrt{2/a}\sin(\pi x/a)$ on $0<x<a$, extended by zero elsewhere. The new [ground state](../../../../../ground-state.md) is $\chi_1=a^{-1/2}\sin(\pi x/(2a))$. Its [probability amplitude](../../../../../probability-amplitude.md) is

$$
c_1=\frac{\sqrt2}{a}\int_0^a\sin\frac{\pi x}{a}\sin\frac{\pi x}{2a}\,dx
=\frac{4\sqrt2}{3\pi}.
$$

The [Born rule](../../../../../born-rule.md) therefore gives

$$
\boxed{P_1=|c_1|^2=\frac{32}{9\pi^2}=0.36025}.
$$

The motion of the walls matters: a symmetric expansion about the old midpoint would instead give $64/(9\pi^2)$. The stated width alone does not explicitly identify the final endpoints. The first result uses the natural continuation of the specified left boundary; if both boundaries are moved, the final location must be supplied. For a new well $(b,b+2a)$ containing $(0,a)$, the overlap is $c_1(b)=(4\sqrt2/(3\pi))[\cos(\pi b/(2a))-\sin(\pi b/(2a))]$.

**Evolution of one [energy eigenstate](../../../../../energy-eigenstate.md).** For a time-independent [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md), write $|\psi(t)\rangle=f(t)|\phi_n\rangle$. Substitution into the [Time-dependent Schrödinger equation](../../../../../time-dependent-schrodinger-equation.md) gives $i\hbar \dot f=E_nf$, so

$$
\boxed{|\psi(t)\rangle=e^{-iE_nt/\hbar}|\phi_n\rangle}.
$$

Only a [global phase](../../../../../global-phase.md) changes, leaving all measurement [probabilities](../../../../../probability.md) unchanged.

**Delayed [energy](../../../../../energy-split.md) measurement.** Expand the unchanged initial state in the complete new [energy](../../../../../energy-split.md) [eigenbasis](../../../../../eigenbasis.md),

$$
\psi(x,t)=\sum_{n=1}^\infty c_n\chi_n(x)e^{-iE_n't/\hbar},
\quad \chi_n=\frac1{\sqrt a}\sin\frac{n\pi x}{2a},
\quad E_n'=\frac{n^2\pi^2\hbar^2}{8ma^2}.
$$

For the fixed-left-wall geometry, direct overlap integration gives

$$
c_2=\frac1{\sqrt2},\qquad
c_n=\frac{4\sqrt2\sin(n\pi/2)}{\pi(4-n^2)}\quad(n\ne2).
$$

[orthogonality](../../../../../orthogonal-vectors.md) isolates the new ground-state amplitude as $c_1e^{-iE_1't/\hbar}$. Its phase cancels on squaring, so **the ground-state [probability](../../../../../probability.md) remains $32/(9\pi^2)$ for every delay**, provided the expanded well remains fixed and no intervening measurement or environment changes the state. The position [probability density](../../../../../probability-density.md) generally evolves because different [eigenstates](../../../../../eigenstate.md) acquire different relative phases.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
