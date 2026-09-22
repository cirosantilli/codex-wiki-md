# Collisional phase gate

↑ **Parent:** [Two-qubit gate](two-qubit-gate.md)

A [two-qubit gate](two-qubit-gate.md) in which an interaction shifts the [energy](energy-split.md) of a selected joint [computational basis](computational-basis.md) state and thereby accumulates a [relative quantum phase](relative-quantum-phase.md). With [Hamiltonian operator](hamiltonian-quantum-mechanics.md) $H=\Omega|01\rangle\langle01|$, where $\Omega$ has units of [energy](energy-split.md), an interaction time $\tau$ gives $U_\phi=\operatorname{diag}(1,e^{-i\phi},1,1)$ with $\phi=\Omega\tau/\hbar$. The selected basis state is part of the convention: this gate differs from the usual [Controlled-Z gate](controlled-z-gate.md) at $\phi=\pi$. Conjugation by a [Pauli X gate](pauli-x-gate.md) on the first [qubit](qubit.md) gives $(X\otimes I)U_\pi(X\otimes I)=\mathrm{CZ}$, because the conjugation interchanges $|01\rangle$ and $|11\rangle$.

## ↑ Ancestors (7)

1. [Two-qubit gate](two-qubit-gate.md)
2. [Quantum logic gate](quantum-logic-gate.md)
3. [Quantum circuit](quantum-circuit-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2005/7-and-8/8/1/solution.md)
