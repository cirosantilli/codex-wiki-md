<h1 id="33c/solution">Solution</h1>

↑ **Parent:** [33C](../33c.md)

The normalized [Bloch states](../../../../../bloch-state.md) $|k\rangle=N^{-1/2}\sum_{n=1}^Ne^{ikna}|n\rangle$ satisfy periodicity when $k=2\pi j/(Na)$. Acting with the hopping terms shifts the coefficients by one site, giving

$$
\boxed{H|k\rangle=(E_0-2J\cos ka)|k\rangle}.
$$

The first [Brillouin zone](../../../../../brillouin-zone.md) is a fundamental cell of reciprocal space, for example $[-\pi/a,\pi/a)$; [wavevectors](../../../../../wavevector.md) differing by $2\pi/a$ label the same state. It contains exactly $N$ distinct allowed [wavevectors](../../../../../wavevector.md) and hence $N$ orbital states. The written [Hamiltonian](../../../../../hamiltonian.md) has no spin index; if electron spin degeneracy is included there are $2N$ states.

For a narrow [wave packet](../../../../../wave-packet.md), [group velocity](../../../../../group-velocity.md) and band-curvature [effective mass](../../../../../band-effective-mass.md) are

$$
\boxed{v(k)=\frac{2Ja}{\hbar}\sin ka,
\qquad m^*(k)=\frac{\hbar^2}{2Ja^2\cos ka}}.
$$

For the usual $J>0$, the mass is negative in the outer half of the zone, $\pi/(2a)<|k|\le\pi/a$, taking one endpoint representative. At $|k|=\pi/(2a)$ the inverse mass vanishes and the mass diverges. For arbitrary nonzero $J$, the sign criterion is $J\cos ka<0$; $J=0$ is a flat band.

For electron charge $-e$ with $e>0$ in a constant [electric field](../../../../../electric-field.md) $\mathcal E$, the single-band semiclassical equations are $\hbar\dot k=-e\mathcal E$, $\dot x=v(k)$. Thus $k(t)=k_0-e\mathcal E t/\hbar$, and for $\mathcal E\ne0$,

$$
\boxed{x(t)-x_0=\frac{2J}{e\mathcal E}\left[\cos\left(k_0a-\frac{e\mathcal E a}{\hbar}t\right)-\cos k_0a\right]}.
$$

These are [Bloch oscillations](../../../../../bloch-oscillation.md) of period $2\pi\hbar/(|e\mathcal E|a)$. The zero-field limit is $x-x_0=v(k_0)t$. This assumes a narrow packet and neglects scattering and interband transitions.

For many electrons obeying the [Pauli exclusion principle](../../../../../pauli-exclusion-principle.md), a partially filled band has available nearby states and can carry current under a displaced occupation distribution: it describes a metal within band theory. A completely filled band has cancelling velocities over the zone, so its current is zero; if separated from empty higher bands by a nonzero gap, it describes an insulator at sufficiently low temperature and weak [electric field](../../../../../electric-field.md). With spin degeneracy this isolated band is filled at two electrons per site. The single-electron [Hamiltonian](../../../../../hamiltonian.md) alone does not specify the filling or a gap to a next band, so those extra physical assumptions are required for classifying a material.

## ↑ Ancestors (10)

1. [33C](../33c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
