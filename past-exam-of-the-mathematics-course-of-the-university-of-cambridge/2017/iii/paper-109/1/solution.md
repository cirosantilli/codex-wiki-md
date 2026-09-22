<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $D=\sum_{i=1}^n b_i$ and let $\lambda$ denote [Lebesgue measure](../../../../../lebesgue-measure.md). Necessity follows from [measure](../../../../../measure.md) additivity and monotonicity: the pairwise disjoint [Lebesgue measurable sets](../../../../../lebesgue-measurable-set.md) $B_i$ give

$$
\lambda\!\left(\bigcup_{i\in I}A_i\right)\geq\lambda\!\left(\bigcup_{i\in I}B_i\right)=\sum_{i\in I}b_i.
$$

For sufficiency, form the finite [measurable partition](../../../../../measurable-partition.md) into membership cells

$$
E_J=\left(\bigcap_{j\in J}A_j\right)\setminus\left(\bigcup_{j\notin J}A_j\right),\qquad \varnothing\ne J\subseteq[n].
$$

These [Lebesgue measurable sets](../../../../../lebesgue-measurable-set.md) are pairwise disjoint, and $A_i=\bigcup_{J\ni i}E_J$. Empty cells may be retained. Construct a [flow network](../../../../../flow-network.md) with a source, one vertex for each index $i$, one vertex for each cell $E_J$, and a sink. Give the source-to-$i$ edge capacity $b_i$, the $i$-to-$J$ edge capacity $D$ whenever $i\in J$, and the $J$-to-sink edge capacity $\lambda(E_J)$.

Consider any [cut of a flow network](../../../../../cut-of-a-flow-network.md), and let $I$ be its index vertices on the source side. If an index-to-cell edge crosses the [cut of a flow network](../../../../../cut-of-a-flow-network.md), its capacity alone is $D$. Otherwise every cell with $J\cap I\ne\varnothing$ lies on the source side, so the [cut of a flow network](../../../../../cut-of-a-flow-network.md) has capacity at least

$$
\sum_{i\notin I}b_i+\sum_{J:J\cap I\ne\varnothing}\lambda(E_J)=D-\sum_{i\in I}b_i+\lambda\!\left(\bigcup_{i\in I}A_i\right)\geq D.
$$

The cut immediately after the source has capacity $D$. The [max-flow min-cut theorem](../../../../../max-flow-min-cut-theorem.md), valid for finite [flow networks](../../../../../flow-network.md) with real capacities, therefore supplies a flow of value $D$. Its cell allocations $f_{iJ}\geq0$ satisfy

$$
\sum_{J\ni i}f_{iJ}=b_i,\qquad \sum_{i\in J}f_{iJ}\leq\lambda(E_J).
$$

It remains to convert these numbers into [Lebesgue measurable sets](../../../../../lebesgue-measurable-set.md); this uses [divisibility of Lebesgue measure](../../../../../divisibility-of-lebesgue-measure.md). Indeed, for any [Lebesgue measurable set](../../../../../lebesgue-measurable-set.md) $E\subseteq[0,1]$, the function $F(t)=\lambda(E\cap[0,t])$ satisfies $F(0)=0$, $F(1)=\lambda(E)$ and $|F(t)-F(u)|\leq|t-u|$. Thus it has [Lipschitz continuity](../../../../../lipschitz-continuity.md), and the [intermediate value theorem](../../../../../intermediate-value-theorem.md) supplies a measurable [subset](../../../../../subset.md) of $E$ of any prescribed measure between $0$ and $\lambda(E)$. Successively apply this to the remaining portion of each $E_J$, choosing disjoint pieces $E_{iJ}$ of measure $f_{iJ}$; choose the empty [set](../../../../../set-split.md) when $f_{iJ}=0$. Then

$$
\boxed{B_i=\bigcup_{J\ni i}E_{iJ}\subseteq A_i,\qquad \lambda(B_i)=b_i,\qquad B_i\cap B_j=\varnothing\ (i\ne j).}
$$

This proves the [measurable Hall theorem](../../../../../measurable-hall-theorem.md). The splitting step is essential: an arbitrary [measure](../../../../../measure.md) with an [atom of a measure](../../../../../atom-measure-theory.md) would not support the same conclusion. Here inclusion allows equality; even if strict inclusion is required, deleting one point of each nonempty $A_i$ from every $B_j$ preserves all measures and ensures $B_i\ne A_i$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 109](../../paper-109-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
