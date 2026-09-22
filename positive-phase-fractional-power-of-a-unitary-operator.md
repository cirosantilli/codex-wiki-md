# Positive-phase fractional power of a unitary operator

↑ **Parent:** [Quantum phase estimation](quantum-phase-estimation.md)

Choose eigenphase representatives $0\leq\phi_j<1$ for a [unitary operator](unitary-operator.md) $U$ and a positive integer $M$. Its positive-phase fractional power acts on each [eigenstate](eigenstate.md) by $e^{2\pi i\phi_j/M}$. This branch uses arguments in $[0,2\pi)$ and can differ from the usual complex principal branch using $(-\pi,\pi]$. For exactly dyadic phases, [exact quantum phase estimation](exact-quantum-phase-estimation.md) stores each label in a coherent phase register; bitwise [phase gates](phase-gate.md) multiply it by the required phase, and inverse phase estimation removes the labels. Keeping the phase register unmeasured preserves arbitrary [eigenstate](eigenstate.md) superpositions and resets the [ancilla qubits](ancilla-qubit.md). With only controlled-$U$ and controlled-$U^{-1}$ primitives, the direct method uses $2(2^n-1)$ oracle calls for $n$ exact phase bits.

## ↑ Ancestors (6)

1. [Quantum phase estimation](quantum-phase-estimation.md)
2. [Quantum Fourier transform](quantum-fourier-transform.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61/3/iii/solution.md)
