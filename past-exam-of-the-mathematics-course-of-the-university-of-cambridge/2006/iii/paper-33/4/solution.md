<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $e_j$ be the bit string with one in position $j$ and zero elsewhere, and use the standard convention $Y=iXZ$. On the [computational basis](../../../../../computational-basis.md), the single-site [Pauli operators](../../../../../pauli-operator.md) act as

$$
\boxed{X_j|x\rangle=|x\mathbin{\oplus}e_j\rangle,\quad Z_j|x\rangle=(-1)^{x_j}|x\rangle,\quad Y_j|x\rangle=i(-1)^{x_j}|x\mathbin{\oplus}e_j\rangle.}
$$

The identity leaves the basis state unchanged. A tensor-product [Pauli operator](../../../../../pauli-operator.md) applies these actions at each occupied site; operators at different sites commute. Their linear span is the full operator algebra, so correcting their span handles coherent combinations as well as random Pauli errors.

Let $P$ project onto the code $\mathcal C$, with orthonormal logical basis $|i_L\rangle$. A set $\mathcal E=\{E_a\}$ is correctable exactly when the [Knill--Laflamme condition](../../../../../knill-laflamme-condition.md) holds:

$$
\boxed{PE_a^\dagger E_bP=C_{ab}P,\quad\text{equivalently }\langle i_L|E_a^\dagger E_b|j_L\rangle=C_{ab}\delta_{ij},}
$$

for a matrix $C$ independent of the logical indices. A set $\mathcal D$ is detectable when

$$
\boxed{PDP=c_DP\quad\text{for every }D\in\mathcal D.}
$$

These conditions extend by linearity to the corresponding operator spans. Detection allows an error to act as a harmless scalar on the code; it need not assign a distinct syndrome to such an error.

For distinct Pauli representatives modulo phase, a [nondegenerate quantum error-correcting code](../../../../../nondegenerate-quantum-error-correcting-code.md) has orthogonal error-image subspaces, giving $C_{ab}=\delta_{ab}$ because each Pauli is unitary. In the usual nondegenerate, or pure, detection convention, every nonidentity detectable Pauli has $PDP=0$, while $PIP=P$. More generally a nonsingular error-overlap matrix can be diagonalized and the resulting error operators rescaled to obtain orthogonal syndrome spaces; a singular overlap matrix expresses degeneracy of the specified independent error family.

For an $[[n,k,d]]$ code, the [quantum code distance](../../../../../distance-of-a-quantum-error-correcting-code.md) is the smallest [Pauli weight](../../../../../weight-of-a-pauli-operator.md) for which scalar compression fails. Hence every Pauli of weight at most $d-1$ is detectable. If $E_a,E_b$ each have weight at most $t$, their product $E_a^\dagger E_b$ has weight at most $2t$. When $2t<d$, its compression is scalar, so the [Knill--Laflamme condition](../../../../../knill-laflamme-condition.md) proves simultaneous correction of all such errors. Therefore

$$
\boxed{\text{detectable weight: }d-1,\qquad\text{correctable unknown-location weight: }\left\lfloor\frac{d-1}{2}\right\rfloor.}
$$

The integer part is understood when the printed half-distance is not an integer. Arbitrary operators on such subsets are covered by their Pauli expansion.

For errors confined to a known set of $m$ positions, every pairwise product is still supported on that same set and has weight at most $m$, rather than $2m$. Thus $m<d$ supplies [quantum erasure correction](../../../../../quantum-erasure-correction.md), with maximum guaranteed number

$$
\boxed{m=d-1.}
$$

This guarantee cannot hold for every set of $d$ positions: a minimum-weight undetectable Pauli has support in such a set, and the pair consisting of it and the identity violates the [Knill--Laflamme condition](../../../../../knill-laflamme-condition.md). Particular larger location sets can sometimes be correctable; $d-1$ is the maximum uniform guarantee over all possible known sets.

For the [Shor code](../../../../../shor-code.md), write $|G_\pm\rangle=(|000\rangle\pm|111\rangle)/\sqrt2$. The logical codewords are $|G_+\rangle^{\otimes3}$ and $|G_-\rangle^{\otimes3}$. A [phase flip](../../../../../pauli-z-gate.md) $Z_j$ in one block interchanges $G_+$ and $G_-$ in that block, independently of its position within the block. Let $B_1=X_1X_2X_3$, $B_2=X_4X_5X_6$, $B_3=X_7X_8X_9$. Measure the two commuting [stabilizer generators](../../../../../stabilizer-generator.md) $S_1=B_1B_2$ and $S_2=B_2B_3$. Both are $+1$ on the entire logical code space. The [Shor-code phase-flip syndrome](../../../../../shor-code-phase-flip-syndrome.md) is

$$
\begin{array}{c|cc|c}\text{affected block}&S_1&S_2&\text{correction}\\\hline\text{none}&+1&+1&I\\1&-1&+1&Z_1\\2&-1&-1&Z_4\\3&+1&-1&Z_7\end{array}.
$$

These parity measurements reveal the erroneous block without revealing the logical amplitudes, so they preserve arbitrary superpositions of the two codewords. Applying the listed representative phase flip restores the state.

For any two physical positions $i,j$ in the same block, $Z_iZ_j$ acts as $+1$ on both $|000\rangle$ and $|111\rangle$, and hence on the code. Therefore $Z_iP=Z_jP$ and $PZ_i^\dagger Z_jP=P$ even when $i\ne j$. Their error spaces coincide, and the error-overlap matrix has a nonzero off-diagonal entry. **The correction is degenerate because different within-block phase errors have exactly the same action on every logical state.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
