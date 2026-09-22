<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Schrödinger–Jaynes–Hughston–Jozsa–Wootters theorem](../../../../../hughston-jozsa-wootters-theorem.md) classifies all finite [quantum state ensembles](../../../../../quantum-state-ensemble.md) of a [density matrix](../../../../../density-matrix.md). Write its nonzero spectral decomposition as $\rho=\sum_{a=1}^r\lambda_a|e_a\rangle\langle e_a|$, with $\lambda_a>0$ and orthonormal [eigenvectors](../../../../../eigenvector.md). An ensemble with subnormalized vectors $|w_j\rangle=\sqrt{p_j}|\phi_j\rangle$, $j=1,\ldots,m$, represents $\rho$ exactly when

$$
\boxed{|w_j\rangle=\sum_{a=1}^rU_{ja}\sqrt{\lambda_a}|e_a\rangle,\qquad U^\dagger U=I_r.}
$$

Here $U$ is an $m\times r$ column [linear isometry](../../../../../linear-isometry-of-hilbert-spaces.md). Zero-weight vectors may be included or discarded. Equivalently, any two ensembles represent the same [density matrix](../../../../../density-matrix.md) if and only if, after padding the shorter list with zero vectors, their subnormalized vectors are related by a [unitary matrix](../../../../../unitary-matrix.md) acting on the ensemble index. This is the [isometry parametrization of a density-matrix ensemble](../../../../../isometry-parametrization-of-a-density-matrix-ensemble.md).

For necessity, if $|v\rangle$ lies in the kernel of $\rho$, then

$$
0=\langle v|\rho|v\rangle=\sum_j|\langle v|w_j\rangle|^2.
$$

Every $w_j$ therefore lies in the support of $\rho$. Define $U_{ja}=\langle e_a|w_j\rangle/\sqrt{\lambda_a}$. The ensemble identity gives

$$
\sum_jU_{ja}^*U_{jb}
=\frac{\langle e_b|\rho|e_a\rangle}{\sqrt{\lambda_a\lambda_b}}
=\delta_{ab},
$$

so these columns are orthonormal and the displayed parametrization follows.

Conversely, start with any such isometry and define $w_j$ by the boxed equation. Then

$$
\sum_j|w_j\rangle\langle w_j|
=\sum_{a,b}\sqrt{\lambda_a\lambda_b}\left(\sum_jU_{ja}U_{jb}^*\right)|e_a\rangle\langle e_b|
=\rho.
$$

The weights are $p_j=\|w_j\|^2=\sum_a\lambda_a|U_{ja}|^2\geq0$ and sum to $\operatorname{Tr}\rho=1$. Normalize every nonzero $w_j$ to obtain its [pure state](../../../../../pure-state.md). This proves both directions and includes degenerate [eigenvalues](../../../../../eigenvalue.md) without any preferred choice of basis in their eigenspaces.

To prove the unitary-mixing version, pad two ensembles to a common length $L$. Their matrices $U$ and $V$ have $r$ orthonormal columns in $\mathbb C^L$. Extend each column family to an [orthonormal basis](../../../../../orthonormal-basis.md), obtaining square unitaries $\widetilde U$ and $\widetilde V$. Then $W=\widetilde V\widetilde U^\dagger$ is unitary and $V=WU$, so the second ensemble vectors satisfy $v_k=\sum_jW_{kj}w_j$. Conversely this unitary mixing preserves $\sum_j|w_j\rangle\langle w_j|$, because $\sum_kW_{ki}W_{kj}^*=\delta_{ij}$. Independent phase choices for ensemble kets are absorbed in the row phases of these matrices.

The classification also has a measurement interpretation. Purify $\rho$ as $|\Psi\rangle=\sum_a\sqrt{\lambda_a}|e_a\rangle|a\rangle$. On the ancillary system define $|\eta_j\rangle=\sum_aU_{ja}^*|a\rangle$. The effects $E_j=|\eta_j\rangle\langle\eta_j|$ sum to $I_r$, hence form a [POVM](../../../../../positive-operator-valued-measure.md). The conditional unnormalized system ket is $(I\otimes\langle\eta_j|)|\Psi\rangle=w_j$, with [probability](../../../../../probability.md) $p_j$. Thus every ensemble can be realized by measuring a purifying system; with a sufficiently enlarged ancilla the measurement can be projective. The [density matrix](../../../../../density-matrix.md) specifies the common statistics without selecting one particular ensemble decomposition.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
