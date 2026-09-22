# Coherent syndrome extraction for the three-qubit repetition code

↑ **Parent:** [Bit-flip repetition code](bit-flip-repetition-code.md)

Encode $u|0\rangle+v|1\rangle$ as $u|000\rangle+v|111\rangle$. Four [controlled-NOT gates](controlled-not-gate.md) copy the displayed two data parities into initially zero [quantum ancillas](quantum-ancilla.md). No logical amplitude is measured. The [error syndromes](error-syndrome.md) $00,01,10,11$ correspond respectively to no bit flip and bit flips on data qubits $1,2,3$. Conditional [Toffoli gates](toffoli-gate.md), with temporary [Pauli X gates](pauli-x-gate.md) implementing zero-valued controls, undo the indicated error. Inverse encoding yields the original logical state and a separate syndrome state. A phase flip has zero bit-flip syndrome and remains as a logical phase error; this three-qubit code is not a general single-qubit-error code.

**Table of contents**

- [Timed bit flip during repetition-code syndrome extraction](timed-bit-flip-during-repetition-code-syndrome-extraction.md)
  - [Exact encoded-state failure with a faulty parity check](exact-encoded-state-failure-with-a-faulty-parity-check.md)

## ↑ Ancestors (7)

1. [Bit-flip repetition code](bit-flip-repetition-code.md)
2. [Stabilizer code](stabilizer-code.md)
3. [Quantum error correction](quantum-error-correction-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-49/3/a/solution.md)
