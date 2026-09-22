<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For disjoint nonempty vertex sets $U,W$, define their [edge density of a bipartite graph](../../../../../../edge-density-of-a-bipartite-graph.md) by $d(U,W)=e(U,W)/(|U||W|)$. They form an $\varepsilon$-[regular pair of vertex sets](../../../../../../regular-pair-of-vertex-sets.md) if every $X\subseteq U$, $Y\subseteq W$ with $|X|\ge\varepsilon|U|$, $|Y|\ge\varepsilon|W|$ satisfies $|d(X,Y)-d(U,W)|\le\varepsilon$.

The [Szemerédi regularity lemma](../../../../../../szemeredi-regularity-lemma.md) asserts that, given $\varepsilon>0$ and a positive integer $m_0$, there are $M,n_0$ such that every [graph](../../../../../../graph-split.md) on $n\ge n_0$ vertices has a [set partition](../../../../../../set-partition.md) $V_0,V_1,\ldots,V_k$ with

$$
m_0\le k\le M,\qquad |V_0|\le\varepsilon n,\qquad |V_1|=\cdots=|V_k|,
$$

and at most $\varepsilon k^2$ irregular ordered pairs $(V_i,V_j)$ with $1\le i\ne j\le k$.

Assume $0<\varepsilon\le1/2$, which suffices since a smaller regularity parameter gives the claim for a larger one. Treat the exceptional vertices as singleton cells in the full partition $\mathcal P$, and use [equitable regularity energy](../../../../../../equitable-regularity-energy.md)

$$
q(\mathcal P)=\frac1{n^2}\sum_{A,B\in\mathcal P}|A||B|d(A,B)^2.
$$

Here the adjacency [indicator function](../../../../../../indicator-function.md) defines density even for diagonal cells. Clearly $0\le q\le1$. If $\mathcal P'$ refines $\mathcal P$, weighted averaging of densities gives the [refinement variance identity for regularity energy](../../../../../../refinement-variance-identity-for-regularity-energy.md)

$$
q(\mathcal P')-q(\mathcal P)
=\frac1{n^2}\sum_{A,B\in\mathcal P}\sum_{\substack{A'\subseteq A\\B'\subseteq B}}|A'||B'|\bigl(d(A',B')-d(A,B)\bigr)^2\ge0.
$$

To verify it, expand each square and use $\sum_{A',B'}|A'||B'|d(A',B')=|A||B|d(A,B)$.

For every irregular ordered pair of nonexceptional cells, choose witnesses $X_{ij},Y_{ij}$ of relative sizes at least $\varepsilon$ and density discrepancy greater than $\varepsilon$. Split each $V_i$ along all witnesses involving it; symmetry allows at most one witness for each other cell, hence at most $2^k$ atoms in each $V_i$. In the witness rectangle, the weighted [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) in the variance identity contributes more than $\varepsilon^4|V_i||V_j|/n^2$.

If more than $\varepsilon k^2$ pairs are irregular and the equal cell size is $L$, the energy increase is greater than

$$
\varepsilon^5\frac{k^2L^2}{n^2}
=\varepsilon^5\left(1-\frac{|V_0|}{n}\right)^2
\ge\frac{\varepsilon^5}{4}.
$$

Restore equal cell sizes by cutting each witness atom into pieces of size $\ell=\lfloor L/4^k\rfloor$, with leftover vertices added to $V_0$ as singleton cells. This operation is a further refinement, so the energy does not decrease. There are at most $k2^k$ atoms, and fewer than $\ell$ leftover vertices in each, giving at most $k2^k\ell\le n2^{-k}$ new exceptional vertices.

Here is a uniform bound ensuring that the iteration is legitimate. Put $R=\lceil4\varepsilon^{-5}\rceil$ and choose

$$
k_0\ge\max\left\{m_0,\left\lceil\log_2(2R/\varepsilon)\right\rceil,2\right\}.
$$

Start with $k_0$ equal classes and fewer than $k_0$ exceptional vertices. Taking $n\ge2k_0/\varepsilon$ makes the initial exception at most $\varepsilon n/2$. At every refinement the number of nonexceptional cells does not decrease: each old cell loses at most $L2^{-k}\le L/2$ vertices and is cut into pieces of size at most $L/4^k$. Thus each of the at most $R$ rounds adds at most $\varepsilon n/(2R)$ exceptional vertices.

When $L\ge2\cdot4^k$, the new cell count is at most

$$
\frac n\ell\le\frac{2n4^k}{L}\le4k4^k,
$$

using $|V_0|\le\varepsilon n\le n/2$. Define $K_0=k_0$ and $K_{j+1}=4K_j4^{K_j}$, and take $M=K_R$. Choosing $n_0\ge\max\{2k_0/\varepsilon,\,4M4^M\}$ ensures $L\ge n/(2M)\ge2\cdot4^M$ at every stage. All rounds are therefore defined, with cell count between $m_0$ and $M$ and exceptional size at most $\varepsilon n$.

If the lemma still failed after $R$ refinements, the energy would have increased by more than $R\varepsilon^5/4\ge1$, impossible because it lies in $[0,1]$. Hence some stage has the required regular pairs. This completes the [energy-increment proof of Szemerédi regularity](../../../../../../energy-increment-proof-of-szemeredi-regularity.md), including the equal-size and exceptional-set conditions.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
