<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We need [independent sets](../../../../../../independent-set-graph-theory.md) in every sufficiently large remaining [induced subgraph](../../../../../../induced-subgraph.md), rather than just one in the initial [random graph](../../../../../../random-graph.md). The useful concentration variable is the maximum [edge-disjoint clique packing](../../../../../../edge-disjoint-clique-packing.md) in the [complement graph](../../../../../../complement-graph.md); changing one [edge](../../../../../../edge-of-a-graph.md) changes that variable by at most one. This avoids the much larger sensitivity of the ordinary [clique count in a binomial random graph](../../../../../../clique-count-in-a-binomial-random-graph.md).

First work in a [binomial random graph](../../../../../../binomial-random-graph.md) $H\sim G(m,1/2)$, take $r=r_0(m)$, and let $X$ count its $r$-[cliques](../../../../../../clique-graph-theory.md). Put $\mu=\mathbb EX\geq m^{9/5}$ and let $Z$ be its maximum [edge-disjoint clique packing](../../../../../../edge-disjoint-clique-packing.md) size. Form the [clique conflict graph](../../../../../../clique-conflict-graph.md) whose [vertices](../../../../../../vertex-graph-theory.md) are these [cliques](../../../../../../clique-graph-theory.md), adjacent when they share an [edge](../../../../../../edge-of-a-graph.md). If $Q$ counts unordered conflicting pairs, the [Caro-Wei bound](../../../../../../caro-wei-bound.md) gives, for each realization,

$$
Z\geq\frac{X^2}{X+2Q}.
$$

To verify the bound, randomly order the [vertices](../../../../../../vertex-graph-theory.md) of a finite [graph](../../../../../../graph-split.md) and retain each [vertex](../../../../../../vertex-graph-theory.md) preceding all its [graph neighbours](../../../../../../neighbour-of-a-vertex.md). These retained [vertices](../../../../../../vertex-graph-theory.md) are an [independent set](../../../../../../independent-set-graph-theory.md), with expected size $\sum_v(1+\deg v)^{-1}\geq X^2/(X+2Q)$ by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Interpret the ratio as zero when $X=0$. A second application of the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), now to [expectations](../../../../../../expected-value.md), gives

$$
\mathbb EZ\geq\frac{\mu^2}{\mathbb E(X+2Q)}.
$$

Counting ordered pairs of $r$-sets with $j$ common [vertices](../../../../../../vertex-graph-theory.md), including identical sets when $j=r$, yields

$$
\Delta:=\frac{\mathbb E(X+2Q)}{\mu^2}
=\sum_{j=2}^r D_j,\qquad
D_j=\frac{\binom rj\binom{m-r}{r-j}}{\binom mr}\,2^{\binom j2}.
$$

The shared [edges](../../../../../../edge-of-a-graph.md) account for the factor $2^{\binom j2}$. We claim

$$
\Delta=O(r^5/m^2)+O(1/\mu).
$$

Here are the estimates, including the large overlaps. For $2\leq j\leq\lfloor r/2\rfloor$, the probability that a random $r$-set contains any specified $j$ elements is at most $(r/(m-r))^j$. Summing over their choices inside the first $r$-set gives

$$
D_j\leq T_j:=\left(\frac{r^2}{m-r}\right)^j2^{j(j-1)/2}.
$$

The [logarithm](../../../../../../logarithm.md) of $T_j$ is a [convex function](../../../../../../convex-function.md), a quadratic in $j$, so the maximum on this interval is at an endpoint. We have $T_2=O(r^4/m^2)$. As $r=(2+o(1))\log_2m$, the other endpoint satisfies

$$
\log_2T_{\lfloor r/2\rfloor}
=-\left(\frac12+o(1)\right)(\log_2m)^2,
$$

and is smaller than $T_2$ for sufficiently large $m$. Summing at most $r$ terms gives $O(r^5/m^2)$.

For the other half of the overlaps, write $j=r-s$, where $0\leq s\leq\lceil r/2\rceil$. The exact identity and an upper bound are

$$
D_{r-s}=\frac1\mu\binom rs\binom{m-r}s2^{-sr+s(s+1)/2}
\leq\frac1\mu\left(rm\,2^{-3r/4+2}\right)^s.
$$

