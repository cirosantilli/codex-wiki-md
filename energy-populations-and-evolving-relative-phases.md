# Energy populations and evolving relative phases

↑ **Parent:** [Time-evolution operator](time-evolution-operator.md)

Suppose a constant [Hamiltonian operator](hamiltonian-quantum-mechanics.md) has a complete discrete [orthonormal basis](orthonormal-basis.md) of [energy eigenstates](energy-eigenstate.md), $H|n\rangle=E_n|n\rangle$. Expanding an initial [pure state](pure-state.md) and applying the [time-evolution operator](time-evolution-operator.md) term by term gives

$$
|\psi(0)\rangle=\sum_n c_n|n\rangle,\qquad
|\psi(t)\rangle=\sum_n c_ne^{-iE_nt/\hbar}|n\rangle.
$$

A [projective measurement](projective-measurement.md) resolving these [basis](basis.md) vectors therefore assigns the same [Born rule](born-rule.md) [probability](probability.md) $|c_n|^2$ to each label $n$ at every time. An [energy measurement](energy-measurement.md) groups labels sharing the same [energy eigenvalue](energy-eigenvalue-split.md): $P(E)=\sum_{n:E_n=E}|c_n|^2$ is also constant. If $c_m,c_n\ne0$, their [probability amplitude](probability-amplitude.md) ratio instead evolves as

$$
\frac{c_n(t)}{c_m(t)}=\frac{c_n}{c_m}
\exp\!\left[-\frac{i(E_n-E_m)t}{\hbar}\right].
$$

Only [energy](energy-split.md) differences enter this relative [quantum phase](quantum-phase.md). Adding a constant $\varepsilon I$ to the [Hamiltonian operator](hamiltonian-quantum-mechanics.md) multiplies the entire [pure state](pure-state.md) by $e^{-i\varepsilon t/\hbar}$, a [global phase](global-phase.md), and leaves the [density operator](density-matrix-split.md) unchanged.

For a fixed [observable](observable.md) $A$, the [expectation value](expectation-value.md) can nevertheless vary:

$$
\langle A\rangle_t=\sum_{m,n}c_m^*c_n
 e^{i(E_m-E_n)t/\hbar}\langle m|A|n\rangle.
$$

Terms joining distinct [energy eigenvalues](energy-eigenvalue-split.md) can oscillate; diagonal terms cannot. If $[A,H]=0$, these terms between different [energies](energy-split.md) vanish, so the [expectation value](expectation-value.md) is constant. This distinguishes [conservation of energy](conservation-of-energy.md) from the stronger claim that every [observable](observable.md) is stationary.

An [energy eigenstate](energy-eigenstate.md) has only a [global phase](global-phase.md) evolution and is a [stationary state](stationary-state.md). A [quantum superposition](quantum-superposition.md) entirely within one degenerate [energy eigenspace](energy-eigenspace.md) is also an [energy eigenstate](energy-eigenstate.md) and is stationary. For a general [density operator](density-matrix-split.md) in finite [dimension](dimension-vector-space.md), stationarity under a constant [Hamiltonian operator](hamiltonian-quantum-mechanics.md) means $[H,\rho]=0$: differentiating $U\rho U^\dagger$ proves necessity, and commuting $\rho$ through the exponential proves sufficiency. Merely fixing the diagonal energy populations does not fix the off-diagonal [quantum coherence](quantum-coherence-in-a-specified-basis.md).

**Table of contents**

- [Qubit precession under a constant Hamiltonian](qubit-precession-under-a-constant-hamiltonian.md)
  - [Ramsey interferometry](ramsey-interferometry.md)
    - [Initial-state dependence of Ramsey contrast](initial-state-dependence-of-ramsey-contrast.md)
    - [Ramsey ensemble coherence](ramsey-ensemble-coherence.md)
    - [Quantronium Ramsey interference experiment](quantronium-ramsey-interference-experiment.md)
    - [Ramsey separated oscillatory fields experiment](ramsey-separated-oscillatory-fields-experiment.md)
      - [Ramsey spectroscopy](ramsey-spectroscopy.md)
        - [Ramsey frequency precision](ramsey-frequency-precision.md)
      - [Finite-pulse Ramsey transition probability](finite-pulse-ramsey-transition-probability.md)
        - [Ramsey fringe envelope](ramsey-fringe-envelope.md)
        - [Finite-pulse Ramsey phase response](finite-pulse-ramsey-phase-response.md)
        - [Velocity-averaged Ramsey line](velocity-averaged-ramsey-line.md)

## ↑ Ancestors (10)

1. [Time-evolution operator](time-evolution-operator.md)
2. [Unitary time evolution](unitary-time-evolution.md)
3. [Hamiltonian (quantum mechanics)](hamiltonian-quantum-mechanics.md)
4. [Observable](observable.md)
5. [Quantum state](quantum-state.md)
6. [Quantum system](quantum-system-split.md)
7. [Quantum mechanics](quantum-mechanics-split.md)
8. [Branches of physics](branches-of-physics.md)
9. [Physics](physics-split.md)
10. [Codex Wiki](split.md)
