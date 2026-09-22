<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [proper edge colouring](../../../../proper-edge-coloring.md) assigns colours to the [edges](../../../../edge-of-a-graph.md) of a [graph](../../../../graph-split.md) so that distinct [edges](../../../../edge-of-a-graph.md) sharing a [vertex](../../../../vertex-graph-theory.md) have different colours. The [edge chromatic number](../../../../edge-chromatic-number.md) $\chi'(G)$ is the least number of colours in such an assignment. Equivalently, it is the least number of [matchings in a graph](../../../../matching-graph-theory-split.md) whose disjoint union is the entire collection of [edges](../../../../edge-of-a-graph.md).

[Vizing's theorem](../../../../vizing-s-theorem.md) states that a finite [simple graph](../../../../simple-graph.md) of [maximum degree](../../../../maximum-degree.md) $\Delta$ satisfies

$$
\boxed{\Delta\leq\chi'(G)\leq\Delta+1.}
$$

The lower bound holds because all [edges](../../../../edge-of-a-graph.md) incident with a [vertex](../../../../vertex-graph-theory.md) of [vertex degree](../../../../degree-graph-theory.md) $\Delta$ require different colours.

[Hall's marriage theorem](../../../../hall-s-marriage-theorem.md) states that a finite [bipartite graph](../../../../bipartite-graph-split.md) with [vertex sets](../../../../vertex-set.md) $A,B$ has a [matching in a graph](../../../../matching-graph-theory-split.md) saturating $A$ if and only if

$$
\boxed{|N(S)|\geq|S|\quad\text{for every }S\subseteq A,}
$$

where $N(S)\subseteq B$ is the [graph neighbourhood](../../../../graph-neighbourhood.md) of $S$. Here [matching saturation](../../../../matching-saturation.md) means that each [vertex](../../../../vertex-graph-theory.md) of $A$ is incident with an [edge](../../../../edge-of-a-graph.md) of the [matching in a graph](../../../../matching-graph-theory-split.md); it does not require every [vertex](../../../../vertex-graph-theory.md) of $B$ to be met.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
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
