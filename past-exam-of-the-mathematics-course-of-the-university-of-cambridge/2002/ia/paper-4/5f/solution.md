<h1 id="5f/solution">Solution</h1>

↑ **Parent:** [5F](../5f.md)

A [set](../../../../../set-split.md) is [countable](../../../../../countable-set.md) if it is finite or admits an [injection](../../../../../injective-function.md) into the natural numbers; an infinite [countable set](../../../../../countable-set.md) can equivalently be listed as a sequence. Let $A=\bigcup_{i\ge1}A_i$ with each $A_i$ [countable](../../../../../countable-set.md). Choose an enumeration of each nonempty $A_i$, allowing repetition if it is finite. List the pairs $(i,j)\in\mathbb N^2$ in successive finite diagonals of constant $i+j$ and output the $j$th member of $A_i$. This lists every member of $A$, so $A$ is [countable](../../../../../countable-set.md); empty sets contribute nothing, and repetitions can be removed by retaining first occurrences. This is the [countable union of countable sets](../../../../../countable-union-of-countable-sets.md) theorem, in the usual setting with [axiom of countable choice](../../../../../axiom-of-countable-choice.md) for selecting the enumerations.

Each positive-length interval $J_i$ has a nonempty interior containing a [rational number](../../../../../rational-number.md) by the [density of the rational numbers](../../../../../density-of-the-rational-numbers.md). Fix one enumeration of the [rational numbers](../../../../../rational-number.md) and let $q_i$ be its first member in the interior of $J_i$. Disjointness gives $i\ne j\Rightarrow q_i\ne q_j$, so $i\mapsto q_i$ is an [injection](../../../../../injective-function.md) of $I$ into a [countable set](../../../../../countable-set.md). Hence $I$ is [countable](../../../../../countable-set.md). This proof of the [countability of disjoint positive-length intervals](../../../../../countability-of-disjoint-positive-length-intervals.md) uses a fixed enumeration and needs no arbitrary simultaneous choice of rationals.

## ↑ Ancestors (10)

1. [5F](../5f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
