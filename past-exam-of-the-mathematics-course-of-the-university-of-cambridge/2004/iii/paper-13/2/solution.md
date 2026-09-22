<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For disjoint [vertex sets](../../../../../vertex-set.md) $A,B$, define their [edge density of a bipartite graph](../../../../../edge-density-of-a-bipartite-graph.md) by $d(A,B)=e(A,B)/(|A||B|)$. They form a [regular pair](../../../../../regular-pair-of-vertex-sets.md) with parameter $\varepsilon$ if every $A'\subseteq A,B'\subseteq B$ with $|A'|\geq\varepsilon|A|$, $|B'|\geq\varepsilon|B|$ satisfies $|d(A',B')-d(A,B)|\leq\varepsilon$.

The [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md) says that for every $\varepsilon>0$ and minimum cell count $k_0$, some $K,n_0$ have the following property. Every [graph](../../../../../graph-split.md) on $n\geq n_0$ [vertices](../../../../../vertex-graph-theory.md) admits

$$
V=V_0\sqcup V_1\sqcup\cdots\sqcup V_k,
\qquad k_0\leq k\leq K,
$$

with $|V_0|\leq\varepsilon n$, equal-sized $V_1,\ldots,V_k$, and at most $\varepsilon k^2$ unordered [irregular pairs](../../../../../irregular-pair-of-vertex-sets.md). It is enough to consider $0<\varepsilon<1/2$.

Prove this using [equitable regularity energy](../../../../../equitable-regularity-energy.md). Treat exceptional [vertices](../../../../../vertex-graph-theory.md) as singleton cells and set

$$
q(\mathcal P)=\frac1{n^2}\sum_{A,B\in\mathcal P}|A||B|d(A,B)^2,
$$

with ordered pairs and the adjacency indicator also defining diagonal densities. Then $0\leq q\leq1$. The [refinement variance identity for regularity energy](../../../../../refinement-variance-identity-for-regularity-energy.md) proves refinement cannot decrease $q$:

$$
\sum_{a,b}|A_a||B_b|d(A_a,B_b)^2-|A||B|d(A,B)^2
=\sum_{a,b}|A_a||B_b|(d(A_a,B_b)-d(A,B))^2.
$$

An [irregular pair](../../../../../irregular-pair-of-vertex-sets.md) supplies witness subsets of relative sizes at least $\varepsilon$ whose density differs by more than $\varepsilon$. Refining along those witnesses raises $q$ by more than $\varepsilon^4L^2/n^2$ per orientation, where $L$ is the common cell size. If there are more than $\varepsilon k^2$ [irregular pairs](../../../../../irregular-pair-of-vertex-sets.md), the increase is greater than $\varepsilon^5(kL/n)^2\geq\varepsilon^5/4$, provided the exceptional set has size at most $n/2$.

Refine each cell by all its witness subsets; this produces at most $2^k$ atoms per cell. Restore equal sizes by the [equalization with a controlled exceptional set](../../../../../equalization-with-a-controlled-exceptional-set.md): cut each atom into blocks of size $\lfloor L/4^k\rfloor$ and declare its remainder exceptional, still retaining every such [vertex](../../../../../vertex-graph-theory.md) as a singleton in the energy. This is another refinement, so no energy is lost. At most $k2^k\lfloor L/4^k\rfloor\leq n2^{-k}$ [vertices](../../../../../vertex-graph-theory.md) become exceptional, and, when $L\geq2\cdot4^k$, at most $2k4^k$ new nonexceptional cells occur.

Put $T=\lceil4\varepsilon^{-5}\rceil$ and start with $k\geq k_0$ so large that $T2^{-k}\leq\varepsilon/2$. An initial equitable partition has at most $\varepsilon n/2$ exceptional [vertices](../../../../../vertex-graph-theory.md) when $n$ is sufficiently large. Subsequent cell counts only increase, so the total added exceptional set has size at most $\varepsilon n/2$. The recurrence $k\mapsto2k4^k$, iterated at most $T$ times, supplies a finite bound $K$; choose $n_0$ large enough that every intermediate $L$ meets the size requirement. More than $T$ unsuccessful refinements would raise $q$ above one. The process must therefore stop with the required [regular pairs](../../../../../regular-pair-of-vertex-sets.md). This proves the lemma.

Its usefulness comes from replacing an arbitrarily large [graph](../../../../../graph-split.md) by the bounded [reduced graph of a regularity partition](../../../../../reduced-graph-of-a-regularity-partition.md). For fixed positive cross-density, the [graph embedding lemma for regular pairs](../../../../../graph-embedding-lemma-for-regular-pairs.md) lifts fixed configurations from the reduced [graph](../../../../../graph-split.md) to the original one. In particular, three sufficiently regular positive-density pairs contain many [triangles in a graph](../../../../../triangle-in-a-graph.md). Deleting exceptional, intracell, irregular and sparse-pair [edges](../../../../../edge-of-a-graph.md) then gives the [triangle removal lemma](../../../../../triangle-removal-lemma.md): a [graph](../../../../../graph-split.md) with sufficiently few triangles can be made [triangle-free](../../../../../triangle-free-graph.md) by deleting $o(n^2)$ [edges](../../../../../edge-of-a-graph.md). A triangle surviving in the reduced [graph](../../../../../graph-split.md) would force a positive proportion of the original possible triangles, a contradiction. More generally this approach yields the [clique removal lemma](../../../../../clique-removal-lemma.md) and the asymptotic [Erdős-Stone theorem](../../../../../erdos-stone-theorem.md). Applied to the tripartite [graph](../../../../../graph-split.md) encoding $x+z=2y$, triangle removal also gives [Roth theorem](../../../../../roth-s-theorem.md) on three-term [arithmetic progressions](../../../../../arithmetic-progression.md). The price is that the energy argument gives a very rapidly growing, iterated-exponential bound on $K(\varepsilon)$; the lemma is a structural tool, not a promise of small practical constants.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
