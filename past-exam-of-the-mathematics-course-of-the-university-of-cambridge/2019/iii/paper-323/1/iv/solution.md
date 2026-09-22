<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use the normalized [Choi state](../../../../../../choi-state.md) $C_\Lambda=(\Lambda\otimes\operatorname{id})(|\Phi_d\rangle\langle\Phi_d|)$, with $|\Phi_d\rangle=d^{-1/2}\sum_i|ii\rangle$. If $\Lambda$ is an [entanglement-breaking channel](../../../../../../entanglement-breaking-channel.md), its action on this particular bipartite input makes $C_\Lambda$ a [separable quantum state](../../../../../../separable-quantum-state.md).

Conversely, suppose $C_\Lambda=\sum_ap_a\sigma_a\otimes\tau_a$, with local [density operators](../../../../../../density-matrix.md) $\sigma_a,\tau_a$. The [Choi reconstruction formula](../../../../../../choi-reconstruction-formula.md) gives

$$
\Lambda(X)=d\operatorname{Tr}_B\left[C_\Lambda(I\otimes X^T)\right]
=\sum_a\operatorname{Tr}(E_aX)\sigma_a,\qquad E_a=dp_a\tau_a^T\geq0.
$$

Because $\Lambda$ is trace preserving, $\operatorname{Tr}_A C_\Lambda=I/d$, so $\sum_aE_a=I$. Thus the $E_a$ form a [POVM](../../../../../../positive-operator-valued-measure.md) and the channel is a [measure-and-prepare channel](../../../../../../measure-and-prepare-channel.md).

For any bipartite input $\rho_{AR}$, define the positive, possibly unnormalized reference operators

$$
R_a=\operatorname{Tr}_A\left[(\sqrt{E_a}\otimes I)\rho_{AR}(\sqrt{E_a}\otimes I)\right].
$$

Its output is $\sum_a\sigma_a\otimes R_a$. Since $\sum_a\operatorname{Tr}R_a=1$, normalizing each nonzero $R_a$ expresses this as a [convex combination](../../../../../../convex-combination.md) of [product states](../../../../../../product-state.md). Hence every output is separable, proving the [separable Choi-state criterion for entanglement breaking](../../../../../../separable-choi-state-criterion-for-entanglement-breaking.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
