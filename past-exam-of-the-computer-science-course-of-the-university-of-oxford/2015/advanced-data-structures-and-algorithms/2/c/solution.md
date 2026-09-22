<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For any feasible [circulation with vertex demands](../../../../../circulation-with-vertex-demands.md), sum its defining [flow balance](../../../../../flow-balance.md) over all [vertices](../../../../../vertex-graph-theory.md):

$$
\sum_{v\in V}d_v
=\sum_{v\in V}\sum_{u:uv\in E}f_{uv}
-\sum_{v\in V}\sum_{w:vw\in E}f_{vw}.
$$

Every directed [edge](../../../../../edge-of-a-graph.md) $ab\in E$ contributes $+f_{ab}$ exactly once to the first sum, at its head $b$, and $-f_{ab}$ exactly once to the second, at its tail $a$. The two sums therefore contain exactly the same terms. They cancel, giving

$$
\boxed{\sum_{v\in V}d_v=0.}
$$

This is global [flow conservation](../../../../../flow-conservation.md): internal transport cannot create or destroy the total amount. [Lower bounds on network flow](../../../../../lower-bounds-on-network-flow.md) and [capacity constraints](../../../../../capacity-constraint.md) restrict which [flows](../../../../../flow.md) are feasible but do not affect the cancellation. The condition is necessary, not sufficient: insufficient [flow network edge capacities](../../../../../flow-network-edge-capacity.md) can still prevent satisfying balanced demands.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Advanced data structures and algorithms](../../../advanced-data-structures-and-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
