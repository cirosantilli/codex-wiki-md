<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

For a connected plane drawing, [Euler formula for a connected planar graph](../../../../../euler-formula-for-a-connected-planar-graph.md) is

$$
\boxed{v-e+f=2.}
$$

For a simple [planar graph](../../../../../planar-graph.md) with $v\ge3$, counting edge sides around faces gives $3f\le2e$ and hence $e\le3v-6$. Thus some vertex has degree at most five. A tree or a graph with bridges obeys the same bound; a face boundary is counted as a closed walk with edge multiplicity, and the small cases are immediate.

Induct on the number of vertices to prove the [five colour theorem](../../../../../five-color-theorem.md). Remove a vertex $v$ of degree at most five and five-colour the remainder. If fewer than five colors appear at its neighbours, extend the coloring. Otherwise it has five neighbours in their cyclic order, with colors $1,2,3,4,5$. If the color-1 neighbour is not connected to the color-3 neighbour by a path using only colors 1 and 3, swap these colors in the component containing the former, freeing color 1 at $v$. If they are connected, that path together with its two edges to $v$ is a simple closed curve. The colour-2 and colour-4 neighbours lie on opposite sides, so cannot be joined by a path using only colors 2 and 4, which would have to cross it. Swap colors in the component containing the colour-2 neighbour and give $v$ color 2. This establishes the induction without the [four colour theorem](../../../../../four-color-theorem.md).

For a triangle-free simple [planar graph](../../../../../planar-graph.md) with $v\ge3$, the analogous bound is $e\le2v-4$, so some vertex has degree at most three. One can prove the bound for connected graphs with no bridges by $4f\le2e$; bridges and isolated components are then joined or split off, with the small tree cases checked directly. Every subgraph is still triangle-free and planar. Successively remove a vertex of degree at most three, and color in reverse order with four colors. Thus **triangle-free planar graphs have [chromatic number](../../../../../chromatic-number.md) at most four**.

Finally, let $G$ be minimal 5-chromatic. Removing any vertex leaves a graph colorable with four colors. If its degree is at most three, that coloring extends immediately. If its degree is four, either a colour is unused at its neighbours, or all four appear once in cyclic order. The same two-path argument, now using opposite pairs 1,3 and 2,4, permits a [Kempe chain](../../../../../kempe-chain.md) interchange freeing one colour. Therefore a planar minimal 5-chromatic graph must satisfy

$$
\boxed{\delta(G)\ge5.}
$$

Without planarity only $\delta(G)\ge4$ follows from the elementary extension argument. The [complete graph](../../../../../complete-graph.md) $K_5$ is a counterexample to the stronger assertion: it is minimal 5-chromatic and every vertex has degree four. Deleting an edge allows its endpoints to share a color; deleting a vertex also reduces the required number of colors.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
