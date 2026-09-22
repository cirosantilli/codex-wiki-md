<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We prove a weighted version of the [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md), which is sufficient for the grid application. For disjoint nonempty vertex sets $U,W$ in a [graph](../../../../../graph-split.md), write $d(U,W)=e(U,W)/(|U||W|)$ for their [edge density of a bipartite graph](../../../../../edge-density-of-a-bipartite-graph.md). Call the pair $\varepsilon$-regular if every $U'\subseteq U$, $W'\subseteq W$ with $|U'|\geq\varepsilon|U|$ and $|W'|\geq\varepsilon|W|$ satisfies $|d(U',W')-d(U,W)|\leq\varepsilon$.

The [weighted Szemerédi regularity lemma](../../../../../weighted-szemeredi-regularity-lemma.md) states that, for every $0<\varepsilon<1$, there are integers $M,v_0$ such that every [graph](../../../../../graph-split.md) on $v\geq v_0$ vertices has a [set partition](../../../../../set-partition.md) into at most $M$ nonempty cells $V_1,\ldots,V_k$, each of size at most $\varepsilon v$, for which

$$
\sum_{\substack{i\ne j\\(V_i,V_j)\text{ not }\varepsilon\text{-regular}}}|V_i||V_j|\leq\varepsilon v^2.
$$

The sum is ordered. The cells need not have equal sizes; their weights replace the usual unweighted count of bad pairs.

To prove it, start with $k_0=\lceil2/\varepsilon\rceil$ nearly equal cells, taking $v\geq k_0$. Each has size at most $v/k_0+1\leq\varepsilon v$. Define the [regularity energy](../../../../../equitable-regularity-energy.md)

$$
q(\mathcal P)=\frac1{v^2}\sum_{U,W\in\mathcal P}|U||W|d(U,W)^2.
$$

Here even diagonal rectangles use the mean adjacency indicator, counting ordered pairs of vertices. Thus $0\leq q\leq1$. Under a refinement, the old rectangle density is the weighted mean of the new ones, and the [refinement variance identity for regularity energy](../../../../../refinement-variance-identity-for-regularity-energy.md) gives

$$
\sum_{a,b}|U_a||W_b|d(U_a,W_b)^2-|U||W|d(U,W)^2=\sum_{a,b}|U_a||W_b|(d(U_a,W_b)-d(U,W))^2.
$$

In particular refinement cannot decrease energy.

If the irregular-pair weight exceeds $\varepsilon v^2$, choose witness subsets $U'\subseteq U$, $W'\subseteq W$ for every irregular unordered pair, and split each cell simultaneously by all its witnesses. There are at most $k-1$ such subsets in any one cell, so the new number of cells is at most $k2^k$. In an irregular rectangle, its witness has relative area at least $\varepsilon^2$ and density discrepancy greater than $\varepsilon$. Since the witness rectangle is now a union of refined rectangles, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) applied to their weighted density discrepancies bounds the variance contribution from below by

$$
|U'||W'|\,|d(U',W')-d(U,W)|^2>\varepsilon^4|U||W|.
$$

Summing over both orientations of all irregular pairs raises $q$ by more than $\varepsilon^5$. Since $q\leq1$, after at most $\lceil\varepsilon^{-5}\rceil$ rounds the required weight bound must hold. The finite recurrence $k\mapsto k2^k$, starting at $k_0$, supplies $M(\varepsilon)$; all cells remain small because we only refine. This proves the stated [weighted Szemerédi regularity lemma](../../../../../weighted-szemeredi-regularity-lemma.md).

We next derive the [triangle removal lemma](../../../../../triangle-removal-lemma.md) from this version. First, three disjoint classes $U,W,Z$ whose pairs are $\varepsilon$-[regular pairs](../../../../../regular-pair-of-vertex-sets.md) of density at least $d$ have many triangles if $\varepsilon\leq d/2$ and $\varepsilon\leq1/4$. Fewer than $\varepsilon|U|$ vertices of $U$ have fewer than $(d-\varepsilon)|W|$ neighbours in $W$: otherwise that set of vertices, paired with all of $W$, would violate regularity. The same holds for $Z$. For each of the at least $(1-2\varepsilon)|U|$ remaining vertices, both neighbour sets have relative size at least $d-\varepsilon\geq\varepsilon$. Regularity of $(W,Z)$ then supplies at least $(d-\varepsilon)$ times the product of those two neighbour-set sizes edges. Thus the [regular triangle counting lemma](../../../../../regular-triangle-counting-lemma.md), also for unequal class sizes, gives

