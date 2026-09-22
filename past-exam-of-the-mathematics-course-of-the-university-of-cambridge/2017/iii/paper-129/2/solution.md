<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $d(U,V)=e(U,V)/(|U||V|)$ for the [edge density of a bipartite graph](../../../../../edge-density-of-a-bipartite-graph.md) between nonempty disjoint [vertex](../../../../../vertex-graph-theory.md) sets. A [regular pair of vertex sets](../../../../../regular-pair-of-vertex-sets.md) $(U,V)$ is $\varepsilon$-regular if $|d(U',V')-d(U,V)|\leq\varepsilon$ whenever $U'\subseteq U$, $V'\subseteq V$, $|U'|\geq\varepsilon|U|$, and $|V'|\geq\varepsilon|V|$.

The [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md) says that for every $\varepsilon>0$ and positive [integer](../../../../../integer.md) $m_0$ there is $M=M(\varepsilon,m_0)$ such that every finite simple [graph](../../../../../graph-split.md) on $N\geq m_0$ [vertices](../../../../../vertex-graph-theory.md) has a [set partition](../../../../../set-partition.md)

$$
V=V_0\sqcup V_1\sqcup\cdots\sqcup V_k,
\qquad m_0\leq k\leq M,
\qquad |V_0|\leq\varepsilon N,
$$

where $V_1,\ldots,V_k$ have equal positive size and at most $\varepsilon k^2$ unordered pairs $(V_i,V_j)$, $i<j$, fail to be [regular pairs of vertex sets](../../../../../regular-pair-of-vertex-sets.md). The version requiring only sufficiently large $N$ is equivalent, since the finitely many smaller admissible sizes can use [singleton sets](../../../../../singleton-mathematics.md) as classes. It suffices to prove this for $0<\varepsilon\leq1/2$: reducing a larger parameter to $1/2$ gives stronger conclusions.

Here is a complete energy proof, including restoration of equal class sizes. For a [set partition](../../../../../set-partition.md) with exceptional set $V_0$, use the following version of [equitable regularity energy](../../../../../equitable-regularity-energy.md), omitting pairs incident with $V_0$:

$$
q(\mathcal P)=\frac1{N^2}\sum_{i,j\geq1}|V_i||V_j|d(V_i,V_j)^2,\qquad0\leq q(\mathcal P)\leq1.
$$

For $i=j$, define $d(V_i,V_i)$ using the ordered adjacency [indicator function](../../../../../indicator-function.md), with diagonal entries zero. Thus the same formula works on every rectangle. The [refinement variance identity for regularity energy](../../../../../refinement-variance-identity-for-regularity-energy.md) is

$$
\sum_{A\subseteq U,\ B\subseteq V}|A||B|d(A,B)^2-|U||V|d(U,V)^2
=\sum_{A,B}|A||B|\bigl(d(A,B)-d(U,V)\bigr)^2,
$$

where $A,B$ run over the refined cells. Expanding the square proves the identity because their weighted mean [edge density of a bipartite graph](../../../../../edge-density-of-a-bipartite-graph.md) is $d(U,V)$. In particular, refinement never decreases the energy. If a union of refined cells $U'\times V'$ has discrepancy greater than $\varepsilon$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) bounds its contribution below by $|U'||V'|\varepsilon^2/N^2$. For an irregular equal-class pair of size $L$, witnesses have sizes at least $\varepsilon L$, so the increase exceeds $\varepsilon^4L^2/N^2$ in each orientation.

Choose $k_0\geq\max\{m_0,2\}$ so large that $2^{-k_0}\leq\varepsilon^6/100$. Initially partition into $k_0$ equal classes and fewer than $k_0$ exceptional [vertices](../../../../../vertex-graph-theory.md). For sufficiently large $N$ this exceptional set has size at most $\varepsilon N/2$. Suppose there are more than $\varepsilon k^2$ irregular unordered pairs at a subsequent step, with equal class size $L$. Choose one witnessing pair of subsets for every such pair. Split each class according to membership in all its witness subsets; each class produces at most $2^k$ atoms. The preceding [refinement variance identity for regularity energy](../../../../../refinement-variance-identity-for-regularity-energy.md) shows that the energy increase exceeds

