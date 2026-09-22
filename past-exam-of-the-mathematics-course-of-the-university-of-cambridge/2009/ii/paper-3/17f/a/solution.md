<h1 id="17f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Brooks' theorem](../../../../../../brooks-theorem.md) states that a finite connected simple [graph](../../../../../../graph-split.md) with maximum [vertex degree](../../../../../../degree-graph-theory.md) $\Delta$ has [chromatic number](../../../../../../chromatic-number.md) at most $\Delta$, unless it is a [complete graph](../../../../../../complete-graph.md) or an odd [cycle graph](../../../../../../cycle-graph.md); those exceptions have chromatic number $\Delta+1$.

First, if the graph is not regular, choose a vertex $v$ of degree less than $\Delta$ and a [spanning tree](../../../../../../spanning-tree.md) rooted at $v$. Order vertices with every child before its parent, and apply the [greedy coloring](../../../../../../greedy-coloring.md) algorithm. Every vertex except $v$ has an as-yet uncolored parent, so has at most $\Delta-1$ colored neighbors; $v$ also has fewer than $\Delta$ neighbors. Thus $\Delta$ colors suffice. This justifies reducing to the regular case.

Now let $G$ be regular, 3-connected and not complete. A shortest path between two nonadjacent vertices contains an induced two-edge path $a,v,b$ with $a,b$ nonadjacent. By 3-connectivity, $G-\{a,b\}$ is connected. Color $a,b$ with the same color. Choose a [spanning tree](../../../../../../spanning-tree.md) of the remaining graph rooted at $v$ and color its vertices in child-before-parent order. Each vertex other than $v$ again has an uncolored parent and thus at most $\Delta-1$ already colored neighbors. At the last vertex $v$, the two neighbors $a,b$ share a color, so its $\Delta$ neighbors use at most $\Delta-1$ distinct colors. A color is therefore available at every step, proving $\boxed{\chi(G)\le\Delta}$ in the required 3-connected noncomplete case. A 3-connected graph has $\Delta\ge3$, so the odd-cycle exception cannot arise here.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17F](../../17f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
