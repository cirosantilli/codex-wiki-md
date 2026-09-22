<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose [Kraus representations](../../../../../../kraus-representation.md)

$$
\mathcal C(L)=\sum_a C_aLC_a^\dagger,\qquad
\mathcal D(M)=\sum_b D_bMD_b^\dagger,\qquad
\sum_aC_a^\dagger C_a=I_Q,\quad\sum_bD_b^\dagger D_b=I_K.
$$

The composite [quantum channel](../../../../../../quantum-channel.md) has [Kraus operators](../../../../../../kraus-operator.md) $T_{ba}=D_bC_a$. Each has [matrix rank](../../../../../../matrix-rank.md) at most $k$, because it factors through the $k$-dimensional space $K$, and

$$
\sum_{a,b}T_{ba}^\dagger T_{ba}=I_Q.
$$

The [operation fidelity](../../../../../../operation-fidelity.md) uses the unsquared [quantum fidelity](../../../../../../fidelity-of-quantum-states.md) on a [purification of a density operator](../../../../../../purification-of-a-density-operator.md), so its square is [entanglement fidelity](../../../../../../entanglement-fidelity.md). The [Kraus formula for entanglement fidelity](../../../../../../kraus-formula-for-entanglement-fidelity.md) gives

$$
F_{\rm op}(\mathcal D\mathcal C,\rho_Q)^2
=\sum_{a,b}|\operatorname{Tr}(\rho_Q T_{ba})|^2.
$$

Indeed each overlap $\langle\Psi_\rho|(I_R\otimes T_{ba})|\Psi_\rho\rangle$ equals $\operatorname{Tr}(\rho_QT_{ba})$.

For any one of these [Kraus operators](../../../../../../kraus-operator.md) $T$, let $\Pi_T$ be the [orthogonal projection](../../../../../../orthogonal-projection.md) onto its image, of [matrix rank](../../../../../../matrix-rank.md) $r_T\leq k$. Since $\Pi_TT=T$, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) for the [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md) gives the [rank bound for a weighted operator trace](../../../../../../rank-bound-for-a-weighted-operator-trace.md):

$$
\begin{aligned}
|\operatorname{Tr}(\rho_QT)|^2
&=|\operatorname{Tr}[(\Pi_T\sqrt{\rho_Q})^\dagger(T\sqrt{\rho_Q})]|^2\\
&\leq\operatorname{Tr}(\rho_Q\Pi_T)\operatorname{Tr}(\rho_QT^\dagger T)\\
&\leq\left(\sum_{j<k}\lambda_j\right)\operatorname{Tr}(\rho_QT^\dagger T).
\end{aligned}
$$

The last step uses part (i) at $r_T$, followed by nonnegativity of the [eigenvalues](../../../../../../eigenvalue.md) of the [density operator](../../../../../../density-matrix.md) $\rho_Q$. Summing over the [Kraus operators](../../../../../../kraus-operator.md) and using their completeness relation proves **the [finite-dimensional quantum compression converse](../../../../../../finite-dimensional-quantum-compression-converse.md)**:

$$
\boxed{1-\epsilon\leq F_{\rm op}(\mathcal D\mathcal C,\rho_Q)^2\leq\sum_{j<k}\lambda_j.}
$$

No invertibility of $\rho_Q$, or restriction to an isometric decoder, was used.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