The quantity in parentheses is $m^{-1/2+o(1)}$, which tends to zero. The [geometric series](../../../../../../geometric-series.md) is thus at most $2/\mu$ for sufficiently large $m$. This proves the claim. In fact $r^5/m^2=o(m^{-9/5})$ and $1/\mu\leq m^{-9/5}$, so eventually

$$
\Delta\leq3m^{-9/5},\qquad \mathbb EZ\geq\frac13m^{9/5}.
$$

Now expose the $N=\binom m2$ independent [edge](../../../../../../edge-of-a-graph.md) indicators one at a time. The [edge-exposure martingale](../../../../../../edge-exposure-martingale.md) $M_i=\mathbb E[Z\mid\text{first }i\text{ indicators}]$ starts at $\mathbb EZ$ and ends at $Z$. Deleting one [edge](../../../../../../edge-of-a-graph.md) destroys at most one member of any [edge-disjoint clique packing](../../../../../../edge-disjoint-clique-packing.md). Hence changing one indicator changes $Z$ by at most one; coupling the remaining indicators shows $|M_i-M_{i-1}|\leq1$.

Precisely, the [Azuma-Hoeffding inequality](../../../../../../azuma-s-inequality.md) says that if $(M_i)_{i=0}^N$ is a [martingale](../../../../../../martingale-split.md) and $|M_i-M_{i-1}|\leq c_i$ almost surely for deterministic $c_i$, then, for $t>0$,

$$
\mathbb P(M_N-M_0\leq-t)\leq
\exp\left(-\frac{t^2}{2\sum_{i=1}^Nc_i^2}\right),
\qquad
\mathbb P(M_N-M_0\geq t)\leq
\exp\left(-\frac{t^2}{2\sum_{i=1}^Nc_i^2}\right).
$$

If all $c_i=0$, the [martingale](../../../../../../martingale-split.md) is constant. Applying the lower-tail inequality with $c_i=1$ and $t=\mathbb EZ$ gives

$$
\mathbb P(Z=0)\leq\exp\left(-\frac{(\mathbb EZ)^2}{2N}\right)
\leq\exp(-m^{8/5}/9)
$$

for sufficiently large $m$. This is the only [martingale](../../../../../../martingale-split.md) concentration inequality needed.

Return to the original [binomial random graph](../../../../../../binomial-random-graph.md) $G\sim G(n,1/2)$ and set $m=\lceil n/(\log_2n)^2\rceil$. For each fixed $m$-element [vertex](../../../../../../vertex-graph-theory.md) set $U$, the [complement graph](../../../../../../complement-graph.md) of $G[U]$ has distribution $G(m,1/2)$. The [union bound](../../../../../../boole-s-inequality.md) therefore gives

$$
\mathbb P(\text{some }U\text{ has no independent }r_0(m)\text{-set in }G[U])
\leq\binom nm e^{-m^{8/5}/9}\leq2^n e^{-m^{8/5}/9}=o(1),
$$

since $m^{8/5}/n\to\infty$. Thus [with high probability](../../../../../../with-high-probability.md) every [vertex](../../../../../../vertex-graph-theory.md) set of size at least $m$ contains an [independent set](../../../../../../independent-set-graph-theory.md) of size

$$
r_0(m)=(2+o(1))\log_2m=(2+o(1))\log_2n.
$$

Apply [greedy colouring by removing independent sets](../../../../../../greedy-colouring-by-removing-independent-sets.md): remove such an [independent set](../../../../../../independent-set-graph-theory.md), give it a fresh colour, and repeat while at least $m$ [vertices](../../../../../../vertex-graph-theory.md) remain. Give each of the fewer than $m$ final [vertices](../../../../../../vertex-graph-theory.md) its own colour. This uses at most

$$
\frac n{r_0(m)}+m=(1+o(1))\frac n{2\log_2n}
$$

colours, since $m=o(n/\log_2n)$. Together with the lower bound, **this gives the [chromatic number of the half-density binomial random graph](../../../../../../chromatic-number-of-the-half-density-binomial-random-graph.md)**:

$$
\boxed{\chi(G(n,1/2))=(1+o(1))\frac n{2\log_2n}\quad\text{with high probability}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
