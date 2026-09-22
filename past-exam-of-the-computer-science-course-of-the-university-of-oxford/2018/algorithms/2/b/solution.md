<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Construct a [set cover problem](../../../../../set-cover-problem.md) instance whose universe is the [set](../../../../../set-split.md) of [edges](../../../../../edge-of-a-graph.md) $E$. For each [vertex](../../../../../vertex-graph-theory.md) $v\in V$, supply the [set](../../../../../set-split.md) $S_v$ of all [edges](../../../../../edge-of-a-graph.md) incident to $v$. A collection $\{S_v:v\in C\}$ covers the universe if and only if every [edge](../../../../../edge-of-a-graph.md) has an endpoint in $C$, which is precisely the [vertex cover](../../../../../vertex-cover.md) condition.

The correspondence preserves [cardinality](../../../../../cardinality.md): **a [vertex cover](../../../../../vertex-cover.md) of size $k$ is a feasible solution of the [set cover problem](../../../../../set-cover-problem.md) using $k$ of these sets, and conversely**. If two labelled [vertices](../../../../../vertex-graph-theory.md) produce identical [sets](../../../../../set-split.md), one can keep their labels or discard duplicate choices without changing the optimum. The construction has size $O(|V|+|E|)$ when incidences are listed, so it is a [polynomial-time reduction](../../../../../polynomial-time-reduction.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
