<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use natural logarithms. A $K_t$ [graph minor](../../../../../graph-minor.md) is represented by $t$ disjoint nonempty [branch sets of a graph minor](../../../../../branch-set-of-a-graph-minor.md), each inducing a [connected graph](../../../../../connected-graph.md), with an [edge](../../../../../edge-of-a-graph.md) between every pair. The [complete graph minor density threshold](../../../../../complete-graph-minor-density-threshold.md) is defined over nonempty finite [graphs](../../../../../graph-split.md) by

$$
c(t)=\inf\{c:\text{for every nonempty finite }G,\ e(G)\geq c|G|\Longrightarrow G\succ K_t\}.
$$

It uses $e(G)/|G|$, half the average [degree of a vertex](../../../../../degree-graph-theory.md); the nonempty convention excludes the vacuous density inequality for the empty [graph](../../../../../graph-split.md). The PDF has the intended definition with a universal implication over $G$; the TeX transcription corrupts that definition.

**Probabilistic lower bound.** Put $N=\lfloor t\sqrt{\log t}/4\rfloor$ and take the [binomial random graph](../../../../../binomial-random-graph.md) $G(N,1/2)$. Its [edge](../../../../../edge-of-a-graph.md) count has mean $N(N-1)/4$. The [Chernoff bound](../../../../../chernoff-bound.md) implies

$$
\mathbb P(e(G)\geq N^2/8)\longrightarrow1.
$$

We show that the [probability](../../../../../probability.md) of a $K_t$ [graph minor](../../../../../graph-minor.md) tends to zero. Ignore connectedness, which only enlarges the set of possible models, and assign each of the $N$ [vertices](../../../../../vertex-graph-theory.md) one of $t$ branch labels or an unused label. There are at most $(t+1)^N$ assignments.

For any assignment with $t$ nonempty branch sets, at least $t/2$ of them have size at most $2N/t\leq\sqrt{\log t}/2$. Between any two such small sets $A,B$, the [probability](../../../../../probability.md) of no [edge](../../../../../edge-of-a-graph.md) is

$$
2^{-|A||B|}\geq \exp\left(-\frac{\log2}{4}\log t\right)\geq t^{-1/4}.
$$

The absence or presence of [edges](../../../../../edge-of-a-graph.md) between different pairs of branch sets depends on disjoint sets of random [edges](../../../../../edge-of-a-graph.md), so these events are independent. For this assignment the [probability](../../../../../probability.md) that all small pairs are adjacent is at most

$$
(1-t^{-1/4})^{\binom{\lfloor t/2\rfloor}{2}}
\leq\exp\left(-\binom{\lfloor t/2\rfloor}{2}t^{-1/4}\right).
$$

The [union bound](../../../../../boole-s-inequality.md) over assignments is therefore at most

$$
\exp\left(N\log(t+1)-\binom{\lfloor t/2\rfloor}{2}t^{-1/4}\right)\longrightarrow0,
$$

since the positive term is $O(t(\log t)^{3/2})$ and the negative term has order $t^{7/4}$. There is consequently a [graph](../../../../../graph-split.md) with no $K_t$ [graph minor](../../../../../graph-minor.md) and with $e(G)/N\geq N/8$. Any constant having the universal forcing property must exceed this ratio. Since $N/8\geq t\sqrt{\log t}/64$ for large $t$,

$$
\boxed{c(t)\geq\beta t\sqrt{\log t}\quad\text{with }\beta=1/64.}
$$

**The auxiliary density lemma contains a typo.** Both the original PDF and the TeX print $e(G)\leq11k|G|$ in the hint. This cannot imply its conclusion: for $k\geq1$, an edgeless [graph](../../../../../graph-split.md) has only edgeless [graph minors](../../../../../graph-minor.md), and none satisfies $2\delta(H)\geq|H|+4k-1$. We use the intended [dense minor with bounded order and high minimum degree](../../../../../dense-minor-with-bounded-order-and-high-minimum-degree.md) lemma with the hypothesis $e(G)\geq11k|G|$ for nonempty $G$. The upper-bound argument below depends on that corrected supplied lemma; the literal printed hint is false.

