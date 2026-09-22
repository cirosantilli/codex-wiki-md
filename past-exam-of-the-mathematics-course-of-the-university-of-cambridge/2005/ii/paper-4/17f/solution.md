<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

[Extremal graph theory](../../../../../extremal-graph-theory.md) asks how many edges a graph can have while avoiding a prescribed subgraph. Define $\operatorname{ex}(n,H)$ as the maximum number of edges of an $n$-vertex simple graph containing no copy of $H$; copies need not be induced. The extremal graph often reveals the structural reason a forbidden configuration must appear.

A complete proof of [Mantel theorem](../../../../../mantel-theorem.md) illustrates this principle. In a triangle-free graph, the neighborhoods of the endpoints of any edge are disjoint, so $d(u)+d(v)\le n$. Summing over edges gives $\sum_vd(v)^2\le nm$, where $m$ is the edge count. By [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md),

$$
(2m)^2=\left(\sum_vd(v)\right)^2\le n\sum_vd(v)^2\le n^2m.
$$

Thus $m\le n^2/4$ when $m>0$, and the zero-edge case is immediate. A balanced [complete bipartite graph](../../../../../complete-bipartite-graph.md) is triangle-free and has $\lfloor n^2/4\rfloor$ edges. Therefore

$$
\boxed{\operatorname{ex}(n,K_3)=\lfloor n^2/4\rfloor}.
$$

The proof links a local forbidden triangle to a global degree inequality.

The general [Turan theorem](../../../../../turan-s-theorem.md) states that the balanced complete $(r-1)$-partite graph $T_{r-1}(n)$ maximizes the edge count among $K_r$-free graphs. Its leading density is $(1-1/(r-1))n^2/2$. A standard symmetrization explanation is to replace a lower-degree vertex by a twin of a nonadjacent higher-degree vertex: no $K_r$ is created and the edge count does not decrease. Iterating at the level of twin classes produces a [complete multipartite graph](../../../../../complete-multipartite-graph.md) with at most $r-1$ parts. Moving vertices between parts then balances the part sizes and maximizes the number of cross edges. This provides structural intuition beyond the preceding exact triangle proof.

For any fixed graph $H$ with [chromatic number](../../../../../chromatic-number.md) $r\ge2$, the [Erdős-Stone theorem](../../../../../erdos-stone-theorem.md) is

$$
\boxed{\operatorname{ex}(n,H)
=\left(1-\frac1{r-1}+o(1)\right)\frac{n^2}{2}}.
$$

The lower bound is the Turan construction: an $(r-1)$-partite graph cannot contain $H$. To describe the upper-bound proof, fix an edge-density excess above $1-1/(r-1)$. Apply a regularity partition with an error parameter much smaller than that excess and a positive density threshold. Delete irregular and low-density pairs; the resulting reduced graph still has density above the Turan threshold, so it contains $K_r$. The corresponding $r$ vertex classes form pairwise regular, positive-density pairs. The embedding argument successively chooses vertices with large neighborhoods in every remaining class; regularity discards only a small exceptional set at each choice. With the parameters sufficiently small and $n$ sufficiently large, this embeds a complete $r$-partite graph with $|V(H)|$ vertices in each part, and therefore a properly colored copy of $H$. This explains why [chromatic number](../../../../../chromatic-number.md), rather than the exact shape of $H$, controls the leading quadratic term.

For example $\chi(C_5)=3$, so forbidding a five-cycle still allows asymptotically $n^2/4$ edges, and exceeding that density by any fixed positive fraction eventually forces a five-cycle. For $K_r$ the exact [Turan theorem](../../../../../turan-s-theorem.md) strengthens the asymptotic statement. For bipartite $H$, the theorem gives only $o(n^2)$, leaving an important finer problem: for example $K_{s,t}$-free graphs have upper bounds of order $n^{2-1/s}$ from counting common neighborhoods. Extremal results consequently range from exact finite bounds to asymptotic density thresholds and stability questions about near-extremal structure.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
