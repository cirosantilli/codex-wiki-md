<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Store a tensor-product element of the [Pauli group](../../../../../../pauli-group.md) as

$$
P=i^s\bigotimes_{j=1}^nX^{a_j}Z^{b_j},\qquad s\in\mathbb Z/4\mathbb Z,\quad a_j,b_j\in\{0,1\}.
$$

The phases of the original single-[qubit](../../../../../../qubit.md) factors can all be accumulated into $i^s$. This [binary phase representation of a Pauli string](../../../../../../binary-phase-representation-of-a-pauli-string.md) uses $2n+2$ bits. It retains phases, which must not be dropped when computing probabilities later.

For the conjugation convention $U^\dagger P U$ in the question, direct multiplication of the two-by-two matrices gives

$$
H^\dagger XH=Z,\quad H^\dagger ZH=X,\quad H^\dagger XZH=-XZ,
$$

and

$$
S^\dagger XS=-iXZ,\quad S^\dagger ZS=Z,\quad S^\dagger XZS=-iX.
$$

These [backward Pauli updates for Hadamard and phase gates](../../../../../../backward-pauli-updates-for-hadamard-and-phase-gates.md) use $S^\dagger P S$, not $SPS^\dagger$. On the affected line $j$, the updates are

$$
\begin{aligned}
H_j:&\quad(a_j,b_j)\mapsto(b_j,a_j),\quad s\mapsto s+2a_jb_j,\\
S_j:&\quad(a_j,b_j)\mapsto(a_j,b_j\oplus a_j),\quad s\mapsto s-a_j.
\end{aligned}
$$

All phases are reduced modulo four and the updates use the old bits.

For a [Controlled-Z gate](../../../../../../controlled-z-gate.md) on lines $j,k$, its diagonal action gives

$$
CZ\,X_j\,CZ=X_jZ_k,\quad CZ\,X_k\,CZ=Z_jX_k,\quad
CZ\,Z_j\,CZ=Z_j,\quad CZ\,Z_k\,CZ=Z_k.
$$

For the [controlled-Z update in the binary phase representation](../../../../../../controlled-z-update-in-the-binary-phase-representation.md), conjugation respects products, so these determine the rule for every [Pauli operator](../../../../../../pauli-operator.md) on those lines. In the chosen ordered $XZ$ convention it is

$$
\boxed{b_j\mapsto b_j\oplus a_k,\quad b_k\mapsto b_k\oplus a_j,\quad
s\mapsto s+2a_ja_k,\quad a_j,a_k\text{ unchanged}.}
$$

The phase arises when a newly introduced $Z_k$ is moved past $X_k$. For instance $X_jX_k$ becomes $-X_jZ_jX_kZ_k$, so this sign matters.

The untouched factors are unchanged. Each [Clifford operation](../../../../../../clifford-gate.md) therefore needs only a fixed number of local bit updates; reconstructing the requested full list takes $O(n)$ time. Put the final phase into the first factor, which is permitted because the single-[qubit](../../../../../../qubit.md) [Pauli group](../../../../../../pauli-group.md) includes all multiples by $\pm1,\pm i$. **The classical cost is polynomial**, despite the exponentially large matrix of the operation on the full state space.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
