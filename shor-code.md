# Shor code

↑ **Parent:** [Concatenated phase-and-bit-flip repetition code](concatenated-phase-and-bit-flip-repetition-code.md)

The nine-qubit Shor code encodes one logical [qubit](qubit.md) with basis vectors $|0_L\rangle=|G_+\rangle^{\otimes3}$ and $|1_L\rangle=|G_-\rangle^{\otimes3}$, where $|G_\pm\rangle=(|000\rangle\pm|111\rangle)/\sqrt2$. Six adjacent $Z$-pair [stabilizer generators](stabilizer-generator.md) locate a single bit flip within a block, while $X_1\cdots X_6$ and $X_4\cdots X_9$ diagnose which block has had its relative phase changed. Together they correct every single-qubit [Pauli operator](pauli-operator.md), hence every single-qubit error by the [Pauli expansion of a quantum error](pauli-expansion-of-a-quantum-error.md).

A [Pauli Z gate](pauli-z-gate.md) on qubit four has phase-check eigenvalues $(-1,-1)$ and leaves all six $Z$-pair checks positive. Applying $Z_4$ restores the state. The same phase syndrome arises from $Z_5$ or $Z_6$; these have the same action on the code since their pairwise products are stabilizers. This is a degeneracy, not a failure of correction.

**Table of contents**

- [Shor-code phase-flip syndrome](shor-code-phase-flip-syndrome.md)

## ↑ Ancestors (7)

1. [Concatenated phase-and-bit-flip repetition code](concatenated-phase-and-bit-flip-repetition-code.md)
2. [Stabilizer code](stabilizer-code.md)
3. [Quantum error correction](quantum-error-correction-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-33/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60/2/solution.md)