$$
\#\text{triangles across }U,W,Z\geq(1-2\varepsilon)(d-\varepsilon)^3|U||W||Z|\geq\frac{d^3}{16}|U||W||Z|.
$$

For a desired deletion tolerance $0<\eta<1$, take $\varepsilon=\eta/100$, $d=\eta/4$, and a weighted regularity partition with at most $M=M(\varepsilon)$ cells. Put $\tau=\varepsilon/M$. Delete edges inside cells, between irregular pairs, between regular pairs of density less than $d$, and incident to cells smaller than $\tau v$. The first two deletions each cost at most $\varepsilon v^2/2$. The sparse-pair deletion costs at most $dv^2/2$. For the last deletion, [small-cell deletion in weighted regularity](../../../../../small-cell-deletion-in-weighted-regularity.md) removes at most $M\tau v=\varepsilon v$ vertices and at most $\varepsilon v^2$ incident edges. The total is bounded by

$$
(2\varepsilon+d/2)v^2<\eta v^2.
$$

A triangle surviving these deletions would lie in three distinct cells, all of size at least $\tau v$, with all their pairs regular and of density at least $d$. The original graph would then have at least $d^3\tau^3v^3/16$ triangles. Therefore, with

$$
\kappa=\frac{d^3\tau^3}{32}>0,
$$

a graph on sufficiently many vertices with at most $\kappa v^3$ triangles can be made [triangle-free](../../../../../triangle-free-graph.md) by deleting fewer than $\eta v^2$ edges. This establishes the [triangle removal lemma](../../../../../triangle-removal-lemma.md) with every parameter depending only on $\eta$.

Now apply a [tripartite graph encoding of a grid](../../../../../tripartite-graph-encoding-of-a-grid.md). Take separate vertex classes $X=[N]$, $Y=[N]$, $Z=\{2,\ldots,2N\}$. For each grid point $(x,y)$ in the given set, put in the three edges

$$
xy,\qquad x(x+y),\qquad y(x+y),
$$

where their endpoints belong respectively to $X\!\times\!Y$, $X\!\times\!Z$, and $Y\!\times\!Z$. Each point supplies a triangle. These $|A|$ triangles are [edge-disjoint triangles](../../../../../edge-disjoint-triangles.md), since any one of the three edge types uniquely determines the point that supplied it.

Conversely, any triangle with vertices $x\in X$, $y\in Y$, $z\in Z$ forces the three points

$$
(x,y),\qquad(x,z-x),\qquad(z-y,y)
$$

to belong to $A$. Put $d=z-x-y$. For $d\ne0$ these form a [corner in an integer grid](../../../../../corner-in-an-integer-grid.md); for $d=0$ they all arise from the same grid point. Thus if there is no corner, the graph has exactly $|A|\leq N^2$ triangles, yet destroying all triangles requires at least $|A|\geq\delta N^2$ edge deletions.

We may suppose $0<\delta\leq1$, since larger densities make the request vacuous. Use the [triangle removal lemma](../../../../../triangle-removal-lemma.md) with $\eta=\delta/32$. Our graph has $v=4N-1$ vertices, so, for sufficiently large $N$, its bound $N^2$ on the number of triangles is at most $\kappa v^3$. The lemma would delete fewer than

$$
\eta v^2<\frac\delta{32}(4N)^2=\frac\delta2N^2
$$

edges to destroy all triangles. This contradicts the lower bound $\delta N^2$ from the edge-disjoint family. Hence **every sufficiently large positive-density square grid contains a nondegenerate corner**, proving the requested [corners theorem](../../../../../corners-theorem.md) and in particular the existence of a suitable $N$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
