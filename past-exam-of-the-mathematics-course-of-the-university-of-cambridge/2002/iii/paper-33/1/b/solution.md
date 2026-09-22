<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here the number of errors means the number of affected physical [qubits](../../../../../../qubit.md): assume that all errors supported on at most $t$ qubits are jointly correctable. It does not mean the cardinality of an arbitrary selected error list. Let $F$ be any [Pauli operator](../../../../../../pauli-operator.md) of weight at most $2t$. Split its support into disjoint sets $A,B$, each of size at most $t$, and write $F=F_AF_B$. Each Pauli factor is Hermitian, so take $E_a=F_A$, $E_b=F_B$ to get $F=E_a^\dagger E_b$, up to an irrelevant scalar phase if different Pauli representatives are used. The [Knill--Laflamme condition](../../../../../../knill-laflamme-condition.md) gives

$$
PFP=PE_a^\dagger E_bP=C_{ab}P.
$$

This is precisely [quantum error detection](../../../../../../quantum-error-detection.md): a [projective measurement](../../../../../../projective-measurement.md) with outcomes $P,I-P$ either detects departure from the code or leaves the accepted logical state unchanged up to a scalar. Some errors can be harmless scalars on the code, particularly for degenerate correction; detection is not required to flag such an error with certainty.

Any [linear operator](../../../../../../linear-operator.md) supported on at most $2t$ qubits is a linear combination of [Pauli operators](../../../../../../pauli-operator.md) on those qubits, so its code compression is scalar by [linearity](../../../../../../linearity.md). Thus

$$
\boxed{\text{correction of all errors of weight at most }t\ \Longrightarrow\ \text{detection of all errors of weight at most }2t.}
$$

This is [correction implies detection at twice the weight](../../../../../../correction-implies-detection-at-twice-the-weight.md). The premise about all locations and all error types is essential: merely correcting one selected operator gives no universal statement about every operator of twice its weight.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
