<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**No.** A counterexample works for every $k\geq2$. Take the [complete bipartite graph](../../../../../complete-bipartite-graph.md) $G=K_{k,k}$ with [vertex sets](../../../../../vertex-set.md)

$$
A=\{a_1,\ldots,a_k\},\qquad B=\{b_1,\ldots,b_k\}.
$$

It is a [k-connected graph](../../../../../k-connected-graph.md): deleting fewer than $k$ [vertices](../../../../../vertex-graph-theory.md) leaves at least one [vertex](../../../../../vertex-graph-theory.md) in each side, and the remaining [complete bipartite graph](../../../../../complete-bipartite-graph.md) is a [connected graph](../../../../../connected-graph.md).

Choose

$$
U=\{b_1,a_1,\ldots,a_{k-1}\},\qquad
W=\{b_2,\ldots,b_k,a_k\},
$$

and order these [sets](../../../../../set-split.md) so that $u_1=b_1$ and $w_1=b_2$. Order the other members arbitrarily. These are disjoint [sets](../../../../../set-split.md) of [cardinality](../../../../../cardinality.md) $k$, and every [vertex](../../../../../vertex-graph-theory.md) of $G$ is one of the specified endpoints.

If the prescribed $k$ [vertex-disjoint paths](../../../../../vertex-disjoint-paths.md) existed, no one of them could have an internal [vertex](../../../../../vertex-graph-theory.md), because every [vertex](../../../../../vertex-graph-theory.md) must serve as the endpoint of one of the [graph paths](../../../../../path-in-a-graph.md). Thus each [graph path](../../../../../path-in-a-graph.md) would have to be a single [edge](../../../../../edge-of-a-graph.md). But $b_1,b_2$ lie in the same side of the [bipartite graph](../../../../../bipartite-graph-split.md), so there is no [edge](../../../../../edge-of-a-graph.md) $b_1b_2$. This contradicts the requirement on $P_1$.

For $k=2$ this is the four-[vertex](../../../../../vertex-graph-theory.md) [cycle graph](../../../../../cycle-graph.md), with opposite [vertices](../../../../../vertex-graph-theory.md) paired. The stronger property that every prescribed pairing can be realized is the [linked graph](../../../../../linked-graph.md) property; [vertex connectivity](../../../../../vertex-connectivity.md) alone does not guarantee it.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the graph theory course of the University of Oxford](../../../../split.md)
6. [Graph theory course of the University of Oxford](../../../../../graph-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
