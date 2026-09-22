<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Suppose a [Directed acyclic graph](../../../../../directed-acyclic-graph.md) has a [Hamiltonian path](../../../../../hamiltonian-path.md) $(w_1,\ldots,w_n)$. Every edge $(w_j,w_{j+1})$ forces $w_j$ to precede $w_{j+1}$ in every [topological sort](../../../../../topological-sorting.md). Transitivity forces the entire order $(w_1,\ldots,w_n)$, so the [topological sort](../../../../../topological-sorting.md) is unique and every consecutive pair is joined by the requisite edge. No edge can point backwards in this path order, since that edge together with part of the path would form a [directed cycle](../../../../../directed-cycle.md).

Conversely, if a [topological sort](../../../../../topological-sorting.md) $(w_1,\ldots,w_n)$ has an edge from every entry to the next, those edges form a [graph path](../../../../../path-in-a-graph.md) through all [vertices](../../../../../vertex-graph-theory.md) exactly once. Thus **the displayed order is itself a [Hamiltonian path](../../../../../hamiltonian-path.md)**.

The [unique topological ordering criterion](../../../../../unique-topological-ordering-criterion.md) says that uniqueness alone already forces the consecutive-edge condition. If $(w_j,w_{j+1})$ were absent, swapping these adjacent entries would preserve every edge constraint: only their mutual order changes, and a reverse edge is already forbidden by the original [topological sort](../../../../../topological-sorting.md). This would produce a second order. Consequently, for a [Directed acyclic graph](../../../../../directed-acyclic-graph.md), **having a [Hamiltonian path](../../../../../hamiltonian-path.md), having a unique [topological sort](../../../../../topological-sorting.md), and having consecutive edges in a [topological sort](../../../../../topological-sorting.md) are equivalent**. The source's $>$ notation is read as “appears earlier”, consistent with its explicitly directed edges.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
