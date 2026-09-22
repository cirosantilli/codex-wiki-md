<h1 id="6/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [Louvain method](../../../../../louvain-method.md) approximately maximizes [network modularity](../../../../../network-modularity.md). Start with each [vertex](../../../../../vertex-graph-theory.md) in its own community. Repeatedly visit each [vertex](../../../../../vertex-graph-theory.md), evaluate moving it into each neighbouring community, and accept the move with the greatest positive modularity gain. When no such local move improves the score, contract each community into a new weighted [vertex](../../../../../vertex-graph-theory.md), summing inter-community edge weights and retaining internal edges as [self-loops](../../../../../loop-graph-theory.md). Repeat local optimization and contraction until no further gain is obtained, then map the communities back to the original [vertices](../../../../../vertex-graph-theory.md).[§2, Method, pp. 4–5 of the preprint: local moves followed by aggregation](../../../../../fast-unfolding-of-communities-in-large-networks-by-vincent-d-blondel-and-others.md)

For an undirected unweighted [graph](../../../../../graph-split.md) with $m$ edges, [degrees of vertices](../../../../../degree-graph-theory.md) $k_i$ and community labels $c_i$, the objective is

$$
Q=\frac1{2m}\sum_{i,j}\left(A_{ij}-\frac{k_ik_j}{2m}\right)\mathbf1\{c_i=c_j\}.
$$

The term $k_ik_j/(2m)$ subtracts the expected connectivity in a degree-based [network null model](../../../../../network-null-model.md). If all [vertices](../../../../../vertex-graph-theory.md) are put in one community, the observed and expected total weights cancel, so $Q=0$. A partition with excess internal connectivity can have $Q>0$, and merging away that structure reduces the score. **The modularity objective and positive-gain rule prevent arbitrary merging merely to increase cluster size.** They do not forbid a single community in every possible network: if there is no better modular partition, one community may be an appropriate result. The method is a greedy heuristic, so it does not guarantee the global maximum of $Q$.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
