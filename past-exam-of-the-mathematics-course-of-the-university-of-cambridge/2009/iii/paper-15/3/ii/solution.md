<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We first specify the standard hypotheses of [percolation uniqueness on an amenable quasi-transitive graph](../../../../../../percolation-uniqueness-on-an-amenable-quasi-transitive-graph.md). A [locally finite graph](../../../../../../locally-finite-graph.md) has finite degree at every vertex; a [quasi-transitive graph](../../../../../../quasi-transitive-graph.md), or graph of finite type, has finitely many vertex orbits under the acting group $\Gamma$ of [graph automorphisms](../../../../../../graph-automorphism.md). Here the [site percolation](../../../../../../site-percolation-split.md) law is invariant under $\Gamma$ and independent, with one parameter $p_j$ for each orbit. Initially suppose $0<p_j<1$. This gives the [finite-energy property of Bernoulli percolation](../../../../../../finite-energy-property-of-bernoulli-percolation.md): conditional on all states outside any finite set, every assignment inside that set has positive [probability](../../../../../../probability.md). An [amenable graph](../../../../../../amenable-graph.md) has finite sets $W_n$ with $|\partial^+W_n|/|W_n|\to0$, where $\partial^+W_n$ denotes the external vertex boundary. Finite type bounds the degrees uniformly, so internal and external boundary conventions are equivalent here.

Let $N$ be the number of [infinite percolation clusters](../../../../../../infinite-percolation-cluster.md), taking values in $\{0,1,2,\ldots,\infty\}$. Each event $\{N=j\}$ is invariant. Part (i), together with countability of these possibilities, shows that $N$ is an almost-sure constant.

Suppose first that this constant is a finite integer $j\ge2$. Some finite connected set $F$ meets all $j$ [infinite percolation clusters](../../../../../../infinite-percolation-cluster.md) with positive [probability](../../../../../../probability.md), since increasing finite sets exhaust the graph. Make every vertex of $F$ open. This joins all the infinite clusters. Opening a finite set cannot produce a new infinite cluster from finite clusters: only finitely many clusters meet its finite boundary, and their finite union is finite. By the [finite-energy property](../../../../../../finite-energy-property-percolation.md) the modified event has positive [probability](../../../../../../probability.md), contradicting the almost-sure value $j$. Thus a finite $N$ must be $0$ or $1$.

Suppose instead that $N=\infty$ almost surely. Some finite connected set $F$ meets three distinct [infinite percolation clusters](../../../../../../infinite-percolation-cluster.md) with positive [probability](../../../../../../probability.md). Open all of $F$. Its vertices belong to one open cluster, and deleting $F$ from that cluster leaves at least three infinite components. This is an [encounter box in percolation](../../../../../../encounter-box-in-percolation.md). We use boxes rather than assume that the local geometry permits a single [trifurcation vertex in percolation](../../../../../../trifurcation-vertex-in-percolation.md).

Here is the boundary-counting contradiction in detail. Translates of $F$ have the same positive encounter [probability](../../../../../../probability.md). Finite type and bounded degree allow a deterministic packing of mutually disjoint such translates whose centers have positive lower density in the interiors of the [Følner sets](../../../../../../folner-set.md) $W_n$: every vertex is within a fixed distance of one chosen orbit, and a bounded-radius greedy packing discards only a bounded number of possible centers per chosen center. Boundary layers of any fixed thickness have size $o(|W_n|)$. The expected number of encounter boxes wholly inside $W_n$ is consequently at least $c|W_n|$ for a fixed $c>0$ and all large $n$.

On the other hand, contract the open encounter boxes in each cluster to vertices and retain the part inside $W_n$. Each contracted encounter box separates at least three branches that run to infinity, and each branch must leave $W_n$. Choose a minimal forest connecting all these boundary exits. Every encounter junction has degree at least three in that forest: its three infinite branches remain in different components after deleting the junction, so none can be omitted. The leaves are boundary exits. For each nontrivial [tree](../../../../../../tree-graph-theory.md), the degree-sum identity gives at most the number of leaves minus two vertices of degree at least three. Thus the number of encounter boxes is at most a constant times $|\partial^+W_n|$, where the constant accounts for the bounded boundary degrees. Taking [expected values](../../../../../../expected-value.md) contradicts amenability. This excludes $N=\infty$ and proves

