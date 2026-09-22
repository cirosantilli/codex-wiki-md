<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $Z$ be the [set](../../../../../set-split.md) of [isolated vertices](../../../../../isolated-vertex.md) of the finite [simple graph](../../../../../simple-graph.md) $G=(V,E)$. Introduce a nonnegative [integer](../../../../../integer-split.md) $x_v$ for every [vertex](../../../../../vertex-graph-theory.md). Use the [integer program](../../../../../integer-programming.md)

$$
\boxed{\begin{aligned}
\text{maximize}\quad&\sum_{v\in V}x_v\\
\text{subject to}\quad&x_u+x_v\leq1&&\text{for every }\{u,v\}\in E,\\
&x_v\leq1&&\text{for every }v\in Z,\\
&x_v\geq0,\quad x_v\in\mathbb Z&&\text{for every }v\in V.
\end{aligned}}
$$

Every nonisolated [vertex](../../../../../vertex-graph-theory.md) belongs to an [edge](../../../../../edge-of-a-graph.md), whose inequality and the other endpoint's nonnegativity already imply $x_v\leq1$. The explicit bounds on $Z$ therefore make all variables binary. For an [integer](../../../../../integer-split.md) [feasible point](../../../../../feasible-point.md), $S=\{v:x_v=1\}$ is an [independent set](../../../../../independent-set-graph-theory.md), and its [cardinality](../../../../../cardinality.md) is the objective. Conversely the [indicator vector](../../../../../indicator-vector.md) of any [independent set](../../../../../independent-set-graph-theory.md) is feasible. Thus **the optimal value is the maximum [independent set](../../../../../independent-set-graph-theory.md) size**. Including the isolated-[vertex](../../../../../vertex-graph-theory.md) bounds is essential for an arbitrary [graph](../../../../../graph-split.md); without them the formulation would be unbounded whenever an [isolated vertex](../../../../../isolated-vertex.md) is present.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
