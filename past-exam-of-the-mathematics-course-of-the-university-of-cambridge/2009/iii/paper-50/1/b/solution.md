<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $A$ be the known set of affected [qubits](../../../../../../qubit.md), with $|A|\leq d-1$. Expand arbitrary operators on $A$ in [tensor products](../../../../../../tensor-product.md) of $I,X,Y,Z$. These [Pauli operators](../../../../../../pauli-operator.md) span the complete error space on $A$.

By the [distance of a quantum error-correcting code](../../../../../../distance-of-a-quantum-error-correcting-code.md), every [Pauli operator](../../../../../../pauli-operator.md) $F$ of weight below $d$ has scalar compression $PFP=c_FP$. For two errors $E_a,E_b$ on the same known set $A$, their product $E_a^\dagger E_b$ is also supported entirely on $A$. Its weight is therefore at most $|A|$, rather than twice $|A|$. Expansion in the Pauli basis consequently gives

$$
PE_a^\dagger E_bP=C_{ab}P.
$$

The [Knill--Laflamme condition](../../../../../../knill-laflamme-condition.md) applies to the full operator space on $A$, so it gives a recovery for any error channel acting on that subsystem. **Every set of at most $d-1$ known error locations is correctable.** This is [quantum erasure correction](../../../../../../quantum-erasure-correction.md); the ability to use the locations is what improves the guarantee over unknown-location errors.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
