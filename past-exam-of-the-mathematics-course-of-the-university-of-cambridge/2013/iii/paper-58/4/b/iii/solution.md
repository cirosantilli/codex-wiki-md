<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The product of the data [Pauli Z gates](../../../../../../../pauli-z-gate.md) has computational-basis [eigenvalue](../../../../../../../eigenvalue.md)

$$
(Z^{\otimes n})|x\rangle=(-1)^{x_1+\cdots+x_n}|x\rangle=(-1)^{f(x)}|x\rangle.
$$

Use the parity circuit $W$ from part (ii), apply the target [unitary gate](../../../../../../../quantum-logic-gate.md) $R=e^{itZ}=\operatorname{diag}(e^{it},e^{-it})$, and then uncompute the parity with $W^\dagger$. For every basis input,

$$
W^\dagger(I\otimes e^{itZ})W|x\rangle|0\rangle=e^{it(-1)^{f(x)}}|x\rangle|0\rangle.
$$

This equals $e^{itZ^{\otimes n}}$ on the data, with the [ancilla qubit](../../../../../../../ancilla-qubit.md) returned to zero. The [compute-phase-uncompute construction](../../../../../../../compute-phase-uncompute-construction.md) therefore gives **an exact linear-size circuit:**

$$
\boxed{V=e^{itZ^{\otimes n}}:\quad n\ \mathrm{CNOTs},\ e^{itZ}\ \text{on the ancilla},\ n\ \mathrm{CNOTs};\qquad 2n+1\text{ gates}.}
$$

This is a [Pauli-string phase by parity computation](../../../../../../../pauli-string-phase-by-parity-computation.md), an instance of [simulation of a computable diagonal Hamiltonian](../../../../../../../simulation-of-a-computable-diagonal-hamiltonian.md). Part (i) also explains it by $W^\dagger(I\otimes Z)W=Z^{\otimes n}\otimes Z$, whose exponential restricts correctly to the target-$|0\rangle$ subspace. If no extra line is desired, accumulate parity into the last data [qubit](../../../../../../../qubit.md), apply $e^{itZ}$ there, and undo the $n-1$ [CNOT gates](../../../../../../../controlled-not-gate.md), for $2n-1$ gates. Both constructions implement the global phase as well as the relative phases exactly.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 58](../../../../paper-58-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
