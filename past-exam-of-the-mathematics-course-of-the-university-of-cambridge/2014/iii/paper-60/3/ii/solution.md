<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $K_y=|y\rangle\langle y|$. The map is in [Kraus representation](../../../../../../kraus-representation.md):

$$
\Lambda(X)=\sum_yK_yXK_y^\dagger,\qquad
\sum_yK_y^\dagger K_y=\sum_y|y\rangle\langle y|=I.
$$

For any ancillary [Hilbert space](../../../../../../hilbert-space-split.md) $R$ and positive operator $M$ on $R\otimes\mathcal H$,

$$
(\operatorname{id}_R\otimes\Lambda)(M)=\sum_y(I_R\otimes K_y)M(I_R\otimes K_y^\dagger)\geq0.
$$

This verifies complete positivity directly, not merely positivity on unextended states. Cyclicity of the trace gives $\operatorname{Tr}\Lambda(X)=\operatorname{Tr}[X\sum_yK_y^\dagger K_y]=\operatorname{Tr}X$. Thus **$\Lambda$ is a [CPTP map](../../../../../../quantum-channel.md)**, the [completely dephasing channel](../../../../../../rank-one-dephasing.md) in the given basis.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
