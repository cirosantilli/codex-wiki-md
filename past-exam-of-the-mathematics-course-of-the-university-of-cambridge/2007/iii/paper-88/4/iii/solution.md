<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Yes. The same telescoping argument proves the [counting lemma for octahedrally quasirandom three-uniform hypergraphs](../../../../../../counting-lemma-for-octahedrally-quasirandom-three-uniform-hypergraphs.md) for every fixed simple three-uniform [hypergraph](../../../../../../hypergraph-split.md) $F$.

Label its [vertices of a hypergraph](../../../../../../vertex-of-a-hypergraph.md) $1,\ldots,v$ and give [vertex of a hypergraph](../../../../../../vertex-of-a-hypergraph.md) $i$ a nonempty host part $V_i$. For each [hypergraph edge](../../../../../../edge-of-a-hypergraph.md) $e=\{i,j,k\}$, let $h_e$ be the corresponding host [hypergraph edge](../../../../../../edge-of-a-hypergraph.md) [indicator function](../../../../../../indicator-function.md) of [subset density](../../../../../../density-of-a-finite-subset.md) $p_e$, with $\|h_e-p_e\|_{\square^3}\leq\alpha^{1/8}$. The normalized [labelled hypergraph copy count](../../../../../../labelled-hypergraph-copy-count.md) is

$$
t_F=\mathbb E_{x_1\in V_1,\ldots,x_v\in V_v}\prod_{e\in E(F)}h_e(x_e).
$$

If the host parts are disjoint, every such [vertex of a hypergraph](../../../../../../vertex-of-a-hypergraph.md) choice is automatically [injective](../../../../../../injective-function.md). Enumerate the $m$ [hypergraph edges](../../../../../../edge-of-a-hypergraph.md) as $e_1,\ldots,e_m$ and telescope

$$
\prod_{j=1}^mh_{e_j}-\prod_{j=1}^mp_{e_j}=\sum_{j=1}^m\left(\prod_{i<j}p_{e_i}\right)(h_{e_j}-p_{e_j})\left(\prod_{i>j}h_{e_i}\right).
$$

In the term for $e_j=\{a,b,c\}$, fix all variables outside this triple. Since $F$ is simple and three-uniform, every other [hypergraph edge](../../../../../../edge-of-a-hypergraph.md) intersects $\{a,b,c\}$ in at most two [vertices of a hypergraph](../../../../../../vertex-of-a-hypergraph.md). Its remaining factor therefore depends on at most two of $x_a,x_b,x_c$. Group all two-variable factors according to the pairs $(a,b),(a,c),(b,c)$. Absorb each one-variable factor into any pair containing its variable, and constants into any group. The three resulting pair [functions](../../../../../../function-split.md) remain bounded by one.

The balanced factor is now multiplied by exactly the sort of pair [functions](../../../../../../function-split.md) handled in part (ii). Its average has absolute value at most $\alpha^{1/8}$, independently of the fixed outside variables. Averaging those variables and summing the $m$ errors gives

$$
\boxed{|t_F-\prod_{e\in E(F)}p_e|\leq m\alpha^{1/8}.}
$$

Equivalently,

$$
\boxed{\left|\#F-\left(\prod_ep_e\right)\left(\prod_{i=1}^v|V_i|\right)\right|\leq |E(F)|\alpha^{1/8}\prod_{i=1}^v|V_i|.}
$$

This counts labelled copies preserving the specified [vertex of a hypergraph](../../../../../../vertex-of-a-hypergraph.md) classes, for arbitrary intersection patterns among the [hypergraph edges](../../../../../../edge-of-a-hypergraph.md), and includes the [three-uniform tetrahedron](../../../../../../three-uniform-tetrahedron.md) as a special case.

For a common host [vertex of a hypergraph](../../../../../../vertex-of-a-hypergraph.md) [set](../../../../../../set-split.md) of size $n$, the same product average counts homomorphisms. At most $\binom v2n^{v-1}$ assignments identify a pair of distinct labelled [vertices of a hypergraph](../../../../../../vertex-of-a-hypergraph.md), by the [union bound](../../../../../../boole-s-inequality.md). Thus restricting to [injective](../../../../../../injective-function.md) copies changes the estimate by at most this amount. With a common normalized [subset density](../../../../../../density-of-a-finite-subset.md) $p$ the [injective](../../../../../../injective-function.md) count is therefore $p^mn^v+O(m\alpha^{1/8}n^v+v^2n^{v-1})$. For induced copies, include the non[hypergraph edge](../../../../../../edge-of-a-hypergraph.md) [indicator functions](../../../../../../indicator-function.md) as additional factors; their balanced [functions](../../../../../../function-split.md) are negatives of the corresponding edge-balanced [functions](../../../../../../function-split.md) and have the same box [norm](../../../../../../norm.md). The same proof applies provided all the relevant triple parts satisfy the stated quasirandomness condition.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