$$
\boxed{\mathbb P_{\boldsymbol p}(I_0)=1\quad\text{or}\quad\mathbb P_{\boldsymbol p}(I_1)=1.}
$$

There is a genuine endpoint qualification if different orbit parameters are allowed to be $0$ or $1$. Subdivide each horizontal edge of the [square lattice](../../../../../../square-lattice.md) once. Open every original vertex deterministically and close every new midpoint deterministically. This is an invariant independent law on an [amenable graph](../../../../../../amenable-graph.md) that is also a [quasi-transitive graph](../../../../../../quasi-transitive-graph.md), but its infinite open clusters are the distinct vertical columns. Thus the [finite-energy property](../../../../../../finite-energy-property-percolation.md) must be included when interpreting a general vector $\boldsymbol p$. The homogeneous endpoint laws themselves cause no problem: they give zero or one infinite cluster.

**The conclusion is false for $k$-independent laws, even with all site marginals equal to $1/2$.** Here is a fully specified [monochromatic line-graph percolation counterexample](../../../../../../monochromatic-line-graph-percolation-counterexample.md). Form a graph $B$ by replacing each vertex of $\mathbb Z^2$ by a [complete graph](../../../../../../complete-graph.md) on ten vertices and putting every possible edge between the blocks of two neighboring lattice vertices. Every vertex of $B$ has degree $9+4\cdot10=49$. The graph is connected, periodic and amenable: a square of blocks has volume of order $n^2$ and boundary of order $n$. Assign independent fair red/blue colors to the vertices of $B$.

Call a block good when it contains both colors. Good-block indicators are independent, with

$$
g=1-2\cdot2^{-10}=511/512.
$$

They percolate. To verify this without presupposing a site threshold, put $q=1-g=1/512$. A finite nearest-neighbor good-block cluster around a good origin is surrounded by a circuit of bad blocks in the matching square graph, where horizontal, vertical and diagonal neighbors are allowed. A surrounding circuit of length $\ell$ has an anchor within $[-\ell,\ell]^2$. Overcounting its choices by $9\ell^2 8^\ell$ gives the [Peierls argument](../../../../../../peierls-argument.md)

$$
\mathbb P(\text{the origin has no infinite good-block cluster})\le q+\sum_{\ell\ge3}9\ell^2(8q)^\ell<0.003<1.
$$

The sum bound follows directly from $\sum_{\ell\ge1}\ell^2r^\ell=r(1+r)/(1-r)^3$, with $r=1/64$. An infinite good-block cluster therefore exists with positive [probability](../../../../../../probability.md), and by part (i) it exists almost surely. Inside each of its blocks the red vertices are connected to one another, as are the blue vertices; between adjacent good blocks the complete bipartite joining edges connect each color. Hence $B$ has both an infinite red component and an infinite blue component almost surely.

Now use [site percolation](../../../../../../site-percolation-split.md) on $\Gamma=L(B)$, the [line graph](../../../../../../line-graph.md) of $B$: its vertices are the edges $\{u,v\}$ of $B$, two adjacent when they share an endpoint. Declare such a site open exactly when $u,v$ have the same color. Each site has open [probability](../../../../../../probability.md) $1/2$. Sets of sites at [graph distance](../../../../../../distance-graph-theory.md) greater than one involve disjoint sets of underlying color variables, so this is a translation-invariant $1$-independent law. The [line graph](../../../../../../line-graph.md) is again connected, locally finite, amenable and of finite type. The infinite red and blue components of $B$ yield infinite open clusters in $L(B)$. An open path in $L(B)$ cannot change color at a shared endpoint, so those two clusters are distinct. Thus $N\ge2$ almost surely. Local color constraints destroy the [finite-energy property](../../../../../../finite-energy-property-percolation.md), precisely the ingredient missing from the uniqueness proof.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
