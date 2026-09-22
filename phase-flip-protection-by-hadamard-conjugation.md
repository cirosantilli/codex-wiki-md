# Phase-flip protection by Hadamard conjugation

↑ **Parent:** [Phase-flip repetition code](phase-flip-repetition-code.md)

Insert [Hadamard gates](hadamard-gate.md) on every data qubit immediately after encoding by a [bit-flip repetition code](bit-flip-repetition-code.md) and immediately before its bit-flip detection and recovery. The intervening physical error is thereby conjugated by $H^{\otimes n}$, and $HZH=X$ turns a single [Pauli Z gate](pauli-z-gate.md) error into a single bit flip for the original correction circuit. The encoded logical codewords are now $|+\rangle^{\otimes n}$ and $|-\rangle^{\otimes n}$. The syndrome ancillas and the final inverse encoding stay unchanged. This protects against phase flips in the new basis; it does not simultaneously correct arbitrary bit flips in the physical basis.

## ↑ Ancestors (7)

1. [Phase-flip repetition code](phase-flip-repetition-code.md)
2. [Stabilizer code](stabilizer-code.md)
3. [Quantum error correction](quantum-error-correction-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-49/3/d/solution.md)
