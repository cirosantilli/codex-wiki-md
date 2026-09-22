<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For a [connected graph](../../../../../connected-graph.md) with at least one [edge](../../../../../edge-of-a-graph.md), run [depth-first search](../../../../../depth-first-search.md) and output the [set](../../../../../set-split.md) $I$ of [internal vertices of a rooted tree](../../../../../internal-vertex-of-a-rooted-tree.md) in its discovery [tree](../../../../../tree-graph-theory-split.md) $T$. Part (d) proves that $I$ is a [vertex cover](../../../../../vertex-cover.md). It is also connected: every ancestor of an internal [vertex](../../../../../vertex-graph-theory.md) is internal, so the [graph path](../../../../../path-in-a-graph.md) in $T$ from that [vertex](../../../../../vertex-graph-theory.md) to the root stays inside $I$. The root is internal when $|V|\geq2$.

For the approximation guarantee, choose a maximum-size [proper matching in a rooted tree](../../../../../proper-matching-in-a-rooted-tree.md) $M$ of $T$, whose existence is supplied. It is used only in the analysis; the [algorithm](../../../../../algorithm-split.md) need not construct it. Since every matched [edge](../../../../../edge-of-a-graph.md) uses two distinct [vertices](../../../../../vertex-graph-theory.md),

$$
|V|=2|M|+|U(M)|.
$$

By part (e), $|L(T)|\geq|U(M)|$. Therefore

$$
\boxed{|I|=|V|-|L(T)|\leq|V|-|U(M)|=2|M|\leq2\,\mathrm{OPT}.}
$$

The final inequality holds because every [vertex cover](../../../../../vertex-cover.md) of $G$, connected or otherwise, must use at least one distinct endpoint for each of the disjoint [edges](../../../../../edge-of-a-graph.md) in $M\subseteq E(G)$. Thus this is a **2-[approximation algorithm](../../../../../approximation-algorithm.md) in $O(|V|+|E|)$ [time complexity](../../../../../time-complexity.md)**.

For completeness, a disconnected input needs a feasibility check: if two different [connected components of a graph](../../../../../component-graph-theory.md) contain [edges](../../../../../edge-of-a-graph.md), no connected [vertex cover](../../../../../vertex-cover.md) can meet both. If exactly one component contains [edges](../../../../../edge-of-a-graph.md), run the construction on that component and ignore isolated [vertices](../../../../../vertex-graph-theory.md). If there are no [edges](../../../../../edge-of-a-graph.md), the empty [vertex cover](../../../../../vertex-cover.md) is optimal when an empty solution is permitted; if a nonempty connected solution is required, any single [vertex](../../../../../vertex-graph-theory.md) is optimal for a nonempty input. These conventions cover the boundary cases omitted from the main approximation argument.

## ↑ Ancestors (11)

1. [F](../f.md)
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
