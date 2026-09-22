<h1 id="17g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For nonadjacent vertices $a,b$, the [local connectivity](../../../../../../local-connectivity.md) $\kappa(a,b;G)$ is the minimum cardinality of an $a$-$b$ [vertex separator](../../../../../../vertex-separator.md): a set $S\subseteq V(G)\setminus\{a,b\}$ such that $a$ and $b$ lie in different components of $G-S$.

To prove the vertex form of the [Menger theorem](../../../../../../menger-theorem.md), replace every vertex $v\notin\{a,b\}$ by an arc $v_{\mathrm{in}}\to v_{\mathrm{out}}$ of capacity one. Replace every undirected edge $uv$ by directed arcs from $u_{\mathrm{out}}$ to $v_{\mathrm{in}}$ and conversely, each of capacity larger than $|V(G)|$; leave $a,b$ unsplit. An integral $a$-$b$ flow of value $k$ decomposes into $k$ paths, and the unit-capacity vertex arcs force the corresponding graph paths to be [internally vertex-disjoint paths](../../../../../../internally-vertex-disjoint-paths.md). Conversely, $k$ such paths give an integral flow of value $k$.

Because $a$ and $b$ are nonadjacent, any finite minimum cut consists entirely of unit-capacity vertex arcs. These arcs correspond exactly to an $a$-$b$ vertex separator of the same size. The [max-flow min-cut theorem](../../../../../../max-flow-min-cut-theorem.md), whose augmenting-path proof also guarantees an integral maximum flow for integral capacities, therefore gives

$$
\max\{\text{number of internally vertex-disjoint $a$-$b$ paths}\}
=\kappa(a,b;G).
$$

In particular, $G$ contains the required set of $\kappa(a,b;G)$ paths.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [17G](../../17g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
