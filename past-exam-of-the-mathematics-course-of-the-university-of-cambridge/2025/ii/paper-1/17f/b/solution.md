<h1 id="17f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [edge connectivity](../../../../../../edge-connectivity.md) $\lambda(G)$ is the minimum number of edges whose deletion disconnects $G$. Deleting all edges incident with a minimum-degree vertex proves $\lambda(G)\leq\delta(G)$. For a minimum edge cut separating vertex sets $A,B$, its endpoints on either suitable side give a vertex separator of size at most the number of cut edges; the complete-graph convention gives the same conclusion. Hence

$$
\delta(G)\geq\lambda(G)\geq\kappa(G).
$$

To realize prescribed $d\geq\ell\geq k\geq1$, take two disjoint copies $A,B$ of $K_{d+1}$. Add a bipartite set of exactly $\ell$ cross edges whose maximum matching has size $k$: include $a_ib_i$ for $1\leq i\leq k$, and, when $\ell>k$, add $a_1b_j$ for $k<j\leq\ell$. This is simple because $\ell\leq d$, has a matching of size $k$, and all its edges are covered by $\{a_1,\ldots,a_k\}$.

Vertices untouched by cross edges have degree $d$, so $\delta(G)=d$. The cross edges form an edge cut of size $\ell$; every cut that splits either clique uses at least $d\geq\ell$ clique edges, hence $\lambda(G)=\ell$. By König's theorem, the cross graph has a vertex cover of size $k$, whose deletion separates the two surviving clique pieces. Deleting fewer than $k$ vertices leaves each clique connected and at least one cross edge, so $\kappa(G)=k$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17F](../../17f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
