<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The unbroken [group](../../../../group-split.md) is the [stabilizer subgroup](../../../../stabilizer-subgroup.md) of the [vacuum expectation value](../../../../vacuum-expectation-value.md). For a nonzero vector [vacuum expectation value](../../../../vacuum-expectation-value.md), an [orthogonal transformation](../../../../orthogonal-transformation.md) puts $\langle\phi\rangle=v e_N$. A special orthogonal transformation fixing it has the block form $\operatorname{diag}(A,1)$ with $A\in\operatorname{SO}(N-1)$. Consequently

$$
\boxed{\operatorname{SO}(N)\longrightarrow\operatorname{SO}(N-1)\quad(v\ne0).}
$$

The zero [vacuum expectation value](../../../../vacuum-expectation-value.md) leaves the entire [special orthogonal group](../../../../special-orthogonal-group.md) unbroken.

For a real [symmetric tensor](../../../../symmetric-tensor.md) write its [vacuum expectation value](../../../../vacuum-expectation-value.md) as a real [symmetric matrix](../../../../symmetric-matrix.md) $Q$. The transformation is $Q\mapsto OQO^T$. The [spectral theorem for real symmetric matrices](../../../../spectral-theorem-for-real-symmetric-matrices.md) gives an orthonormal [basis](../../../../basis.md) in which

$$
Q=\operatorname{diag}(q_1I_{m_1},\ldots,q_pI_{m_p}),\qquad q_i\ne q_j\ (i\ne j),\qquad \sum_i m_i=N.
$$

Because $OQO^T=Q$ is equivalent to $OQ=QO$, an unbroken transformation preserves each [eigenspace](../../../../eigenspace.md). The complete unbroken [group](../../../../group-split.md) is therefore

$$
\boxed{H=S\bigl(O(m_1)\times\cdots\times O(m_p)\bigr)
=\{(A_1,\ldots,A_p):\prod_i\det A_i=1\}.}
$$

Its [identity component](../../../../identity-component.md) is $H^0=\prod_i\operatorname{SO}(m_i)$. This [symmetric tensor vacuum stabilizer](../../../../symmetric-tensor-vacuum-stabilizer.md) shows why the [representation](../../../../group-representation.md) alone does not determine a unique breaking pattern:

- If $Q=qI$, all of $\operatorname{SO}(N)$ survives, even when $q\ne0$.
- If all [eigenvalues](../../../../eigenvalue.md) are distinct, $H\cong(\mathbb Z/2\mathbb Z)^{N-1}$, consisting of diagonal sign changes with total sign $+1$; no continuous symmetry survives.
- If the two [eigenvalue multiplicities](../../../../eigenvalue-multiplicity.md) are $m$ and $N-m$, then $H=S(O(m)\times O(N-m))$, with [identity component](../../../../identity-component.md) $\operatorname{SO}(m)\times\operatorname{SO}(N-m)$.

For example a rank-one tensor $Q=ve_Ne_N^T$ preserves $O(N-1)$ embedded by $A\mapsto\operatorname{diag}(A,\det A)$. Its continuous unbroken [group](../../../../group-split.md) is $\operatorname{SO}(N-1)$, but it also allows reversal of the distinguished axis. Restricting to a traceless [symmetric tensor](../../../../symmetric-tensor.md) imposes $\sum_i m_iq_i=0$ and otherwise leaves the same classification.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
