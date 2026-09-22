<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Reduce the [Hamiltonian cycle](../../../../../../hamilton-cycle.md) decision problem to the [metric travelling salesman problem](../../../../../../metric-travelling-salesman-problem.md). Given a simple graph on $n\geq3$ vertices, form the complete graph with distance $1$ on original edges and distance $2$ on nonedges. These symmetric distances satisfy the [triangle inequality](../../../../../../triangle-inequality.md), since a direct distance is at most $2$ and any two positive edge distances sum to at least $2$.

A tour has $n$ edges, each of cost at least $1$. It has cost at most $n$ exactly when every edge is an original graph edge, that is, exactly when the original graph has a [Hamiltonian cycle](../../../../../../hamilton-cycle.md). The construction and threshold are polynomial in the input size. Thus **the [metric travelling salesman problem](../../../../../../metric-travelling-salesman-problem.md) is [NP-hard](../../../../../../np-hardness.md)**; its rational-cost threshold version is also in [NP](../../../../../../np-complexity.md) because a tour is a polynomial-size certificate.

Allowing repeated vertex visits does not reduce the optimum for a complete metric instance. Given a closed walk visiting every vertex, keep the vertices in order of first appearance and shortcut the portions between them, including the final return. The [triangle inequality](../../../../../../triangle-inequality.md) makes the resulting Hamiltonian tour no more expensive. Conversely a Hamiltonian tour is an allowed closed walk. Hence the two optimal costs are equal, and **the repeated-visit metric version remains [NP-hard](../../../../../../np-hardness.md)**. If travel is described on a sparse graph, taking its shortest-path metric gives the corresponding closed-walk formulation rather than an easier exact problem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
