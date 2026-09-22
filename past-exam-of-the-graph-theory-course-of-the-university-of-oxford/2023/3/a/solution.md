<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [graph](../../../../graph-split.md) is a [k-connected graph](../../../../k-connected-graph.md) if it has at least $k+1$ [vertices](../../../../vertex-graph-theory.md) and deleting any [set](../../../../set-split.md) of fewer than $k$ [vertices](../../../../vertex-graph-theory.md), together with their incident [edges](../../../../edge-of-a-graph.md), leaves a [connected graph](../../../../connected-graph.md).

The [vertex connectivity](../../../../vertex-connectivity.md) $\kappa(G)$ is the largest such $k$. Equivalently, for a [graph](../../../../graph-split.md) with at least two [vertices](../../../../vertex-graph-theory.md), it is the smallest number of [vertices](../../../../vertex-graph-theory.md) whose deletion either disconnects the [graph](../../../../graph-split.md) or leaves a single [vertex](../../../../vertex-graph-theory.md). The latter convention gives $\kappa(K_n)=n-1$ for a [complete graph](../../../../complete-graph.md). A disconnected [graph](../../../../graph-split.md) has [vertex connectivity](../../../../vertex-connectivity.md) zero; one usually also sets $\kappa(K_1)=0$.

For distinct nonadjacent [vertices](../../../../vertex-graph-theory.md) $x,y$, the [local connectivity](../../../../local-connectivity.md) is

$$
\boxed{\kappa_G(x,y)=\min\{|S|:S\subseteq V(G)\setminus\{x,y\},\ \text{there is no }x\text{--}y\text{ path in }G-S\}.}
$$

Such a [set](../../../../set-split.md) $S$ is an $x$–$y$ [vertex separator](../../../../vertex-separator.md). By [Menger's theorem](../../../../menger-theorem.md), [local connectivity](../../../../local-connectivity.md) also equals the maximum number of [internally vertex-disjoint paths](../../../../internally-vertex-disjoint-paths.md) from $x$ to $y$. If no [graph path](../../../../path-in-a-graph.md) exists already, the empty [vertex separator](../../../../vertex-separator.md) gives zero.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the graph theory course of the University of Oxford](../../../split.md)
5. [Graph theory course of the University of Oxford](../../../../graph-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
