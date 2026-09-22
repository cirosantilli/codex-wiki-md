<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write a bipartite [pure state](../../../../../../pure-state.md) in fixed product bases as $|\psi\rangle=\sum_{ij}M_{ij}|i\rangle|j\rangle$. The [Schmidt decomposition theorem](../../../../../../schmidt-decomposition.md), equivalently the [singular value decomposition](../../../../../../singular-value-decomposition.md) of $M$, says that its [Schmidt rank](../../../../../../schmidt-rank.md) equals $\operatorname{rank}M$. A branch of local operations is a product operator $A\otimes B$, so its coefficient matrix is

$$
M'=AMB^{\mathsf T}.
$$

The elementary rank inequality $\operatorname{rank}(AMB^{\mathsf T})\leq\operatorname{rank}M$ proves [Schmidt-rank contraction under product operators](../../../../../../schmidt-rank-contraction-under-product-operators.md). Normalizing a nonzero branch does not change matrix rank.

For an adaptive [LOCC](../../../../../../local-operations-and-classical-communication.md) protocol, a complete classical transcript selects one local [Kraus operator](../../../../../../kraus-operator.md) at each stage. Multiplying the local operators along that transcript still gives one product $A_t\otimes B_t$. Consequently

$$
\boxed{\operatorname{Schmidt\ rank}(\psi_t)\leq
\operatorname{Schmidt\ rank}(\psi)\quad\text{in every nonzero branch}.}
$$

Classical communication changes which product operator is chosen, not this rank bound. If the overall output is a [pure state](../../../../../../pure-state.md), every nonzero branch must be proportional to that same vector, so its [Schmidt rank](../../../../../../schmidt-rank.md) also cannot increase. If the outcome is discarded and the output is mixed, pure-state [Schmidt rank](../../../../../../schmidt-rank.md) is not defined; the induced decomposition instead shows that its [Schmidt number](../../../../../../schmidt-number.md) is at most the original rank. This includes probabilistic filtering as well as deterministic pure-state conversion.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
