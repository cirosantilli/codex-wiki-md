# Parallel phase multiplication by coherent fanout

↑ **Parent:** [Quantum phase estimation](quantum-phase-estimation.md)

Use [CNOT gates](controlled-not-gate.md) to encode one logical [qubit](qubit.md) and $r-1$ zero ancillas into the repetition subspace spanned by $|0^r\rangle,|1^r\rangle$. Apply the [phase gate](phase-gate.md) in parallel to all $r$ physical [qubits](qubit.md), then undo the encoding. The logical phase is multiplied by $r$ in one oracle-time layer. This copies computational-basis labels coherently rather than cloning an arbitrary [quantum state](quantum-state.md). Blocks of sizes $1,2,4,\ldots,2^{n-1}$ prepare a dyadic Fourier phase state using $2^n-1$ parallel oracle applications.

## ↑ Ancestors (6)

1. [Quantum phase estimation](quantum-phase-estimation.md)
2. [Quantum Fourier transform](quantum-fourier-transform.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-58/1/d/solution.md)
