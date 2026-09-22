# Stabilizer code

↑ **Parent:** [Quantum error correction](quantum-error-correction-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stabilizer_code)

A [stabilizer code](stabilizer-code.md) is the common $+1$ [eigenspace](eigenspace.md) of a [stabilizer group](stabilizer-group.md) $S$, an [abelian subgroup](abelian-subgroup.md) of the [Pauli group](pauli-group.md) excluding $-I$. Choose $r$ independent [stabilizer generators](stabilizer-generator.md) $g_1,\ldots,g_r$ on $n$ physical [qubits](qubit.md). They are commuting [Hermitian operators](hermitian-operator.md), each squaring to $I$. The [stabilizer subspace](stabilizer-subspace.md) and its [orthogonal projector](orthogonal-projection.md) are

$$
\mathcal C=\{\,|\psi\rangle:g_j|\psi\rangle=|\psi\rangle\text{ for }j=1,\ldots,r\,\},\qquad
P=\prod_{j=1}^r\frac{I+g_j}{2}=\frac{1}{|S|}\sum_{g\in S}g.
$$

The [stabilizer-projector formula](stabilizer-projector-formula.md) gives $\dim\mathcal C=2^{n-r}$, so $k=n-r$ [logical qubits](logical-qubit.md) remain. Independent here means that no nonempty product of the chosen [stabilizer generators](stabilizer-generator.md) is $I$. Excluding $-I$ is necessary: a vector cannot simultaneously be fixed by $I$ and $-I$ unless it is zero.

For the three-[qubit](qubit.md) [bit-flip repetition code](bit-flip-repetition-code.md), take $g_1=Z_1Z_2$ and $g_2=Z_2Z_3$, with $Z_j$ the [Pauli Z gate](pauli-z-gate.md) on site $j$ and identities elsewhere. The [stabilizer group](stabilizer-group.md) is $S=\{I,Z_1Z_2,Z_2Z_3,Z_1Z_3\}$. Both [stabilizer generators](stabilizer-generator.md) have [eigenvalue](eigenvalue.md) $+1$ exactly on the span of $|000\rangle$ and $|111\rangle$, giving $2^{3-2}=2$ dimensions for one [logical qubit](logical-qubit.md). A [projective measurement](projective-measurement.md) of these checks distinguishes four [orthogonal](orthogonal-vectors.md) two-dimensional sectors rather than eight individual [computational basis](computational-basis.md) states.

A [Pauli error](pauli-operator.md) that anticommutes with a [stabilizer generator](stabilizer-generator.md) changes that check's sign, producing an [error syndrome](error-syndrome.md). A [Pauli operator](pauli-operator.md) commuting with every check can still act on the [logical qubits](logical-qubit.md); the [centralizer of a stabilizer group](centralizer-of-a-stabilizer-group.md) describes these possibilities. Thus the number of checks determines the encoded dimension, while the [quantum code distance](distance-of-a-quantum-error-correcting-code.md) determines protection against arbitrary local errors. The [five-qubit error correcting code](five-qubit-error-correcting-code.md), for instance, has four [stabilizer generators](stabilizer-generator.md) and [quantum code distance](distance-of-a-quantum-error-correcting-code.md) three; the three-[qubit](qubit.md) [bit-flip repetition code](bit-flip-repetition-code.md) has two checks but [quantum code distance](distance-of-a-quantum-error-correcting-code.md) one because a single [phase flip](pauli-z-gate.md) is unflagged. [Preskill, §7.9.1: stabilizers, syndromes and logical operators](https://www.preskill.caltech.edu/ph229/notes/chap7.pdf).

**Table of contents**

- [Symplectic representation of a stabilizer code](symplectic-representation-of-a-stabilizer-code.md)
- [CSS code](css-code.md)
  - [Nested-code CSS syndrome recovery](nested-code-css-syndrome-recovery.md)
- [Centralizer of a stabilizer group](centralizer-of-a-stabilizer-group.md)
- [Local correctability of a stabilizer code](local-correctability-of-a-stabilizer-code.md)
  - [Pauli error criterion for a stabilizer code](pauli-error-criterion-for-a-stabilizer-code.md)
- [Dressed stabilizer under a weak local perturbation](dressed-stabilizer-under-a-weak-local-perturbation.md)
- [Distance of a stabilizer code](distance-of-a-stabilizer-code.md)
- [Error syndrome](error-syndrome.md)
  - [Stabilizer-syndrome coset](stabilizer-syndrome-coset.md)
- [Phase-flip repetition code](phase-flip-repetition-code.md)
  - [Logical Hadamard convention for a phase-flip repetition code](logical-hadamard-convention-for-a-phase-flip-repetition-code.md)
  - [Logical failure of the three-qubit phase-flip repetition code](logical-failure-of-the-three-qubit-phase-flip-repetition-code.md)
  - [Phase-flip protection by Hadamard conjugation](phase-flip-protection-by-hadamard-conjugation.md)
  - [Majority-vote decoding of a repetition code](majority-vote-decoding-of-a-repetition-code.md)
- [Bit-flip repetition code](bit-flip-repetition-code.md)
  - [Three-qubit bit-flip syndrome table](three-qubit-bit-flip-syndrome-table.md)
  - [Logical failure of the three-qubit bit-flip repetition code](logical-failure-of-the-three-qubit-bit-flip-repetition-code.md)
  - [Coherent syndrome extraction for the three-qubit repetition code](coherent-syndrome-extraction-for-the-three-qubit-repetition-code.md)
    - [Timed bit flip during repetition-code syndrome extraction](timed-bit-flip-during-repetition-code-syndrome-extraction.md)
      - [Exact encoded-state failure with a faulty parity check](exact-encoded-state-failure-with-a-faulty-parity-check.md)
- [Concatenated phase-and-bit-flip repetition code](concatenated-phase-and-bit-flip-repetition-code.md)
  - [Shor code](shor-code.md)
    - [Shor-code phase-flip syndrome](shor-code-phase-flip-syndrome.md)
- [Steane code](steane-code.md)
  - [Nondegenerate phase-flip correction in the Steane code](nondegenerate-phase-flip-correction-in-the-steane-code.md)
- [Color code](color-code.md)
  - [String operator in a topological code](string-operator-in-a-topological-code.md)
- [Surface code](surface-code.md)
  - [Surface code on a chain of spheres](surface-code-on-a-chain-of-spheres.md)
  - [Surface-code decoding as a random-bond Ising model](surface-code-decoding-as-a-random-bond-ising-model.md)
  - [Ground-state splitting of a surface-code cylinder](ground-state-splitting-of-a-surface-code-cylinder.md)
  - [Toric code](toric-code.md)
    - [Surface-code anyon model](surface-code-anyon-model.md)

## ↑ Ancestors (5)

1. [Quantum error correction](quantum-error-correction-split.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Five-qubit stabilizer syndrome table](five-qubit-stabilizer-syndrome-table.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-50/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-342/2/a/solution.md)
- [Quantum error correction](quantum-error-correction-split.md)
- [Stabilizer code](stabilizer-code.md)
