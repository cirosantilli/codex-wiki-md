# Error syndrome

↑ **Parent:** [Stabilizer code](stabilizer-code.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Error_syndrome)

An [error syndrome](error-syndrome.md) is the list of outcomes obtained by measuring a chosen ordered family of [stabilizer generators](stabilizer-generator.md). Write $s_j=0$ for [eigenvalue](eigenvalue.md) $+1$ and $s_j=1$ for [eigenvalue](eigenvalue.md) $-1$. For a definite [Pauli error](pauli-operator.md) $E$ on a code state, the rule is

$$
g_jE=(-1)^{s_j}Eg_j,\qquad g_jE|\psi_L\rangle=(-1)^{s_j}E|\psi_L\rangle.
$$

The commuting checks admit joint [orthogonal projectors](orthogonal-projection.md)

$$
\Pi_s=\prod_{j=1}^r\frac{I+(-1)^{s_j}g_j}{2},\qquad
\sum_{s\in\{0,1\}^r}\Pi_s=I,\qquad \Pi_0=P.
$$

For [density operator](density-matrix.md) $\rho$, the [Born rule](born-rule.md) gives outcome [probability](probability.md) $\operatorname{tr}(\Pi_s\rho)$ and conditional state $\Pi_s\rho\Pi_s/\operatorname{tr}(\Pi_s\rho)$ when that [probability](probability.md) is nonzero. A definite [Pauli error](pauli-operator.md) has one deterministic [error syndrome](error-syndrome.md) independent of the encoded amplitudes. A coherent [linear combination](linear-combination.md) of [Pauli errors](pauli-operator.md) may occupy several sectors, so measuring the [error syndrome](error-syndrome.md) selects a sector; recovery preserves the [logical qubit](logical-qubit.md) when the entire error family is jointly correctable. [Preskill, §§7.2 and 7.9.1](https://www.preskill.caltech.edu/ph229/notes/chap7.pdf).

An [error syndrome](error-syndrome.md) locates an error only relative to an assumed family and a recovery rule. Two [Pauli errors](pauli-operator.md) differing by a logical operator can share an [error syndrome](error-syndrome.md); see [stabilizer-syndrome coset](stabilizer-syndrome-coset.md). In the [three-qubit bit-flip syndrome table](three-qubit-bit-flip-syndrome-table.md), $X_3$ and $X_1X_2$ both give $01$. Recovering with $X_3$ corrects the first but converts the second into the logical operator $X_1X_2X_3$. Likewise, $Z_1$ has [error syndrome](error-syndrome.md) $00$ yet changes the encoded relative phase.

**Table of contents**

- [Stabilizer-syndrome coset](stabilizer-syndrome-coset.md)

## ↑ Ancestors (6)

1. [Stabilizer code](stabilizer-code.md)
2. [Quantum error correction](quantum-error-correction-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (27)

- [Bit-flip repetition code](bit-flip-repetition-code.md)
- [Coherent syndrome extraction for the three-qubit repetition code](coherent-syndrome-extraction-for-the-three-qubit-repetition-code.md)
- [Error syndrome](error-syndrome.md)
- [Exact encoded-state failure with a faulty parity check](exact-encoded-state-failure-with-a-faulty-parity-check.md)
- [Five-qubit stabilizer syndrome table](five-qubit-stabilizer-syndrome-table.md)
- [Logical failure of the three-qubit bit-flip repetition code](logical-failure-of-the-three-qubit-bit-flip-repetition-code.md)
- [Logical failure of the three-qubit phase-flip repetition code](logical-failure-of-the-three-qubit-phase-flip-repetition-code.md)
- [Nondegenerate phase-flip correction in the Steane code](nondegenerate-phase-flip-correction-in-the-steane-code.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53/3/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-49/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-342/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-342/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-342/2/b/solution.md)
- [Quantum error correction](quantum-error-correction-split.md)
- [Quantum error detection](quantum-error-detection.md)
- [Stabilizer code](stabilizer-code.md)
- [Three-qubit bit-flip syndrome table](three-qubit-bit-flip-syndrome-table.md)
- [Timed bit flip during repetition-code syndrome extraction](timed-bit-flip-during-repetition-code-syndrome-extraction.md)
