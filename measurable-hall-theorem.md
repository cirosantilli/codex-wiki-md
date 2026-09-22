# Measurable Hall theorem

↑ **Parent:** [Hall's marriage theorem](hall-s-marriage-theorem.md)

For finitely many [Lebesgue measurable sets](lebesgue-measurable-set.md) $A_i\subseteq[0,1]$ and nonnegative demands $b_i$, pairwise disjoint measurable [subsets](subset.md) $B_i\subseteq A_i$ with $\lambda(B_i)=b_i$ exist exactly when $\lambda(\bigcup_{i\in I}A_i)\geq\sum_{i\in I}b_i$ for every index [subset](subset.md) $I$. Necessity is additivity and monotonicity of [Lebesgue measure](lebesgue-measure.md). For sufficiency, partition the [set union](set-union.md) into membership cells $E_J$, send flow from a source through demand vertices $i$ to cells with $i\in J$, then to a sink. Source capacities are $b_i$, cell capacities are $\lambda(E_J)$, and intermediate capacities are $D=\sum_i b_i$. Every [cut of a flow network](cut-of-a-flow-network.md) has capacity at least $D$ by the assumed inequalities. The [max-flow min-cut theorem](max-flow-min-cut-theorem.md) provides the allocations, and [divisibility of Lebesgue measure](divisibility-of-lebesgue-measure.md) turns each cell allocation into disjoint pieces. If $D=0$, all $B_i$ can simply be empty.

## ↑ Ancestors (7)

1. [Hall's marriage theorem](hall-s-marriage-theorem.md)
2. [Matching (graph theory)](matching-graph-theory.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-109/1/solution.md)
