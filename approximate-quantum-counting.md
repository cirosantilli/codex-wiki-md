# Approximate quantum counting

↑ **Parent:** [Quantum algorithm](quantum-algorithm.md)

Approximate quantum counting estimates the number $k$ of [satisfying assignments](satisfying-assignment.md) of a [Boolean function](boolean-function.md), using a [quantum oracle](quantum-oracle.md) and [quantum measurement](quantum-measurement-split.md). Controlled repetitions of a [Grover search algorithm](grover-s-algorithm.md) iteration let [quantum interference](quantum-interference.md) reveal the count. For one input [bit](bit.md), a [Hadamard test](hadamard-test.md) can give [Pauli Z gate](pauli-z-gate.md) [expectation value](expectation-value.md) $1-k$: with the complemented [phase oracle](phase-oracle.md) $U_f=\operatorname{diag}(2f(0)-1,2f(1)-1)$ and $G=-XU_f$, use $\langle+|X=\langle+|$ to obtain $\langle+|G|+\rangle=-[(2f(0)-1)+(2f(1)-1)]/2=1-k$. Repeated preparations estimate this [expectation value](expectation-value.md); one binary measurement result does not distinguish all three counts $0,1,2$.

## ↑ Ancestors (4)

1. [Quantum algorithm](quantum-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2006/5/2/solution.md)
