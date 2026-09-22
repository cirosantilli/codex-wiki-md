<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the [grand canonical ensemble](../../../../grand-canonical-ensemble.md), the system exchanges both [energy](../../../../energy-split.md) and particles with a reservoir at fixed [temperature](../../../../temperature-split.md) $T$ and [chemical potential](../../../../chemical-potential-split.md) $\mu$. The probability of a particular many-body [microstate](../../../../microstate.md) $i$, with [energy](../../../../energy-split.md) $E_i$ and [particle number](../../../../particle-number.md) $N_i$, is its [Boltzmann weight](../../../../boltzmann-factor.md) $e^{-\beta(E_i-\mu N_i)}$ divided by the [grand canonical partition function](../../../../grand-canonical-partition-function.md) $\Xi$, where $\beta=1/(k_BT)$. The denominator normalizes $\sum_i p_i=1$; a degeneracy is accounted for by counting distinct microstates, rather than changing an individual state's probability.

For noninteracting particles, specify a microstate by the [occupation numbers](../../../../occupation-number.md) $n_r$ of one-particle levels of [energy](../../../../energy-split.md) $\epsilon_r$. Then $E-\mu N=\sum_r(\epsilon_r-\mu)n_r$, so the Gibbs probability factorizes between levels. Put $x_r=e^{-\beta(\epsilon_r-\mu)}$.

For [fermions](../../../../fermion.md), the [Pauli exclusion principle](../../../../pauli-exclusion-principle.md) permits $n_r=0,1$ in each complete one-particle state, giving $\Xi_r=1+x_r$. Its mean occupancy is

$$
\boxed{\langle n_r\rangle=\frac{0+x_r}{1+x_r}
=\frac1{e^{\beta(\epsilon_r-\mu)}+1},}
$$

the [Fermi-Dirac distribution](../../../../fermi-dirac-distribution.md).

For [bosons](../../../../boson.md), $n_r=0,1,2,\ldots$, so the geometric sum is $\Xi_r=1/(1-x_r)$ when $x_r<1$. Differentiating that sum gives

$$
\boxed{\langle n_r\rangle=
\frac{\sum_{n=0}^\infty n x_r^n}{\sum_{n=0}^\infty x_r^n}
=\frac{x_r}{1-x_r}
=\frac1{e^{\beta(\epsilon_r-\mu)}-1},}
$$

the [Bose-Einstein distribution](../../../../bose-einstein-distribution.md). Finite-system convergence requires $\mu<\epsilon_{\min}$; condensation is the limiting approach to the lowest [energy](../../../../energy-split.md) with macroscopic ground-state occupation. Both quantum distributions reduce to $e^{-\beta(\epsilon_r-\mu)}$ when occupation is small. The quantities derived here are mean occupancies of states, rather than normalized probabilities over the set of one-particle energies.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../split.md)
5. [Thermal and Statistical Physics course of the University of Cambridge](../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
