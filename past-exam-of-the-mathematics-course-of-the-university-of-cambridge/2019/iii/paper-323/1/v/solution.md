<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Apply the [measure-and-prepare channel](../../../../../../measure-and-prepare-channel.md) locally to an arbitrary bipartite [density operator](../../../../../../density-matrix.md) $\rho_{AR}$. The resulting state is

$$
(\Lambda\otimes\operatorname{id}_R)(\rho_{AR})=\sum_a\sigma_a\otimes R_a,
$$

where

$$
R_a=\operatorname{Tr}_A\left[(\sqrt{E_a}\otimes I)\rho_{AR}(\sqrt{E_a}\otimes I)\right]\geq0.
$$

To see that this is the correct output, the [partial trace](../../../../../../partial-trace.md) is cyclic for operators acting only on the traced subsystem, so the displayed expression equals $\operatorname{Tr}_A[(E_a\otimes I)\rho_{AR}]$. Put $q_a=\operatorname{Tr}R_a$. The [POVM](../../../../../../positive-operator-valued-measure.md) completeness relation implies $\sum_aq_a=1$, and terms with $q_a=0$ vanish. Therefore

$$
(\Lambda\otimes\operatorname{id}_R)(\rho_{AR})
=\sum_{a:q_a>0}q_a\sigma_a\otimes\frac{R_a}{q_a}
$$

is a [separable quantum state](../../../../../../separable-quantum-state.md). Thus the channel is an [entanglement-breaking channel](../../../../../../entanglement-breaking-channel.md), for every reference-system dimension.

## ↑ Ancestors (11)

1. [V](../v.md)
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
