# Deutsch algorithm

↑ **Parent:** [Deutsch-Jozsa algorithm](deutsch-jozsa-algorithm.md)

The one-input Deutsch algorithm determines whether a [Boolean function](boolean-function.md) is constant or balanced using one [Boolean quantum oracle](boolean-quantum-oracle.md) call. Initialize the input [qubit](qubit.md) in $|+\rangle$ and the answer [qubit](qubit.md) in $|-\rangle$. [Quantum phase kickback](phase-kickback.md) changes the input to $(-1)^{f(0)}(|0\rangle+(-1)^{f(0)\oplus f(1)}|1\rangle)/\sqrt2$. A [Hadamard gate](hadamard-gate.md) and [computational-basis measurement](quantum-measurement-in-the-computational-basis.md) therefore return the parity $f(0)\oplus f(1)$ with certainty.

**Table of contents**

- [Deutsch algorithm with pure dephasing](deutsch-algorithm-with-pure-dephasing.md)

## ↑ Ancestors (5)

1. [Deutsch-Jozsa algorithm](deutsch-jozsa-algorithm.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Balanced Boolean function](balanced-boolean-function.md)
- [Deutsch algorithm with pure dephasing](deutsch-algorithm-with-pure-dephasing.md)
- [One-query obstruction to exact Boolean truth-table identification](one-query-obstruction-to-exact-boolean-truth-table-identification.md)
- [Solution](past-exam-of-the-introduction-to-quantum-information-course-of-the-university-of-oxford/2015/3/c/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2015/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47/1/solution.md)
