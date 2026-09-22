<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

First give $w$ the vote of every voter whose allowed [set](../../../../../set-split.md) contains $w$. Let their number be $K$. This loses no possible strict victory: starting with any winning assignment, changing such a ballot to $w$ increases $w$'s score and weakly decreases an opponent's score. Thus a winning assignment exists exactly when one exists with these $K$ ballots fixed.

Every remaining voter must now be assigned to an allowed opponent, and **each opponent may receive at most $K-1$ votes**. If any allowed [set](../../../../../set-split.md) is empty, there is no valid election assignment. With at least two candidates, $K=0$ immediately makes a unique victory impossible. With only the candidate $w$, every nonempty ballot [set](../../../../../set-split.md) forces that candidate, so the answer is yes under the question's strict-comparison definition.

For the remaining case $K\geq1$, make a [flow network](../../../../../flow-network-split.md) with a [vertex](../../../../../vertex-graph-theory.md) for each remaining voter and each opponent. Add source-to-voter arcs of [flow network edge capacity](../../../../../flow-network-edge-capacity.md) one, voter-to-opponent arcs of [flow network edge capacity](../../../../../flow-network-edge-capacity.md) one for the allowed choices, and opponent-to-sink arcs of [flow network edge capacity](../../../../../flow-network-edge-capacity.md) $K-1$. Compute an integral [maximum flow](../../../../../maximum-flow-problem.md). Then

$$
\boxed{w\text{ can be the unique winner}\iff |f_{\max}|=n-K.}
$$

A [flow](../../../../../flow.md) saturating all voter arcs assigns each remaining voter to exactly one allowed opponent, by integrality and [flow conservation](../../../../../flow-conservation.md). The sink-arc [capacity constraints](../../../../../capacity-constraint.md) give every opponent strictly fewer than $K$ votes. Conversely, any winning assignment with the fixed $K$ votes defines just such a saturating [feasible flow](../../../../../feasible-flow.md). The [flow network](../../../../../flow-network-split.md) has at most $n+m+2$ [vertices](../../../../../vertex-graph-theory.md) and $O(n+m+\sum_i|C_i|)$ arcs, hence the decision takes [polynomial time](../../../../../polynomial-time.md).

## ↑ Ancestors (11)

1. [E](../e.md)
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