**Probabilistic upper bound and the constant seven.** Suppose $G$ is nonempty and $e(G)\geq7t\sqrt{\log t}|G|$, and set

$$
k=\left\lfloor\frac7{11}t\sqrt{\log t}\right\rfloor,\qquad
\ell=\lceil\sqrt{\log t}\rceil.
$$

The corrected lemma gives a [graph minor](../../../../../graph-minor.md) $H$ of order $N\leq11k+2$ with $2\delta(H)\geq N+4k-1$. Since $\delta(H)\leq N-1$, we also have $N\geq4k+1$. For large $k$, every [vertex](../../../../../vertex-graph-theory.md) has at most $N/3$ nonneighbours, counting itself, because

$$
N-\delta(H)\leq N/2-2k+1/2\leq N/3;
$$

the last inequality uses $N\leq11k+2\leq12k-3$. Moreover any two distinct [vertices](../../../../../vertex-graph-theory.md) have at least

$$
2\delta(H)-N\geq4k-1
$$

[common neighbours](../../../../../common-neighbour.md).

Choose $2t$ disjoint random $\ell$-sets $A_1,\ldots,A_{2t}$ from $V(H)$, uniformly, which is possible since $2t\ell<4k-1\leq N$ for sufficiently large $t$. For a set $A$, let $U(A)$ be the set of [vertices](../../../../../vertex-graph-theory.md) having no neighbour in $A$. For each [vertex](../../../../../vertex-graph-theory.md), the [probability](../../../../../probability.md) that all members of a uniformly sampled $\ell$-set are its nonneighbours is at most $3^{-\ell}$, even when sampling without replacement. By linearity of [expected value](../../../../../expected-value.md),

$$
\mathbb E|U(A)|\leq N3^{-\ell}.
$$

Call $A$ good if $|U(A)|\leq N3^{-19\ell/20}$. The [Markov inequality](../../../../../markov-inequality.md) shows that a random set is bad with [probability](../../../../../probability.md) at most $3^{-\ell/20}=o(1)$. Thus the expected number of bad sets among our $2t$ samples is $o(t)$.

Conditional on a fixed good $A_i$, the marginal distribution of $A_j$ is uniform among $\ell$-sets outside $A_i$. For there to be no [edge](../../../../../edge-of-a-graph.md) between them, all its members must lie in $U(A_i)$. Hence

$$
\mathbb P(A_i\text{ good and }e(A_i,A_j)=0)
\leq\left(\frac{N3^{-19\ell/20}}{N-\ell}\right)^\ell.
$$

Here $(N/(N-\ell))^\ell=\exp(O(\ell^2/N))=1+o(1)$. Consequently the expected number of nonadjacent pairs of good sets is at most

$$
\binom{2t}{2}(1+o(1))3^{-19\ell^2/20}
=O\left(t^{2-(19/20)\log3}\right)=o(t),
$$

since $(19/20)\log3>1$. Applying the [Markov inequality](../../../../../markov-inequality.md) to both counts shows that there exists a choice with fewer than $t$ bad sets and at most $t$ nonadjacent pairs of good sets. Select $t$ of the good sets; they still have at most $t$ missing adjacencies.

Make each selected set connected by fixing one of its [vertices](../../../../../vertex-graph-theory.md) as a root and, for each of its other members, adding one unused [common neighbour](../../../../../common-neighbour.md) of that member and the root. This uses at most $t(\ell-1)$ additional [vertices](../../../../../vertex-graph-theory.md). Then for each pair with no original [edge](../../../../../edge-of-a-graph.md), choose one [vertex](../../../../../vertex-graph-theory.md) in each set and add an unused [common neighbour](../../../../../common-neighbour.md) to one of the sets. The added [vertex](../../../../../vertex-graph-theory.md) is joined to that set and to the other set, so it preserves connectedness and repairs their adjacency. At most $t$ such repairs are required.

Throughout this process the total number of occupied [vertices](../../../../../vertex-graph-theory.md) is at most

