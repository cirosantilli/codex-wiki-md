# Quantum state ray

↑ **Parent:** [Quantum state](quantum-state.md)

A [quantum state ray](quantum-state-ray.md) is the [equivalence class](equivalence-class.md) of nonzero [vectors](vector.md) in a complex [Hilbert space](hilbert-space-split.md) under multiplication by a nonzero [complex number](complex-number.md). Its span is a one-dimensional [linear subspace](vector-subspace.md), but the zero [vector](vector.md) is not a state representative. A [unit vector](unit-vector.md) fixes the [norm](norm.md) and leaves a [global phase](global-phase.md) free. [Preskill, Foundations I: States and Ensembles, §2.1, printed p. 2, ray equivalence and normalized representatives](foundations-i-states-and-ensembles-by-john-preskill.md)

For a nonzero representative $|v\rangle$, the associated [pure state](pure-state.md) [density operator](density-matrix-split.md) is

$$
\rho_{[v]}=\frac{|v\rangle\langle v|}{\langle v|v\rangle}.
$$

Replacing $|v\rangle$ by $\lambda|v\rangle$ multiplies both numerator and denominator by $|\lambda|^2$, so the quotient is unchanged. In particular, for every [POVM](positive-operator-valued-measure.md) effect $E$,

$$
\langle e^{i\gamma}\psi|E|e^{i\gamma}\psi\rangle
=e^{-i\gamma}e^{i\gamma}\langle\psi|E|\psi\rangle
=\langle\psi|E|\psi\rangle.
$$

This proves that a [global phase](global-phase.md) changes no measurement [probability](probability.md). Changing the relative [quantum phase](quantum-phase.md) of two nonzero components can change the [density operator](density-matrix-split.md), as the following comparison shows.

## ↑ Ancestors (6)

1. [Quantum state](quantum-state.md)
2. [Quantum system](quantum-system-split.md)
3. [Quantum mechanics](quantum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2019/4/a/solution.md)
- [Quantum state](quantum-state.md)
- [Quantum state ray](quantum-state-ray.md)
- [Qubit precession under a constant Hamiltonian](qubit-precession-under-a-constant-hamiltonian.md)
