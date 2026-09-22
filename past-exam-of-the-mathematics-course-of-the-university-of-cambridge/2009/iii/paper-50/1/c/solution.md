<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use base-two logarithms, so [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) is measured in bits. Take an [orthonormal basis](../../../../../../orthonormal-basis.md) of the code and purify its maximally mixed logical state as

$$
|\Omega\rangle_{RQ}=2^{-k/2}\sum_{j=1}^{2^k}|j\rangle_R|j_L\rangle_Q.
$$

Only a $2^k$-dimensional reference support is needed; it can be embedded in the larger reference [Hilbert space](../../../../../../hilbert-space-split.md) in the hint. Its [reduced density matrix](../../../../../../reduced-density-matrix.md) is maximally mixed on that support, so $S(R)=k$.

For any correctable erased subsystem $A$, the [Knill--Laflamme condition](../../../../../../knill-laflamme-condition.md) gives $P(O_A\otimes I)P=c(O_A)P$ for every operator $O_A$. Taking its [matrix](../../../../../../matrix.md) elements in the logical basis shows that $\operatorname{Tr}_{Q\setminus A}|i_L\rangle\langle j_L|=0$ for $i\ne j$, and that the diagonal reductions are all the same state $\rho_A$. Thus

$$
\rho_{RA}=\rho_R\otimes\rho_A.
$$

In particular, the reference is decoupled from every set of at most $m=d-1$ erased [qubits](../../../../../../qubit.md).

For an information-carrying code $k>0$, first justify that two disjoint sets of size $m$ fit. If $2m\geq n$, partition all the physical [qubits](../../../../../../qubit.md) into sets $A,B$ each of size at most $m$. Both are correctable. Additivity of [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) for a [product state](../../../../../../product-state.md), and equality of complementary entropies for the [pure state](../../../../../../pure-state.md) on $RAB$, give

$$
S(R)+S(A)=S(B),\qquad S(R)+S(B)=S(A).
$$

Adding yields $2S(R)=0$, contradicting $S(R)=k>0$. Hence $2m<n$.

Now choose disjoint $A,B$ of size $m$, and let $C$ contain the remaining $n-2m$ [qubits](../../../../../../qubit.md). The state on $RABC$ is pure. Product-state entropy additivity, equality of complementary entropies, and [Subadditivity of Von Neumann entropy](../../../../../../subadditivity-of-von-neumann-entropy.md) give

$$
S(R)+S(A)=S(RA)=S(BC)\leq S(B)+S(C),
$$

and

$$
S(R)+S(B)=S(RB)=S(AC)\leq S(A)+S(C).
$$

Adding and cancelling proves $S(R)\leq S(C)$. Finally use the [maximum entropy of a quantum state](../../../../../../maximum-entropy-of-a-quantum-state.md) bound $S(C)\leq\log_2\dim\mathcal H_C=n-2m$. Therefore the [quantum Singleton bound](../../../../../../quantum-singleton-bound.md) is

$$
\boxed{k\leq n-2(d-1),\qquad n-k\geq2(d-1).}
$$

This proof uses [quantum erasure correction](../../../../../../quantum-erasure-correction.md), not nondegeneracy, so it applies to degenerate codes as well. A code encoding no logical information requires a separate distance convention; the argument above concerns the usual $k>0$ coding problem.

## ↑ Ancestors (11)

1. [C](../c.md)
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
