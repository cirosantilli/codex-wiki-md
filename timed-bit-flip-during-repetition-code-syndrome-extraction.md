# Timed bit flip during repetition-code syndrome extraction

↑ **Parent:** [Coherent syndrome extraction for the three-qubit repetition code](coherent-syndrome-extraction-for-the-three-qubit-repetition-code.md)

Suppose the first ancilla records parity $q_2\oplus q_3$, then a fault of value $f$ flips $q_2$, and the second ancilla records parity $q_1\oplus q_2$. For incoming bit-error pattern $e$, the observed [error syndrome](error-syndrome.md) is the displayed pair, while the final data error before recovery is $d=e\oplus(0,f,0)$. When $f=1$, the observed syndrome differs from the actual data syndrome by $(1,0)$. Applying the usual minimum-weight recovery leaves a nonzero syndrome, so the state is outside the code space even when the channel itself made no error. This is a timing-dependent failure of this simple extraction circuit, not a general obstruction to fault-tolerant [quantum error correction](quantum-error-correction-split.md).

**Table of contents**

- [Exact encoded-state failure with a faulty parity check](exact-encoded-state-failure-with-a-faulty-parity-check.md)

## ↑ Ancestors (8)

1. [Coherent syndrome extraction for the three-qubit repetition code](coherent-syndrome-extraction-for-the-three-qubit-repetition-code.md)
2. [Bit-flip repetition code](bit-flip-repetition-code.md)
3. [Stabilizer code](stabilizer-code.md)
4. [Quantum error correction](quantum-error-correction-split.md)
5. [Quantum theory](quantum-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58/3/b/solution.md)
