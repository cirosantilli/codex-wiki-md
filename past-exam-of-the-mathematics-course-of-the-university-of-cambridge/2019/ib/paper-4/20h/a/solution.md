<h1 id="20h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [max-flow min-cut theorem](../../../../../../max-flow-min-cut-theorem.md) states that in a finite [flow network](../../../../../../flow-network.md), the maximum value of a feasible source-to-sink flow equals the minimum capacity of a source-to-sink [cut](../../../../../../cut-of-a-flow-network.md).

First consider any feasible flow $f$ and any cut $(A,V\setminus A)$ with $S\in A$ and $T\notin A$. Summing [flow conservation](../../../../../../flow-conservation.md) over the vertices in $A$ cancels all contributions from edges internal to $A$ and gives

$$
|f|
=\sum_{u\in A,v\notin A}f(u,v)
-\sum_{u\notin A,v\in A}f(u,v)
\leq\sum_{u\in A,v\notin A}c(u,v)
=c(A,V\setminus A).
$$

Thus every flow value is at most every cut capacity.

A maximum flow exists because the feasible flows form a nonempty compact subset of a finite-dimensional Euclidean space and the flow value is continuous. Let $f$ be maximum and form its [residual network](../../../../../../residual-network.md). If there were an [augmenting path](../../../../../../augmenting-path.md) from $S$ to $T$, increasing $f$ by the path's positive bottleneck capacity would contradict maximality. Let $A$ be the set of vertices reachable from $S$ in the residual network. Then $T\notin A$. Every original edge from $A$ to its complement is saturated, while every original edge entering $A$ carries zero flow; otherwise the corresponding forward or reverse residual edge would make its other endpoint reachable. Consequently

$$
|f|
=\sum_{u\in A,v\notin A}c(u,v)
=c(A,V\setminus A).
$$

The general upper bound is attained by this flow and cut, proving the theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20H](../../20h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
