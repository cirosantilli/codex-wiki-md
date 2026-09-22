<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Initialize three [qubits](../../../../../../qubit.md) in $|000\rangle$. Apply a [Hadamard gate](../../../../../../hadamard-gate.md) on the first, then [controlled-NOT gates](../../../../../../controlled-not-gate.md) $1\to2$ and $1\to3$:

$$
|000\rangle\longmapsto\frac{|000\rangle+|100\rangle}{\sqrt2}
\longmapsto\frac{|000\rangle+|111\rangle}{\sqrt2}.
$$

Apply the [T gate](../../../../../../t-gate.md) twice to the first [qubit](../../../../../../qubit.md). Because $T^2=\operatorname{diag}(1,i)$, the resulting [GHZ state](../../../../../../greenberger-horne-zeilinger-state.md) with the specified [relative quantum phase](../../../../../../relative-quantum-phase.md) is

$$
\boxed{T_1^2\operatorname{CNOT}_{1\to3}\operatorname{CNOT}_{1\to2}H_1|000\rangle
=\frac{|000\rangle+i|111\rangle}{\sqrt2}.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
