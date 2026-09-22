<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the ordered [computational basis](../../../../../../computational-basis.md) $00,01,10,11$, the first two [qubits](../../../../../../qubit.md) of $|\psi_{0000}\rangle$ have amplitudes $(1,1,1,1)/2$, while those of $|\psi_{1111}\rangle$ have amplitudes $(-1,1,1,1)/2$. Both have the same normalized answer [qubit](../../../../../../qubit.md) $|-\rangle$. Their [inner product](../../../../../../inner-product.md) is therefore

$$
\boxed{\langle\psi_{0000}|\psi_{1111}\rangle=\frac{-1+1+1+1}{4}=\frac12.}
$$

A common [unitary operator](../../../../../../unitary-operator.md) $U\otimes I$ preserves this nonzero [inner product](../../../../../../inner-product.md). To distinguish the alternatives with certainty using the prescribed [quantum measurement in the computational basis](../../../../../../quantum-measurement-in-the-computational-basis.md), their first-register outcome supports would have to be disjoint: every outcome possible under one alternative must be impossible under the other. Vectors with disjoint [computational basis](../../../../../../computational-basis.md) supports have zero [inner product](../../../../../../inner-product.md), contradicting its preservation. Thus **no such $U$ exists**. This is also an instance of [perfect discrimination of pure states requires orthogonality](../../../../../../perfect-discrimination-of-pure-states-requires-orthogonality.md); allowing a more general [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md) would not rescue this pair of states. The obstruction concerns these prepared oracle-output states, rather than every conceivable oracle-query procedure.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
