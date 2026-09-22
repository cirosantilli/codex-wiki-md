<h1 id="1/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Expanding the normalized [maximally entangled state](../../../../../../maximally-entangled-state.md) in the definition of the [Choi state](../../../../../../choi-state.md) gives

$$
C_{\widetilde\Lambda}
=\frac1d\sum_{k,\ell}\widetilde\Lambda(|k\rangle\langle\ell|)\otimes|k\rangle\langle\ell|
=\boxed{\sum_jp_j|a_j\rangle\langle a_j|\otimes|\overline{b_j}\rangle\langle\overline{b_j}|}.
$$

Here the bar denotes componentwise [complex conjugation](../../../../../../complex-conjugation.md) in the basis defining the [Choi state](../../../../../../choi-state.md). Every term is a positive [tensor-product operator](../../../../../../tensor-product-operator.md), and the whole operator has trace one because $\widetilde\Lambda$ is assumed to be a [quantum channel](../../../../../../quantum-channel.md). It is therefore a [separable quantum state](../../../../../../separable-quantum-state.md), proving entanglement breaking by the [separable Choi-state criterion for entanglement breaking](../../../../../../separable-choi-state-criterion-for-entanglement-breaking.md).

If the vectors are unit vectors, the displayed $p_j$ are already the product-state weights. If they are not normalized, absorb their squared norms into the weights and normalize the nonzero vectors. Trace preservation requires

$$
d\sum_jp_j\lVert a_j\rVert^2|b_j\rangle\langle b_j|=I;
$$

the probability-distribution condition alone would not guarantee this. Equivalently, the [Kraus operators](../../../../../../kraus-operator.md) are $K_j=\sqrt{dp_j}|a_j\rangle\langle b_j|$, exhibiting the [rank-one Kraus representation of an entanglement-breaking channel](../../../../../../rank-one-kraus-representation-of-an-entanglement-breaking-channel.md).

## ↑ Ancestors (11)

1. [Vi](../vi.md)
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
