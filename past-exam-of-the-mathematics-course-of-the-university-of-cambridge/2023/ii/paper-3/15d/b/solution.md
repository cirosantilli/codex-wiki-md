<h1 id="15d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [inverse quantum circuit](../../../../../../inverse-quantum-circuit.md) rule. Every gate in $C$ is self-inverse, so reverse their order. From left to right, the circuit for $V^{-1}$ is:

1. a controlled-NOT with the lower qubit controlling the upper;  
2. $Z$ on the upper qubit and $H$ on the lower qubit;  
3. a controlled-NOT with the upper qubit controlling the lower;  
4. $H$ on the upper qubit.

This is the requested circuit description, with the two wires and control directions unchanged under each individual gate's adjoint.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
