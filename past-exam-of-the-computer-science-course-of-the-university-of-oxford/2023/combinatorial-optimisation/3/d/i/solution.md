<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $G$ has no [isolated vertex](../../../../../../isolated-vertex.md); otherwise an [edge cover](../../../../../../edge-cover.md) does not exist. In particular, a one-[vertex](../../../../../../vertex-graph-theory.md) [connected graph](../../../../../../connected-graph.md) is an excluded degenerate case of the statement.

Let $M$ be a [maximum cardinality matching](../../../../../../maximum-cardinality-matching.md), of size $m(G)$, and let $U$ be its [unmatched vertices in a matching](../../../../../../unmatched-vertex-in-a-matching.md). There is no [edge](../../../../../../edge-of-a-graph.md) joining two [vertices](../../../../../../vertex-graph-theory.md) of $U$, since adding it would enlarge $M$. Choose one incident [edge](../../../../../../edge-of-a-graph.md) for each $u\in U$. These chosen [edges](../../../../../../edge-of-a-graph.md) are distinct and outside $M$, so together they form an [edge cover](../../../../../../edge-cover.md) of size

$$
m(G)+|U|=m(G)+|V|-2m(G)=|V|-m(G).
$$

Consequently $e(G)\leq|V|-m(G)$.

For the opposite bound, let $F$ be a minimum-[cardinality](../../../../../../cardinality.md) [edge cover](../../../../../../edge-cover.md). It is inclusion-minimal. Every selected [edge](../../../../../../edge-of-a-graph.md) has an endpoint of [vertex degree](../../../../../../degree-graph-theory.md) one in $(V,F)$: otherwise deleting that [edge](../../../../../../edge-of-a-graph.md) would leave both endpoints covered. Each [connected component of a graph](../../../../../../component-graph-theory.md) of $(V,F)$ is therefore a [star graph](../../../../../../star-graph-theory.md). To see this, a component can have at most one [vertex](../../../../../../vertex-graph-theory.md) of [vertex degree](../../../../../../degree-graph-theory.md) greater than one; a shortest [graph path](../../../../../../path-in-a-graph.md) between two such [vertices](../../../../../../vertex-graph-theory.md) would contain an [edge](../../../../../../edge-of-a-graph.md) whose endpoints both have [vertex degree](../../../../../../degree-graph-theory.md) greater than one. A component with no such [vertex](../../../../../../vertex-graph-theory.md) is a single [edge](../../../../../../edge-of-a-graph.md), also a [star graph](../../../../../../star-graph-theory.md).

If there are $t$ such [star graphs](../../../../../../star-graph-theory.md), each has one fewer [edge](../../../../../../edge-of-a-graph.md) than [vertices](../../../../../../vertex-graph-theory.md), so $|F|=|V|-t$. Select one [edge](../../../../../../edge-of-a-graph.md) from each component to get a [matching in a graph](../../../../../../matching-graph-theory-split.md) of size $t$. Hence $m(G)\geq t=|V|-e(G)$, proving the [edge cover and matching identity](../../../../../../edge-cover-and-matching-identity.md)

$$
\boxed{e(G)+m(G)=|V|.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Combinatorial optimisation](../../../../combinatorial-optimisation-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
