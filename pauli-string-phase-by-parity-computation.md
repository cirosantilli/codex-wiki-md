# Pauli-string phase by parity computation

↑ **Parent:** [Simulation of a computable diagonal Hamiltonian](simulation-of-a-computable-diagonal-hamiltonian.md)

The [Pauli Z gates](pauli-z-gate.md) give [eigenvalue](eigenvalue.md) $(-1)^{\sum_jx_j}$ on $|x\rangle$. Use [parity computation by CNOT gates](parity-computation-by-cnot-gates.md) to put the [parity bit](parity-bit.md) in a zero ancilla, apply $e^{itZ}$ to it, and uncompute. The data acquire exactly $e^{it(-1)^{\sum_jx_j}}$, and the ancillary line returns to zero. This [compute-phase-uncompute construction](compute-phase-uncompute-construction.md) needs $2n+1$ one- and [two-qubit gates](two-qubit-gate.md). Accumulating parity into the last data line instead uses $2n-1$ gates without an extra ancilla. Neither implementation drops the global phase.

## ↑ Ancestors (6)

1. [Simulation of a computable diagonal Hamiltonian](simulation-of-a-computable-diagonal-hamiltonian.md)
2. [Hamiltonian simulation](hamiltonian-simulation.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-58/4/b/iii/solution.md)
