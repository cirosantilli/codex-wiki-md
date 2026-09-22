<h1 id="20d/solution">Solution</h1>

↑ **Parent:** [20D](../20d.md)

Start with a feasible [network flow](../../../../../flow.md), meaning capacity bounds and flow conservation at every vertex other than source and sink. Its [residual network](../../../../../residual-network.md) has, for an arc with capacity $c$ and current flow $f$, a forward residual capacity $c-f$ and a reverse residual capacity $f$. A reverse arc allows earlier flow to be cancelled. The [Ford-Fulkerson algorithm](../../../../../ford-fulkerson-algorithm.md) repeatedly finds a residual source-to-sink [augmenting path](../../../../../augmenting-path.md), takes the smallest residual capacity $\delta$ on it, and augments by $\delta$, increasing forward flows and decreasing reverse flows as appropriate. Feasibility is preserved and the total flow increases by $\delta$.

For rational capacities and initial flows, choose one common denominator $D$ and scale all quantities by $D$. Every residual capacity and augmentation is then integral; each augmentation increases the integer-valued flow by at least one. The flow value is bounded by the finite sum of capacities out of the source, so termination occurs after finitely many augmentations. When no residual path remains, let $U$ be the vertices reachable from the source. Every original arc leaving $U$ is saturated and every original arc entering $U$ carries zero flow, or its reverse arc would extend reachability. Conservation then makes the flow value equal to the capacity of the cut $(U,U^c)$. Every feasible flow is bounded by that cut capacity. Thus **the terminating flow is globally optimal**, proving the needed [max-flow min-cut theorem](../../../../../max-flow-min-cut-theorem.md) conclusion.

For the given directed graph, begin at zero. One valid sequence of augmentations is:

| Residual path | Added flow | Cumulative value |
| --- | --- | --- |
| S–A–B–T | 6 | 6 |
| S–D–C–T | 10 | 16 |
| S–A–B–H–J–T | 3 | 19 |
| S–A–G–H–J–T | 3 | 22 |
| S–F–G–H–J–T | 2 | 24 |
| S–F–E–K–C–T | 5 | 29 |
| S–F–E–K–J–T | 1 | 30 |

Each amount is the current path bottleneck. The resulting nonzero arc flows are

$$
\begin{gathered}
SA=12,\ SF=8,\ SD=10,\ AB=9,\ AG=3,\ FG=2,\ FE=6,\ DC=10,\\
EK=6,\ GH=5,\ BH=3,\ BT=6,\ HJ=8,\ KJ=1,\ KC=5,\ JT=9,\ CT=15;
\end{gathered}
$$

every other arc has zero flow. Directly summing incoming and outgoing flows verifies conservation, and every displayed flow is at most its printed capacity. A minimum-cut certificate is

$$
U=\{S,A,B,E,F,G,H\},\qquad U^c=\{D,K,J,C,T\}.
$$

Its only outgoing arcs are $SD$, $EK$, $HJ$ and $BT$, with capacities $10,6,8,6$. Therefore

$$
\boxed{\text{maximum flow}=10+6+8+6=30.}
$$

The matching feasible flow and cut prove optimality independently of the augmenting-path choices.

## ↑ Ancestors (10)

1. [20D](../20d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
