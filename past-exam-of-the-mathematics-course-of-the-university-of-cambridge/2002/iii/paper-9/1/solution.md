<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $K_s(t)$ for a [balanced complete multipartite blow-up](../../../../../balanced-complete-multipartite-blow-up.md) with $s$ classes of size $t$. In the nonvacuous range $0<\varepsilon<1/r$, the answer is

$$
\boxed{t(r,\varepsilon,n)=\Theta_{r,\varepsilon}(\log n).}
$$

We prove both bounds, including the quantitative lower bound.

First, suppose a [bipartite graph](../../../../../bipartite-graph.md) with parts $A,B$, of sizes $m,N$, has at least $pmN$ [edges](../../../../../edge-of-a-graph.md). For any [integer](../../../../../integer.md) $s\le pm/2$, counting pairs consisting of an $s$-subset of $A$ and a [common neighbour](../../../../../common-neighbour.md) in $B$ gives

$$
\sum_{S\in\binom As}|N(S)|=\sum_{v\in B}\binom{d_A(v)}s\ge N\binom{\lfloor pm\rfloor}s.
$$

The inequality follows from discrete [convexity](../../../../../convex-function.md): $\binom{x+1}s-\binom xs=\binom{x}{s-1}$ is nondecreasing, so balancing [integer](../../../../../integer.md) [degrees of vertices](../../../../../degree-graph-theory.md) minimizes their sum. Consequently some $S$ has

$$
|N(S)|\ge N\frac{\binom{\lfloor pm\rfloor}s}{\binom ms}
\ge N\left(\frac{pm-s}{m}\right)^s\ge N(p/2)^s.
$$

The product estimate uses $\lfloor pm\rfloor-j\ge pm-s$ for $0\le j<s$. This is a [common neighbourhood from bipartite density](../../../../../common-neighbourhood-from-bipartite-density.md) bound.

We next prove by [induction](../../../../../mathematical-induction.md) on $q\ge1$ that, for every fixed $\alpha>0$, a [graph](../../../../../graph-split.md) $J$ of order $N$ with [minimum degree](../../../../../minimum-degree-of-a-graph.md) at least $(1-1/q+\alpha)N$ contains $K_{q+1}(\lfloor c\log N\rfloor)$, for some $c=c(q,\alpha)>0$ and all sufficiently large $N$. Impossible minimum-[vertex degree](../../../../../degree-graph-theory.md) parameters need no argument. For $q=1$, take two copies of $V(J)$ with adjacency given by $J$. The preceding count with $p=\alpha$ and $s=\lfloor c\log N\rfloor$, where $c\log(2/\alpha)<1/2$, gives at least $\sqrt N$ [common neighbours](../../../../../common-neighbour.md). The selected [vertices](../../../../../vertex-graph-theory.md) and their [common neighbours](../../../../../common-neighbour.md) are disjoint in $J$, since a [vertex](../../../../../vertex-graph-theory.md) is not its own [neighbour](../../../../../neighbour-of-a-vertex.md). Selecting $s$ [common neighbours](../../../../../common-neighbour.md) gives $K_2(s)$.

For $q\ge2$, the [minimum degree](../../../../../minimum-degree-of-a-graph.md) hypothesis implies the [induction](../../../../../mathematical-induction.md) hypothesis for $q-1$, for example with excess $1/[q(q-1)]$. Thus $J$ contains $K_q(m)$ with $m=\lfloor a\log N\rfloor$ for a positive constant $a$. Pair the [vertices](../../../../../vertex-graph-theory.md) in its classes into $m$ disjoint transversal [cliques](../../../../../clique-graph-theory.md) $C_1,\ldots,C_m$, each of order $q$. By the [union bound](../../../../../boole-s-inequality.md), every $C_i$ has at least

$$
N-q\bigl(N-\delta(J)\bigr)\ge q\alpha N
$$

