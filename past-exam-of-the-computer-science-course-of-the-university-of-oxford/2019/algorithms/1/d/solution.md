<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Separate the forced [integer](../../../../../integer-split.md) portion from the choice of rounding direction. Put $p_{ij}=\lfloor a_{ij}\rfloor$ and $q_{ij}=a_{ij}-p_{ij}$. Define residual demands

$$
r_i=\sum_jq_{ij}=\sum_ja_{ij}-\sum_jp_{ij},\qquad c_j=\sum_iq_{ij}=\sum_ia_{ij}-\sum_ip_{ij}.
$$

These are [nonnegative integers](../../../../../natural-number.md), since the original row and column [sums](../../../../../sum.md) are [integers](../../../../../integer-split.md). Also $\sum_ir_i=\sum_jc_j=:T$. Each [fractional part](../../../../../fractional-part.md) satisfies $0\leq q_{ij}<1$.

Construct a [flow network](../../../../../flow-network-split.md) with a [vertex](../../../../../vertex-graph-theory.md) for each row and column, source-to-row arcs of [flow network edge capacity](../../../../../flow-network-edge-capacity.md) $r_i$, row-to-column arcs of [flow network edge capacity](../../../../../flow-network-edge-capacity.md) one exactly where $q_{ij}>0$, and column-to-sink arcs of [flow network edge capacity](../../../../../flow-network-edge-capacity.md) $c_j$. The amounts $q_{ij}$ themselves define a fractional [feasible flow](../../../../../feasible-flow.md) of [flow value](../../../../../strength-of-a-flow.md) $T$. No [flow](../../../../../flow.md) can exceed $T$, the total source [flow network edge capacity](../../../../../flow-network-edge-capacity.md). Because all constructed [flow network edge capacities](../../../../../flow-network-edge-capacity.md) are [integers](../../../../../integer-split.md), an integral [maximum flow](../../../../../maximum-flow-problem.md) also has [flow value](../../../../../strength-of-a-flow.md) $T$ and saturates every source and sink arc.

Let $h_{ij}$ be its middle-arc [flow](../../../../../flow.md), taking $h_{ij}=0$ when that arc is absent. Then $h_{ij}\in\{0,1\}$, and the required answer is

$$
\boxed{b_{ij}=\lfloor a_{ij}\rfloor+h_{ij}.}
$$

At an already integral entry no middle arc exists, so that entry stays fixed. At a nonintegral entry the two possibilities are precisely its [floor](../../../../../floor-function.md) and [ceiling](../../../../../ceiling-function.md). [Flow conservation](../../../../../flow-conservation.md) gives $\sum_jh_{ij}=r_i$ and $\sum_ih_{ij}=c_j$, preserving every original row and column [sum](../../../../../sum.md).

This is [matrix rounding with fixed margins](../../../../../matrix-rounding-with-fixed-margins.md). There are $m+n+2$ [vertices](../../../../../vertex-graph-theory.md) and at most $mn+m+n$ arcs. Exact [rational arithmetic](../../../../../rational-arithmetic.md) computes the [floors](../../../../../floor-function.md) and residual demands in [polynomial time](../../../../../polynomial-time.md) in the encoded input length; the resulting [flow network edge capacities](../../../../../flow-network-edge-capacity.md) are small [integers](../../../../../integer-split.md), so there is no need to scale by a potentially large common denominator.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
