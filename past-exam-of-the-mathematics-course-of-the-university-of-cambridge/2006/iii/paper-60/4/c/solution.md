<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the first two targets assume $N\ge5$, so the indexed levels exist. A possible [level population](../../../../../../quantum-state-population.md) reward is

$$
\boxed{\mathcal A_1[\rho]=\operatorname{Tr}(|5\rangle\langle5|\rho(10))=\rho_{55}(10).}
$$

It selects $\widehat A=|5\rangle\langle5|$ and $t_F=10$.

For the coherent target, use its rank-one [orthogonal projector](../../../../../../orthogonal-projection.md), not the sum of its two [level populations](../../../../../../quantum-state-population.md):

$$
\begin{aligned}
\widehat A_2&=|\Psi\rangle\langle\Psi|
=\frac12\big(|1\rangle\langle1|+|5\rangle\langle5|+i|1\rangle\langle5|-i|5\rangle\langle1|\big),\\
\mathcal A_2[\rho]&=\operatorname{Tr}(\widehat A_2\rho(100))
=\boxed{\frac12\big(\rho_{11}(100)+\rho_{55}(100)+2\operatorname{Im}\rho_{15}(100)\big)}.
\end{aligned}
$$

The imaginary [quantum coherence](../../../../../../quantum-coherence-in-a-specified-basis.md) term fixes the desired relative phase $-i$. Maximizing [level populations](../../../../../../quantum-state-population.md) alone would not select this superposition.

For energy, choose a specified final energy observable $H_F$:

$$
\boxed{\mathcal A_3[\rho]=\operatorname{Tr}(H_F\rho(t_F)).}
$$

For stored energy after the control is switched off, $H_F=H_0$ is the natural choice. If a fixed external field remains, use that known final [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) instead. If the terminal [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) itself is varied through the controls, the objective has explicit control dependence and additional terminal derivatives must be included. Each reward can be combined with the given dynamics and fluence penalty as $J_j=\mathcal A_j-\mathcal D-\mathcal C$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
