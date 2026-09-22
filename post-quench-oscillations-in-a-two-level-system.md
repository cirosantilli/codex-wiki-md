# Post-quench oscillations in a two-level system

↑ **Parent:** [Two-level sudden quench](two-level-sudden-quench.md)

After the [quantum quench](quantum-quench.md), hold $H_f$ fixed and evolve without an intervening [energy measurement](energy-measurement.md). The [unitary time evolution](unitary-time-evolution.md) is

$$
|\psi(t)\rangle=c\,e^{+i\Delta_ft/(2\hbar)}|g_f\rangle-s\,e^{-i\Delta_ft/(2\hbar)}|e_f\rangle.
$$

Projection onto the original $|0\rangle$ gives [probability amplitude](probability-amplitude.md) $c^2e^{+i\Delta_ft/(2\hbar)}+s^2e^{-i\Delta_ft/(2\hbar)}$. Squaring its [modulus](modulus.md) yields the [two-level quantum return probability](two-level-quantum-return-probability.md)

$$
P_0(t)=1-\sin^2\theta\sin^2\left(\frac{\Delta_ft}{2\hbar}\right),\qquad
P_1(t)=\sin^2\theta\sin^2\left(\frac{\Delta_ft}{2\hbar}\right).
$$

Their sum is one. For $\theta=\pi/3$, the first minimum of $P_0$ is $1/4$ at $t=\pi\hbar/\Delta_f$, and the return is complete at $T=2\pi\hbar/\Delta_f$. At $\theta=0$ or $\pi$ there is no oscillation, because the initial [quantum state](quantum-state.md) is already a final [energy eigenstate](energy-eigenstate.md).

<a id="image-post-quench-oscillations-and-constant-final-energy-populations-in-a-two-level-system"></a>
![](two-level-post-quench-oscillations.png)

**[Figure 4](#image-post-quench-oscillations-and-constant-final-energy-populations-in-a-two-level-system). Post-quench oscillations and constant final energy populations in a two-level system**. [Source](two-level-post-quench-oscillations.py). Original ideal calculation at $\theta=\pi/3$ with final gap $\Delta$. Original-basis [Born rule](born-rule.md) [probabilities](probability.md) oscillate through interference of the evolving relative [quantum phase](quantum-phase.md). Final [energy measurement](energy-measurement.md) [probabilities](probability.md) remain $3/4$ and $1/4$, so $\langle H_f\rangle=-\Delta/4$ is constant after the driven switch. Curves describe independent preparations measured at different times.

Changing measurement basis reveals the evolving relative [quantum phase](quantum-phase.md). Measuring the final [energy](energy.md) first instead destroys this [quantum coherence](quantum-coherence-in-a-specified-basis.md) between final [energy eigenstates](energy-eigenstate.md) in the unconditioned ensemble: its later original-basis return [probability](probability.md) is $c^4+s^4=1-\tfrac12\sin^2\theta$, equal to $5/8$ for this example. That constant differs from the oscillation of the unmeasured [pure state](pure-state.md). The [work](work.md) protocol and the oscillation protocol therefore use separate preparations.

## ↑ Ancestors (7)

1. [Two-level sudden quench](two-level-sudden-quench.md)
2. [Quantum quench](quantum-quench.md)
3. [Sudden approximation](sudden-approximation.md)
4. [Quantum mechanics](quantum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
