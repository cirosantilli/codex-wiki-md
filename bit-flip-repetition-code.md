# Bit-flip repetition code

↑ **Parent:** [Stabilizer code](stabilizer-code.md)

The $m$-[qubit](qubit.md) [bit-flip repetition code](bit-flip-repetition-code.md) stores one [logical qubit](logical-qubit.md) in $|0_L\rangle=|0\rangle^{\otimes m}$ and $|1_L\rangle=|1\rangle^{\otimes m}$. Its [stabilizer generators](stabilizer-generator.md) are $Z_jZ_{j+1}$ for $j=1,\ldots,m-1$, and its logical operators are $\overline X=X_1\cdots X_m$ and $\overline Z=Z_1$. Interchanging the [Pauli X gate](pauli-x-gate.md) and [Pauli Z gate](pauli-z-gate.md) gives the [phase-flip repetition code](phase-flip-repetition-code.md). For odd $m$, [majority-vote decoding of a repetition code](majority-vote-decoding-of-a-repetition-code.md) corrects up to $(m-1)/2$ physical [Pauli X gate](pauli-x-gate.md) errors, assuming ideal operations and a noise family containing only these bit flips.

For $m=3$, prepare two [quantum ancillas](quantum-ancilla.md) in $|00\rangle$ and apply [controlled-NOT gates](controlled-not-gate.md) from the input [qubit](qubit.md) to each of them. By [linearity](linearity.md), encoding sends

$$
(\alpha|0\rangle+\beta|1\rangle)|00\rangle\longmapsto
|\psi_L\rangle=\alpha|000\rangle+\beta|111\rangle,\qquad |\alpha|^2+|\beta|^2=1.
$$

This does not produce $(\alpha|0\rangle+\beta|1\rangle)^{\otimes3}$, which would contain cross terms. For example, encoding $|+\rangle=(|0\rangle+|1\rangle)/\sqrt2$ produces $(|000\rangle+|111\rangle)/\sqrt2$, whereas three independent copies would have eight equal [computational basis](computational-basis.md) amplitudes. The encoding creates [quantum entanglement](entangled-state.md) when both coefficients are nonzero and respects the [no-cloning theorem](no-cloning-theorem.md).

The [three-qubit bit-flip syndrome table](three-qubit-bit-flip-syndrome-table.md) corrects the family $\{I,X_1,X_2,X_3\}$ and its entire [linear span](linear-span.md), as specified by the [Knill--Laflamme condition](knill-laflamme-condition.md). It cannot correct arbitrary errors on one physical [qubit](qubit.md): the [phase flip](pauli-z-gate.md)

$$
Z_1|\psi_L\rangle=\alpha|000\rangle-\beta|111\rangle
$$

commutes with both checks and acts as logical $\overline Z$. In particular, it takes the encoded $|+\rangle$ to the [orthogonal](orthogonal-vectors.md) encoded $|-\rangle$ with [error syndrome](error-syndrome.md) $00$. Thus its full [quantum code distance](distance-of-a-quantum-error-correcting-code.md) is one, despite correcting one error of the restricted [Pauli X gate](pauli-x-gate.md) type. The [Shor code](shor-code.md), [Steane code](steane-code.md) and [five-qubit error correcting code](five-qubit-error-correcting-code.md) provide protection against arbitrary one-[qubit](qubit.md) errors.

**Table of contents**

- [Three-qubit bit-flip syndrome table](three-qubit-bit-flip-syndrome-table.md)
- [Logical failure of the three-qubit bit-flip repetition code](logical-failure-of-the-three-qubit-bit-flip-repetition-code.md)
- [Coherent syndrome extraction for the three-qubit repetition code](coherent-syndrome-extraction-for-the-three-qubit-repetition-code.md)
  - [Timed bit flip during repetition-code syndrome extraction](timed-bit-flip-during-repetition-code-syndrome-extraction.md)
    - [Exact encoded-state failure with a faulty parity check](exact-encoded-state-failure-with-a-faulty-parity-check.md)

## ↑ Ancestors (6)

1. [Stabilizer code](stabilizer-code.md)
2. [Quantum error correction](quantum-error-correction-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Bit-flip repetition code](bit-flip-repetition-code.md)
- [Concatenated phase-and-bit-flip repetition code](concatenated-phase-and-bit-flip-repetition-code.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-49/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-342/2/c/solution.md)
- [Phase-flip protection by Hadamard conjugation](phase-flip-protection-by-hadamard-conjugation.md)
- [Quantum error correction](quantum-error-correction-split.md)
- [Stabilizer code](stabilizer-code.md)