$$
t\ell+t(\ell-1)+t=2t\ell<4k-1.
$$

Since every pair has at least $4k-1$ [common neighbours](../../../../../common-neighbour.md), an unused choice always exists. The final sets are disjoint connected [branch sets of a graph minor](../../../../../branch-set-of-a-graph-minor.md) with every pair adjacent. They represent $K_t$ in $H$, and hence in $G$, by transitivity of [graph minors](../../../../../graph-minor.md). This [random branch-set construction of a complete graph minor](../../../../../random-branch-set-construction-of-a-complete-graph-minor.md) proves

$$
\boxed{c(t)\leq7t\sqrt{\log t}\quad\text{for sufficiently large }t.}
$$

**The sharp linear threshold for a four-vertex complete minor.** We prove by induction that a [graph](../../../../../graph-split.md) on $n\geq4$ [vertices](../../../../../vertex-graph-theory.md) with at least $2n-2$ [edges](../../../../../edge-of-a-graph.md) has a $K_4$ [graph minor](../../../../../graph-minor.md). The case $n=4$ is $K_4$ itself. If some [edge](../../../../../edge-of-a-graph.md) $uv$ has at most one [common neighbour](../../../../../common-neighbour.md), an [edge contraction](../../../../../edge-contraction.md) reduces the order by one and removes exactly $1+|N(u)\cap N(v)|\leq2$ [edges](../../../../../edge-of-a-graph.md). The contracted [graph](../../../../../graph-split.md) has at least $2(n-1)-2$ [edges](../../../../../edge-of-a-graph.md), so induction applies.

Otherwise every [edge](../../../../../edge-of-a-graph.md) is in at least two [triangles in a graph](../../../../../triangle-in-a-graph.md). Choose a [vertex](../../../../../vertex-graph-theory.md) $v$ incident with an [edge](../../../../../edge-of-a-graph.md). Each [vertex](../../../../../vertex-graph-theory.md) $u\in N(v)$ has at least two [neighbours of a vertex](../../../../../neighbour-of-a-vertex.md) in $N(v)$, since these are the [common neighbours](../../../../../common-neighbour.md) of $u,v$. Thus $G[N(v)]$ has [minimum degree of a graph](../../../../../minimum-degree-of-a-graph.md) at least two. A longest path in this finite [graph](../../../../../graph-split.md) has an endpoint adjacent to an earlier nonconsecutive path [vertex](../../../../../vertex-graph-theory.md), and hence contains a [cycle in a graph](../../../../../cycle-in-a-graph.md). Together with $v$, this [cycle in a graph](../../../../../cycle-in-a-graph.md) gives a [wheel graph](../../../../../wheel-graph.md) as a [subgraph](../../../../../subgraph.md). Divide its rim into three consecutive nonempty connected arcs; these arcs and $\{v\}$ form four pairwise adjacent [branch sets of a graph minor](../../../../../branch-set-of-a-graph-minor.md). Therefore

$$
\boxed{e(G)\geq2n-2\ \Longrightarrow\ G\succ K_4.}
$$

With $2n-3$ [edges](../../../../../edge-of-a-graph.md) the answer is **no**. Take the [join of graphs](../../../../../join-graph-theory.md) of $K_2$ and an [independent set](../../../../../independent-set-graph-theory.md) of $n-2$ [vertices](../../../../../vertex-graph-theory.md). It has $1+2(n-2)=2n-3$ [edges](../../../../../edge-of-a-graph.md). Among four disjoint putative [branch sets of a graph minor](../../../../../branch-set-of-a-graph-minor.md), at most two can contain the two [vertices](../../../../../vertex-graph-theory.md) of $K_2$. Any connected branch set avoiding them is a singleton in the [independent set](../../../../../independent-set-graph-theory.md). At least two such singleton sets would therefore have no [edge](../../../../../edge-of-a-graph.md) between them. This excludes a $K_4$ [graph minor](../../../../../graph-minor.md) for every $n\geq4$ and proves sharpness.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 110](../../paper-110-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
