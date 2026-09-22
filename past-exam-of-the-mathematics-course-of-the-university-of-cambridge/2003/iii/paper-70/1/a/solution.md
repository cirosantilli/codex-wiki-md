<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a real matrix $A$ with positive [determinant](../../../../../../determinant.md), the [polar decomposition of an invertible real matrix](../../../../../../polar-decomposition-of-an-invertible-real-matrix.md) gives unique factorizations

$$
\boxed{A=RU=VR,\qquad R\in SO(3),\quad U=U^T>0,\quad V=V^T>0,}
$$

where $U$ and $V$ are the [right stretch tensor](../../../../../../right-stretch-tensor.md) and [left stretch tensor](../../../../../../left-stretch-tensor.md), respectively. Positivity here means positive definiteness, not merely nonnegative entries.

To prove existence, $C=A^TA$ is symmetric and $v^TCv=|Av|^2>0$ for every nonzero $v$, because $A$ is invertible. The [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md) supplies an [orthogonal matrix](../../../../../../orthogonal-matrix.md) $Q$ and positive [eigenvalues](../../../../../../eigenvalue.md) $c_j$ such that $C=Q\operatorname{diag}(c_1,c_2,c_3)Q^T$. Define $U$ using the [principal square root of a positive semidefinite matrix](../../../../../../principal-square-root-of-a-positive-semidefinite-matrix.md) construction:

$$
U=Q\operatorname{diag}(\sqrt{c_1},\sqrt{c_2},\sqrt{c_3})Q^T,
\qquad R=AU^{-1}.
$$

Then $R^TR=U^{-1}A^TAU^{-1}=I$, so $R$ is orthogonal. Also $\det R=\det A/\det U>0$; an [orthogonal matrix](../../../../../../orthogonal-matrix.md) has [determinant](../../../../../../determinant.md) plus or minus one, hence $\det R=1$. Set $V=RUR^T$. It is symmetric positive definite, $V^2=AA^T$, and $VR=RU=A$.

For uniqueness, any second factorization $A=R_1U_1$ with the same properties gives $U_1^2=A^TA=C$. Since $U_1$ commutes with its square, it preserves every [eigenspace](../../../../../../eigenspace.md) of $C$. On a $c$-eigenspace its own positive [eigenvalues](../../../../../../eigenvalue.md) must square to $c$, so it equals $\sqrt c$ times the identity there. Thus $U_1=U$, then $R_1=AU^{-1}=R$, and finally $V$ is fixed too. This proves both uniqueness and the [polar decomposition in continuum mechanics](../../../../../../polar-decomposition-in-continuum-mechanics.md), with the same proper rotation in its left and right forms.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
