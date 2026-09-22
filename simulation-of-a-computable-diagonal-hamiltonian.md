# Simulation of a computable diagonal Hamiltonian

↑ **Parent:** [Hamiltonian simulation](hamiltonian-simulation.md)

Let $A|x\rangle=a(x)|x\rangle$, where a [reversible circuit](reversible-circuit.md) $C$ computes $a(x)$ into a clean register. Then applying $e^{-ita(x)}$ as a phase on that register and performing [uncomputation](uncomputation.md) implements $e^{-itA}$ on the data register. For $a(x)=(-1)^{f(x)}$, a Boolean output qubit suffices: $C^\dagger(I\otimes e^{-itZ})C$ acts as $e^{-itA}$ when that qubit starts in $|0\rangle$. This exact construction avoids a [Lie-Trotter product formula](lie-product-formula.md) because the eigenvalue is computed directly.

**Table of contents**

- [Pauli-string phase by parity computation](pauli-string-phase-by-parity-computation.md)

## ↑ Ancestors (5)

1. [Hamiltonian simulation](hamiltonian-simulation.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-58/4/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324/3/b/ii/solution.md)
- [Rotation about the z-axis](rotation-about-the-z-axis.md)
