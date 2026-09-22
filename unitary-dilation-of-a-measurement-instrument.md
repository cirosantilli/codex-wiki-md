# Unitary dilation of a measurement instrument

↑ **Parent:** [Quantum instrument](quantum-instrument.md)

For [Kraus operators](kraus-operator.md) satisfying $\sum_iA_i^\dagger A_i=I$, the map $V|\phi\rangle=\sum_iA_i|\phi\rangle\otimes|i\rangle$ is an [isometry](isometry.md). Implement it by a [unitary operator](unitary-operator.md) on the system and a [quantum ancilla](quantum-ancilla.md), initially in an extra unused state $|0\rangle$. Projecting the output [quantum ancilla](quantum-ancilla.md) onto $|i\rangle$ gives joint unnormalized state $A_i\rho A_i^\dagger\otimes|i\rangle\langle i|$. The outcome [probability](probability.md) is $\operatorname{Tr}(A_i\rho A_i^\dagger)$, and the conditional system state is $A_i\rho A_i^\dagger$ divided by this [probability](probability.md). The unused level can be merged into the first [orthogonal projection](orthogonal-projection.md) without changing any outcome on the prepared state, giving a complete [projective measurement](projective-measurement.md) with exactly the original outcome labels.

// Target: quantum-theory.bigb

## ↑ Ancestors (7)

1. [Quantum instrument](quantum-instrument.md)
2. [No information without disturbance](no-information-without-disturbance.md)
3. [Measurement in quantum mechanics](quantum-measurement-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-59/3/solution.md)
