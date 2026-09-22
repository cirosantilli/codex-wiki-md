<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a classical [error-correcting code](../../../../../error-correcting-code.md) of length $n$, alphabet size $q$, minimum [Hamming distance](../../../../../hamming-distance.md) $d$ and $M$ codewords, the [Singleton bound](../../../../../singleton-bound.md) is

$$
M\le q^{n-d+1}.
$$

For a linear $[n,k,d]_q$ code this is **$n-k\ge d-1$**. Deleting any $d-1$ coordinates is injective on the codewords, since two words agreeing on the remaining coordinates would differ in fewer than $d$ positions; this also explains the classical bound.

For an n-[qubit](../../../../../qubit.md) [quantum code](../../../../../quantum-error-correcting-code.md) carrying $k>0$ [logical qubits](../../../../../logical-qubit.md) and having [quantum code distance](../../../../../distance-of-a-quantum-error-correcting-code.md) $d$, the [quantum Singleton bound](../../../../../quantum-singleton-bound.md) is

$$
\boxed{n-k\ge2(d-1).}
$$

More generally replace $k$ by $\log_2K$ for code dimension $K>1$. The proof applies to degenerate codes too.

Let $r=d-1$. Purify the maximally mixed encoded input by a reference $R$ of dimension $K$:

$$
|\Omega\rangle=K^{-1/2}\sum_{j=1}^K|j\rangle_R|j_L\rangle,\qquad S(R)=\log_2K=:k.
$$

Distance $d$ makes erasure of any subset of at most $r$ [qubits](../../../../../qubit.md) correctable. The allowed [quantum erasure correction](../../../../../quantum-erasure-correction.md) condition says that a correctable erased set $A$ is decoupled from $R$:

$$
\rho_{RA}=\rho_R\otimes\rho_A,\qquad S(RA)=k+S(A).
$$

This is the [matrix](../../../../../matrix.md)-element correction condition in another form: all operators on $A$ have constant diagonal [matrix](../../../../../matrix.md) elements and zero off-diagonal [matrix](../../../../../matrix.md) elements in the logical basis, so tracing the other physical [qubits](../../../../../qubit.md) in $|\Omega\rangle\langle\Omega|$ yields the displayed product.

First justify the sizes needed for the partition. If $2r>n$, partition all physical [qubits](../../../../../qubit.md) into $A,B$, both of size at most $r$. Both sets are correctable. Purity of $RAB$ and the [Schmidt decomposition](../../../../../schmidt-decomposition.md) give

$$
k+S(A)=S(RA)=S(B),\qquad k+S(B)=S(RB)=S(A).
$$

Adding forces $k=0$, a contradiction. Thus $2r\le n$, without assuming the bound we aim to prove.

Choose disjoint sets $A,B$ of size $r$, and let $C$ contain the remaining $n-2r$ [qubits](../../../../../qubit.md). The joint state $RABC$ is pure, so decoupling and [Subadditivity of Von Neumann entropy](../../../../../subadditivity-of-von-neumann-entropy.md) give

$$
k+S(A)=S(RA)=S(BC)\le S(B)+S(C),
$$



$$
k+S(B)=S(RB)=S(AC)\le S(A)+S(C).
$$

Adding and cancelling gives $k\le S(C)$. The [Von Neumann entropy](../../../../../von-neumann-entropy-split.md) of $D$-dimensional states is at most $\log_2D$: for positive [eigenvalues](../../../../../eigenvalue.md) $p_i$, concavity of the [logarithm](../../../../../logarithm.md) gives $\sum_i p_i\log_2(1/p_i)\le\log_2\sum_i p_i/p_i\le\log_2D$. Here $D=2^{n-2r}$, so $k\le n-2r$, proving the quantum bound. The code is assumed to encode information ($K>1$); a one-dimensional code requires a separate distance convention, since simply re-preparing a known state makes its erasure-correction condition vacuous.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
