<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**The printed identity has the wrong sign for the specified relative phase.** Differentiating the [energy](../../../../energy-split.md) found above and evaluating the [operator commutator](../../../../operator-commutator.md) give

$$
\frac{\partial E}{\partial\chi}=tN\sin(2\theta)\sin\chi,\qquad
[\hat H,\hat n_L]=t(\hat a_L^\dagger\hat a_R-\hat a_R^\dagger\hat a_L),\qquad
i\langle[\hat H,\hat n_L]\rangle=-tN\sin(2\theta)\sin\chi.
$$

Thus the [phase derivative of a two-mode condensate energy](../../../../phase-derivative-of-a-two-mode-condensate-energy.md) is

$$
\boxed{\frac{\partial E}{\partial\chi}=-i\langle[\hat H,\hat n_L]\rangle
=i\langle[\hat H,\hat n_R]\rangle.}
$$

A concrete counterexample to the printed sign is $N=100$, $\theta=\pi/4$, $\chi=\pi/2$ and $t>0$: its left side is $100t$, whereas its printed right side is $-100t$, independently of $w$ and $\mu$.

There is also a direct derivation without inserting the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md). Since $|\theta,\chi;N\rangle=e^{i\chi\hat n_R}|\theta,0;N\rangle$, differentiating this [unitary operator](../../../../unitary-operator.md) gives $\partial_\chi E=i\langle[\hat H,\hat n_R]\rangle$. Conservation of the total [particle number](../../../../particle-number.md), $[\hat H,\hat n_L+\hat n_R]=0$, then supplies the minus sign for the left well.

By the [Heisenberg equation of motion](../../../../heisenberg-equation-of-motion.md), $\hbar\,d\langle\hat n_L\rangle/dt=i\langle[\hat H,\hat n_L]\rangle$. Define the [bosonic Josephson junction](../../../../bosonic-josephson-junction.md) [particle current](../../../../particle-current.md) from left to right as $J_{L\to R}=-d\langle\hat n_L\rangle/dt$. The corrected identity means

$$
\boxed{J_{L\to R}=\frac1\hbar\frac{\partial E}{\partial\chi}
=\frac{tN}{\hbar}\sin(2\theta)\sin\chi.}
$$

The [energy](../../../../energy-split.md) slope with respect to the relative [phase](../../../../phase-waves.md) drives particle transfer; an extremum with respect to that [phase](../../../../phase-waves.md) has zero instantaneous [particle current](../../../../particle-current.md). The printed sign would work with $e^{-i\chi}$ in the right-well [orbital](../../../../single-particle-orbital.md), or with $[\hat n_L,\hat H]$ in place of $[\hat H,\hat n_L]$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the quantum matter course of the University of Oxford](../../../split.md)
5. [Quantum matter course of the University of Oxford](../../../../quantum-matter-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
