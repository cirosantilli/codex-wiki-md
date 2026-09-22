<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose a fixed [prime](../../../../../../prime-number.md) $p\geq k$, and put $s=2p-2$. We first derive the [polynomial](../../../../../../polynomial-split.md) step: a [graph](../../../../../../graph-split.md) $H$ on $N$ [vertices](../../../../../../vertex-graph-theory.md) and $M>(p-1)N$ [edges](../../../../../../edge-of-a-graph.md), with maximum degree at most $2p-1$, contains a nonempty $p$-regular subgraph. Use a Boolean variable $x_e$ for each [edge](../../../../../../edge-of-a-graph.md) and work over $\mathbb F_p$. Define

$$
R(x)=\prod_{v\in V(H)}\left[1-\left(\sum_{e\ni v}x_e\right)^{p-1}\right]-\prod_{e\in E(H)}(1-x_e).
$$

The first product has degree at most $(p-1)N<M$, while the full squarefree [monomial](../../../../../../monomial.md) $\prod_e x_e$ has [coefficient](../../../../../../coefficient.md) $(-1)^{M+1}\ne0$ in the second term with its minus sign. The [Combinatorial Nullstellensatz](../../../../../../combinatorial-nullstellensatz.md), with every grid $\{0,1\}$, gives a nonzero value of $R$. Since $R(0)=0$, this is a nonempty [edge](../../../../../../edge-of-a-graph.md) selection. The second product is then zero, so the first is nonzero. [Fermat's little theorem](../../../../../../fermat-little-theorem.md) makes each selected [vertex](../../../../../../vertex-graph-theory.md) degree zero modulo $p$. The maximum-degree bound implies that every positive selected degree is precisely $p$. This proves the [prime-regular subgraph from Boolean polynomial constraints](../../../../../../prime-regular-subgraph-from-boolean-polynomial-constraints.md).

We next turn density into an almost-regular bipartite subgraph, keeping the logarithmic loss explicit. Let the original [graph](../../../../../../graph-split.md) have $n\geq2$ [vertices](../../../../../../vertex-graph-theory.md) and $m>0$ [edges](../../../../../../edge-of-a-graph.md). Some bipartition retains at least $m/2$ [edges](../../../../../../edge-of-a-graph.md): choose the sides independently with [probability](../../../../../../probability.md) $1/2$ and average the number crossing. Its average degree is at least $m/n$. Repeatedly delete a [vertex](../../../../../../vertex-graph-theory.md) of degree at most half the current average degree. Such a deletion cannot lower that average, since

$$
\frac{2(e-d(v))}{N-1}\geq\frac{2e}{N}\quad\Longleftrightarrow\quad d(v)\leq e/N.
$$

The process cannot delete the last positive-density [graph](../../../../../../graph-split.md), because the maintained average is positive. At termination the minimum degree is an [integer](../../../../../../integer.md) $\sigma>m/(2n)$.

Choose the larger side $A$ of this remaining [bipartite graph](../../../../../../bipartite-graph.md), with opposite side $B$. Keep exactly $\sigma$ [edges](../../../../../../edge-of-a-graph.md) at each [vertex](../../../../../../vertex-graph-theory.md) of $A$; choices at different [vertices](../../../../../../vertex-graph-theory.md) of $A$ do not conflict. Remove any now-isolated [vertices](../../../../../../vertex-graph-theory.md) of $B$. Thus $|A|\geq|B|$, and every [vertex](../../../../../../vertex-graph-theory.md) of $A$ has degree $\sigma$.

Such a half-regular [graph](../../../../../../graph-split.md) contains a half-regular restriction with a [perfect matching](../../../../../../perfect-matching.md). Choose a minimal nonempty $X\subseteq A$ satisfying $|N(X)|\leq|X|$, which exists because the whole side $A$ satisfies this inequality. In fact equality holds: if it were strict, deleting a [vertex](../../../../../../vertex-graph-theory.md) of $X$ would retain the inequality, contradicting minimality; the singleton case has at least one neighbor. Every proper [subset](../../../../../../subset.md) $Y\subset X$ satisfies $|N(Y)|\geq|Y|$. [Hall's marriage theorem](../../../../../../hall-s-marriage-theorem.md) therefore supplies a [perfect matching](../../../../../../perfect-matching.md) on $X\cup N(X)$. All $\sigma$ [edges](../../../../../../edge-of-a-graph.md) incident with each [vertex](../../../../../../vertex-graph-theory.md) of $X$ remain inside that restriction.

Delete this [perfect matching](../../../../../../perfect-matching.md) and repeat the restriction argument. The left degrees decrease by one at each step. We obtain $\sigma$ edge-disjoint [perfect matchings](../../../../../../perfect-matching.md) $M_0,\ldots,M_{\sigma-1}$ on nested nonempty [vertex](../../../../../../vertex-graph-theory.md) sets, with sizes

$$
n=N_{-1}\geq N_0\geq N_1\geq\cdots\geq N_{\sigma-1}\geq2.
$$

For any $i$ with $i+s\leq\sigma-1$, the union of $s+1=2p-1$ consecutive [matchings in a graph](../../../../../../matching-graph-theory.md) has maximum degree at most $2p-1$ and at least $(s+1)N_{i+s}/2$ [edges](../../../../../../edge-of-a-graph.md) on $N_i$ [vertices](../../../../../../vertex-graph-theory.md). If

$$
N_{i+s}>\frac{s}{s+1}N_i,
$$

it has more than $(p-1)N_i$ [edges](../../../../../../edge-of-a-graph.md), so the [polynomial](../../../../../../polynomial-split.md) step yields a $p$-regular bipartite subgraph. Every regular [bipartite graph](../../../../../../bipartite-graph.md) decomposes into [perfect matchings](../../../../../../perfect-matching.md): for a set in one part, counting incident [edges](../../../../../../edge-of-a-graph.md) gives Hall's inequality, so a [perfect matching](../../../../../../perfect-matching.md) exists; remove it and repeat. Choosing $k$ of these $p$ [matchings in a graph](../../../../../../matching-graph-theory.md) gives a nonempty $k$-regular subgraph. This is the [nested matching criterion for a regular subgraph](../../../../../../nested-matching-criterion-for-a-regular-subgraph.md).

If no $k$-regular subgraph exists, every displayed size ratio must therefore satisfy the reverse inequality. Iterating at indices $0,s,2s,\ldots$ gives, with $r=\lfloor(\sigma-1)/s\rfloor$,

$$
2\leq N_{rs}\leq n\left(\frac{s}{s+1}\right)^r.
$$

Consequently $r\leq\log n/\log((s+1)/s)$ and

$$
\sigma\leq1+s\left(1+\frac{\log n}{\log((s+1)/s)}\right).
$$

Combining with $\sigma>m/(2n)$ proves the required [edge](../../../../../../edge-of-a-graph.md) bound. For example the finite constant

$$
c_k=2\left(\frac{1+s}{\log2}+\frac{s}{\log((s+1)/s)}\right),\qquad s=2p-2,\ p\geq k\text{ fixed prime},
$$

works for every $n\geq2$, and the case $n=1$ has no [edges](../../../../../../edge-of-a-graph.md). Thus

$$
\boxed{m\leq c_k n\log n.}
$$

The logarithm comes from how often a nested [matching in a graph](../../../../../../matching-graph-theory.md) [vertex](../../../../../../vertex-graph-theory.md) set can shrink by a fixed factor before becoming empty; it is not supplied by the [polynomial](../../../../../../polynomial-split.md) step alone.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
