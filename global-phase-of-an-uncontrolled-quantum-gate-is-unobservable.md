# Global phase of an uncontrolled quantum gate is unobservable

↑ **Parent:** [Global phase](global-phase.md)

A physical [unitary gate](quantum-logic-gate.md) used without coherent control gives the same [quantum channel](quantum-channel.md) for $V$ and $e^{i\gamma}V$:

$$
(e^{i\gamma}V)\rho(e^{i\gamma}V)^\dagger=V\rho V^\dagger.
$$

Interleaving any preparations, known operations and measurements preserves this equality. Equivalently, each fixed measurement branch with $k$ uses gains only the overall factor $e^{ik\gamma}$, which cancels in its [probability](probability.md). Thus unrestricted repeated uncontrolled uses do not determine the common phase of the [eigenvalues](eigenvalue.md). A supplied [controlled unitary gate](controlled-unitary-gate.md) is a different resource: $|0\rangle\langle0|\otimes I+|1\rangle\langle1|\otimes V$ changes by a relative control phase when $V$ is replaced by $e^{i\gamma}V$. Such controlled access permits [quantum phase estimation](quantum-phase-estimation.md) to measure that phase relative to the identity branch.

## ↑ Ancestors (8)

1. [Global phase](global-phase.md)
2. [Quantum phase](quantum-phase.md)
3. [Quantum state](quantum-state.md)
4. [Quantum system](quantum-system.md)
5. [Quantum mechanics](quantum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/4/d/solution.md)
