# Berry-phase interference with a reference path

↑ **Parent:** [Berry phase](berry-phase.md)

An isolated [qubit](qubit.md) that acquires only a [global phase](global-phase.md) has unchanged measurement [probabilities](probability.md). To reveal the [Berry phase](berry-phase.md), use two coherent paths of a [Mach-Zehnder interferometer](mach-zehnder-interferometer.md), represented by a path [qubit](qubit.md). In one arm the internal [spin one-half](spin-one-half.md) [qubit](qubit.md) follows the loop; in the reference arm it stays in its starting [energy eigenstate](energy-eigenstate.md). Assume equal arm amplitudes, identical final internal states, cancelled relative [dynamical phases](dynamical-phase.md), and calibrated fixed apparatus phases. In the model above, hold the reference [Hamiltonian operator](hamiltonian-quantum-mechanics.md) at its initial value for the same duration. Both arms then have [energy eigenvalue](energy-eigenvalue-split.md) $-\Delta/2$ and acquire the same [dynamical phase](dynamical-phase.md) $\Delta T/(2\hbar)$, so their relative [dynamical phase](dynamical-phase.md) vanishes in the ideal limit of the [adiabatic theorem](adiabatic-theorem.md).

The joint [quantum state](quantum-state.md) before recombination then factors as

$$
\frac{|\mathrm{ref}\rangle+e^{i\gamma}|\mathrm{loop}\rangle}{\sqrt2}\otimes|\psi(\theta,0)\rangle.
$$

The [Berry phase](berry-phase.md) is now a relative [quantum phase](quantum-phase.md) between the two paths. The calibrated plus output projects onto $|+\rangle=(|\mathrm{ref}\rangle+|\mathrm{loop}\rangle)/\sqrt2$. The [Born rule](born-rule.md) gives

$$
P_+=\left|\frac{1+e^{i\gamma}}{2}\right|^2=\frac{1+\cos\gamma}{2},\qquad P_-=1-P_+.
$$

For the [Berry phase of a Bloch-sphere latitude](berry-phase-of-a-bloch-sphere-latitude.md), the plus-port [probabilities](probability.md) at $\theta=0,60^\circ,90^\circ,180^\circ$ are respectively $1,1/2,0,1$. This ideal [Mach-Zehnder interferometer](mach-zehnder-interferometer.md) measurement cannot distinguish $\gamma$ from $-\gamma$ or $\gamma+2\pi$ by itself; scanning a known reference phase can resolve the sign. An uncancelled relative [dynamical phase](dynamical-phase.md) would shift the fringe as well.

<a id="image-unwrapped-berry-phase-and-ideal-reference-path-interference-probability-for-latitude-loops"></a>
![](berry-phase-versus-loop-angle.png)

**[Figure 8](#image-unwrapped-berry-phase-and-ideal-reference-path-interference-probability-for-latitude-loops). Unwrapped Berry phase and ideal reference-path interference probability for latitude loops**.

## ↑ Ancestors (5)

1. [Berry phase](berry-phase.md)
2. [Quantum mechanics](quantum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Berry phase](berry-phase.md)
