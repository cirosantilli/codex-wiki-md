# Entanglement-assisted promised equality protocol

↑ **Parent:** [Communication complexity](communication-complexity.md)

For even positive $n$, share the [maximally entangled state](maximally-entangled-state.md) $|\Omega\rangle=n^{-1/2}\sum_{i=0}^{n-1}|ii\rangle$. Each party applies a [phase oracle](phase-oracle.md) from its input [binary string](binary-string.md), producing $|\Omega_{xy}\rangle=n^{-1/2}\sum_i(-1)^{x_i+y_i}|ii\rangle$. Its overlap with $|\Omega\rangle$ is the displayed expression because the [Hamming distance](hamming-distance.md) counts exactly the negative signs. Under the promise $d_H(x,y)\in\{0,n/2\}$, the output either equals $|\Omega\rangle$ or is [orthogonal](orthogonal-vectors.md) to it. Sending one subsystem lets the receiver distinguish the cases with the [projective measurement](projective-measurement.md) $\{|\Omega\rangle\langle\Omega|,I-|\Omega\rangle\langle\Omega|\}$. The transmitted system needs $\lceil\log_2n\rceil$ [qubits](qubit.md), including when $n$ is not a power of two.

## ↑ Ancestors (5)

1. [Communication complexity](communication-complexity.md)
2. [Computational complexity theory](computational-complexity-theory.md)
3. [Theoretical computer science](theoretical-computer-science-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/quantum-information/2/c/solution.md)
