<h1 id="4/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The path [graph state](../../../../../../../graph-state.md) is $|\psi_3\rangle=E_{23}E_{12}|+\rangle_1|+\rangle_2|+\rangle_3$. The factor $Z_3^r$ commutes with both the [Controlled-Z gates](../../../../../../../controlled-z-gate.md) and the [measurement in quantum mechanics](../../../../../../../quantum-measurement-split.md) of [vertex](../../../../../../../vertex-graph-theory.md) $1$. Treat $Z_1^r|+\rangle_1$ as the input of [one-bit teleportation](../../../../../../../one-bit-teleportation.md). The [equatorial qubit measurement](../../../../../../../equatorial-qubit-measurement.md) result $s$ therefore gives the normalized state

$$
E_{23}X_2^sJ(\alpha)_2Z_2^r|+\rangle_2\,Z_3^r|+\rangle_3.
$$

Here the subscript on $Z_2^r$ expresses the teleported input factor; it is not an extra operation on the already measured [vertex](../../../../../../../vertex-graph-theory.md). Use $J(\alpha)Z^r=X^rJ(\alpha)$ to obtain

$$
\boxed{E_{23}X_2^{r\oplus s}J(\alpha)_2Z_3^r|+\rangle_2|+\rangle_3.}
$$

The [exclusive or](../../../../../../../exclusive-or.md) exponent is equivalent to the printed sum $r+s$ because $X^2=I$. The conditional probability of $s$ is one half for either $r$, by the [one-bit teleportation](../../../../../../../one-bit-teleportation.md) branch norm. This calculation concerns an [equatorial measurement of a graph-state leaf](../../../../../../../equatorial-measurement-of-a-graph-state-leaf.md); no third remaining [qubit](../../../../../../../qubit.md) or extra $|-\rangle$ factor is present.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