[common neighbours](../../../../../common-neighbour.md). Form an auxiliary [bipartite graph](../../../../../bipartite-graph.md) between these $m$ [cliques](../../../../../clique-graph-theory.md) and the $N$ [vertices](../../../../../vertex-graph-theory.md), using common-neighbour incidence, and put $p=q\alpha$. Choose $c>0$ small enough that $c<pa/3$ and $c\log(2/p)<1/2$. The count above, with $s=\lfloor c\log N\rfloor$, gives $s$ [cliques](../../../../../clique-graph-theory.md) with at least $\sqrt N$ simultaneous [common neighbours](../../../../../common-neighbour.md). Their [vertices](../../../../../vertex-graph-theory.md) form $q$ classes of size $s$, and $s$ of those [common neighbours](../../../../../common-neighbour.md) form the last class. None of the [common neighbours](../../../../../common-neighbour.md) belongs to a selected [clique](../../../../../clique-graph-theory.md), because that would require a loop. This proves the [logarithmic clique blow-up from minimum degree](../../../../../logarithmic-clique-blow-up-from-minimum-degree.md) assertion.

To pass from an [edge](../../../../../edge-of-a-graph.md) count to [minimum degree](../../../../../minimum-degree-of-a-graph.md), put $b=1-1/r+\varepsilon$ and $a=b-\varepsilon/2$. Repeatedly remove a [vertex](../../../../../vertex-graph-theory.md) whose current [degree of a vertex](../../../../../degree-graph-theory.md) is below $a$ times the current order. If the process reaches order $m$, its deleted [edges](../../../../../edge-of-a-graph.md) and remaining [edges](../../../../../edge-of-a-graph.md) give

$$
b\binom n2\le e(G)\le a\sum_{j=m+1}^n j+\binom m2
=\frac a2(n^2+n-m^2-m)+\frac12(m^2-m).
$$

Thus $(1-a)m^2\ge (\varepsilon/2)n^2-O(n)$. In particular, for a fixed sufficiently small $\gamma>0$, the process cannot reach $m=\lfloor\gamma n\rfloor$: the displayed inequality would fail. It stops earlier with a subgraph of order $N\ge\gamma n$ and [minimum degree](../../../../../minimum-degree-of-a-graph.md) at least $(1-1/r+\varepsilon/2)N$. The [induction](../../../../../mathematical-induction.md) just proved supplies $K_{r+1}(\lfloor c\log N\rfloor)$, hence a lower bound $c'\log n$ on $t(r,\varepsilon,n)$. In particular, **the guaranteed part size tends to infinity**.

For the upper bound, choose a fixed $p$ with $b<p<1$ and take a [binomial random graph](../../../../../binomial-random-graph.md) $G(n,p)$. Its [edge](../../../../../edge-of-a-graph.md) count has [expectation](../../../../../expected-value.md) $p\binom n2$ and [variance](../../../../../variance-split.md) $p(1-p)\binom n2$. The [Chebyshev inequality](../../../../../chebyshev-inequality.md) shows that $e(G)\ge b\binom n2$ with [probability](../../../../../probability.md) tending to one. The expected number of labeled copies of $K_{r+1}(t)$ is at most

$$
n^{(r+1)t}p^{\binom{r+1}2t^2}.
$$

For $t=\lceil C\log n\rceil$ and $C>2/[r\log(1/p)]$, this tends to zero. The [Markov inequality](../../../../../markov-inequality.md) therefore shows that with positive [probability](../../../../../probability.md) both the required [edge](../../../../../edge-of-a-graph.md) density holds and there is no such copy. This proves $t(r,\varepsilon,n)=O(\log n)$ and completes the [random obstruction to larger clique blow-ups](../../../../../random-obstruction-to-larger-clique-blow-ups.md) argument.

There is a necessary qualification to the density parameter. If $\varepsilon=1/r$, the only eligible [graph](../../../../../graph-split.md) is the [complete graph](../../../../../complete-graph.md), and **$t(r,1/r,n)=\lfloor n/(r+1)\rfloor$**. If $\varepsilon>1/r$ and $n\ge2$, there are no eligible simple [graphs](../../../../../graph-split.md); the universal assertion is vacuous for every $t$, so the printed maximum has no finite value in that range.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
