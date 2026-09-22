<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $P$ be the [orthogonal projector](../../../../../../orthogonal-projection.md) onto the [quantum code](../../../../../../quantum-error-correcting-code.md) $\mathcal X$, and choose an [orthonormal basis](../../../../../../orthonormal-basis.md) $|i_L\rangle$ for it. The necessary and sufficient [Knill--Laflamme condition](../../../../../../knill-laflamme-condition.md) is that one [matrix](../../../../../../matrix.md) $C$, independent of the logical labels, satisfies

$$
\boxed{PE_a^\dagger E_bP=C_{ab}P\quad\text{for all }E_a,E_b\in\mathcal E.}
$$

Equivalently, $\langle i_L|E_a^\dagger E_b|j_L\rangle=C_{ab}\delta_{ij}$. This makes the information in the error label independent of the encoded [quantum state](../../../../../../quantum-state.md). It applies to the whole linear span of the errors, and hence to every noise [quantum channel](../../../../../../quantum-channel.md) with [Kraus operators](../../../../../../kraus-operator.md) in that span.

Here is a proof of both directions. For [necessity of the Knill-Laflamme condition](../../../../../../necessity-of-the-knill-laflamme-condition.md), let $R_\mu$ be [Kraus operators](../../../../../../kraus-operator.md) of a common recovery, so $\sum_\mu R_\mu^\dagger R_\mu=I$. Since recovery after $E_a$ must return the pure input state, every vector $R_\mu E_a|\psi\rangle$ is parallel to $|\psi\rangle$. A [linear operator](../../../../../../linear-operator.md) on the code which sends every vector to a multiple of itself is scalar: apply it to two basis vectors and their sum to force the two multipliers to agree. Therefore $R_\mu E_aP=c_{\mu a}P$ with no dependence on $|\psi\rangle$. It follows that

$$
PE_a^\dagger E_bP=\sum_\mu PE_a^\dagger R_\mu^\dagger R_\mu E_bP
=\sum_\mu c_{\mu a}^*c_{\mu b}P.
$$

This proves necessity without assuming in advance that the physical errors have orthogonal syndromes.

For sufficiency, $C$ is [positive semidefinite](../../../../../../positive-semidefinite-matrix.md): for any normalized code state and coefficients $v_a$, $v^\dagger Cv=\|\sum_a v_aE_a|\psi\rangle\|^2\geq0$. Diagonalize $C$ by a unitary change of the error basis to get operators $F_j$ with $PF_j^\dagger F_lP=c_j\delta_{jl}P$. If $c_j>0$, $V_j=F_jP/\sqrt{c_j}$ is a [linear isometry](../../../../../../linear-isometry-of-hilbert-spaces.md) from the code to an error-image subspace, and distinct such images are orthogonal. If $c_j=0$, then $F_jP=0$. A [projective measurement](../../../../../../projective-measurement.md) of these image subspaces followed by $V_j^\dagger$ recovers every logical state. Complete the recovery on the unused orthogonal complement in any trace-preserving manner. For a coherent error $\sum_jv_jF_j$, the measurement branch $j$ contains $v_j\sqrt{c_j}|\psi\rangle$; the branch probability is independent of the logical state, and discarding the syndrome leaves the original state. This is [constructive recovery from the Knill-Laflamme condition](../../../../../../constructive-recovery-from-the-knill-laflamme-condition.md).

For the usual family of distinct unitary [Pauli errors](../../../../../../pauli-operator.md) modulo scalar phase, [nondegenerate quantum code](../../../../../../nondegenerate-quantum-error-correcting-code.md) correction means that different physical errors have orthogonal image subspaces. The precise condition is

$$
\boxed{C_{ab}=\delta_{ab},\qquad
\langle i_L|E_a^\dagger E_b|j_L\rangle=\delta_{ab}\delta_{ij}.}
$$

For nonunitary errors, replace the unit diagonal by positive norm factors. In an arbitrary error basis the Gram matrix need not initially be diagonal; its positive-eigenvalue modes give the independent syndrome spaces just constructed. A kernel of $C$ exhibits a linear combination of errors acting as zero on the code. In particular two distinct physical errors with the same action on the code cannot be distinguished and give degenerate correction, as in part (c).

## ↑ Ancestors (11)

1. [A](../a.md)
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