$$
2\varepsilon k^2\frac{\varepsilon^4L^2}{N^2}
=2\varepsilon^5\left(\frac{kL}{N}\right)^2
\geq\frac{\varepsilon^5}{2},
$$

as long as the exceptional set has size at most $\varepsilon N\leq N/2$.

Apply [equalization with a controlled exceptional set](../../../../../equalization-with-a-controlled-exceptional-set.md). Set $\ell=\lfloor L/4^k\rfloor$, cut every atom into blocks of size $\ell$, and send its leftover points to $V_0$. Provided $L\geq2\cdot4^k$, the new number $k'$ of classes satisfies

$$
k\leq k'\leq2k4^k.
$$

The lower bound holds because every old class retains at least one full block: its leftovers total less than $2^k\ell<L$. The discarded fraction is at most

$$
r\leq\frac{k2^k\ell}{N}\leq2^{-k}\leq\frac{\varepsilon^6}{100}.
$$

Cutting blocks is a further refinement before discarding. Discarding changes only ordered pairs with at least one discarded [vertex](../../../../../vertex-graph-theory.md), so it loses at most $2r$ in the energy. The net increase is therefore at least $\varepsilon^5/2-2\varepsilon^6/100\geq\varepsilon^5/4$.

There can be fewer than $T=\lceil4\varepsilon^{-5}\rceil$ such strict energy increases, because the energy stays in $[0,1]$. Through $T$ steps the exceptional fraction is at most

$$
\frac\varepsilon2+T\frac{\varepsilon^6}{100}
\leq\frac\varepsilon2+\frac{4\varepsilon+\varepsilon^6}{100}<\varepsilon.
$$

This also verifies the exceptional-set bound used at every preceding step. Iterating the finite recursion $k\mapsto2k4^k$ at most $T$ times bounds all class counts by some $K=K(\varepsilon,m_0)$. Choosing $N$ sufficiently large in terms of $K$, for instance with $N\geq4K4^K$ and $N\geq2k_0/\varepsilon$, guarantees $L=(N-|V_0|)/k\geq N/(2K)\geq2\cdot4^k$ throughout. Thus the process terminates with the desired [regular pairs of vertex sets](../../../../../regular-pair-of-vertex-sets.md). Choose a finite integer threshold $N_*$ for these requirements and set $M\geq\max\{K,N_*\}$. For $m_0\leq N<N_*$, use $N$ [singleton sets](../../../../../singleton-mathematics.md); every pair is regular because its only admissible nonempty subsets are the whole pair. This completes the [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md) for all admissible $N$.

For the [half graph](../../../../../half-graph.md), a class of size $s$ has exactly $\lceil s/10\rceil$ elements with fewer than $s/10$ predecessors, and the same number with fewer than $s/10$ successors. Thus its boundary contains at most $2\lceil s/10\rceil$ elements. Let $k_X,k_Y$ be the numbers of classes. The [boundary rank obstruction in a half graph](../../../../../boundary-rank-obstruction-in-a-half-graph.md) gives the union bound

$$
B\leq2\sum_i\left\lceil\frac{|X_i|}{10}\right\rceil
+2\sum_j\left\lceil\frac{|Y_j|}{10}\right\rceil
\leq\frac{2n}{5}+2(k_X+k_Y)
\leq\boxed{\frac{11n}{25}}<n,
$$

because $k_X,k_Y\leq n/100$. There is therefore an index $m$ away from both boundaries. In its classes $X_i,Y_j$, all four subsets $X^- =\{x<m\}$, $X^+=\{x>m\}$, $Y^-=\{y<m\}$, $Y^+=\{y>m\}$ have at least one tenth of their respective class sizes. These subsets are taken within $X_i,Y_j$, which need not be intervals.

In the [half graph](../../../../../half-graph.md), $d(X^-,Y^+)=1$ and $d(X^+,Y^-)=0$. If $(X_i,Y_j)$ were a $1/10$-[regular pair of vertex sets](../../../../../regular-pair-of-vertex-sets.md), both values would be within $1/10$ of $d(X_i,Y_j)$, implying $1\leq2/10$, a contradiction. **At least one class pair is not $1/10$-regular.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 129](../../paper-129-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
