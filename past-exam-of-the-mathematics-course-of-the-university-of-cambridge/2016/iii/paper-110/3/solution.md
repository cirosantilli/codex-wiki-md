<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Think of a vertex of this [hypergraph](../../../../../hypergraph-split.md) as an edge of the complete [graph](../../../../../graph-split.md) on $[N]$. A hyperedge is the edge set of one $t$-vertex [clique](../../../../../clique-graph-theory.md). A fixed pair belongs to a [clique](../../../../../clique-graph-theory.md) precisely when its other $t-2$ vertices are chosen from the remaining $N-2$, giving

$$
\boxed{d=\binom{N-2}{t-2}.}
$$

For a set $\sigma$ of [graph](../../../../../graph-split.md) edges, let $v$ be the number of their distinct endpoints. If $v>t$, no $t$-[clique](../../../../../clique-graph-theory.md) contains them and the [codegree](../../../../../hypergraph-codegree.md) is zero. Otherwise its other $t-v$ vertices may be chosen freely, so

$$
\boxed{d(\sigma)=\binom{N-v}{t-v}.}
$$

For $2\le k=|\sigma|\le\binom t2$, distinct edges have at least three endpoints, and all $k$ edges lie among the $\binom v2$ possible pairs. Thus $3\le v\le t$ and $k\le\binom v2$. In particular,

$$
2(k-1)\le v(v-1)-2=(v-2)(v+1)\le(v-2)(t+1).
$$

This also identifies why the relevant exponent is $2/(t+1)$.

For fixed $t$ and $3\le v\le t$, the ratio of the two [binomial coefficients](../../../../../binomial-coefficient.md) satisfies $d(\sigma)/d\le A_tN^{-(v-2)}$ for all sufficiently large $N$, with one constant $A_t$ valid for every $v$. For $\tau=c'N^{-2/(t+1)}$,

$$
\frac{d(\sigma)}{d\tau^{k-1}}
\le\frac{A_t}{(c')^{k-1}}N^{-(v-2)+2(k-1)/(t+1)}
\le\frac{A_t}{(c')^{k-1}}.
$$

For any fixed $c>0$, choose $c'\ge1$ so large that the last bound is at most $c$ for every $2\le k\le\binom t2$. Zero [codegrees](../../../../../hypergraph-codegree.md) satisfy the bound automatically. **The asserted small-codegree condition therefore holds uniformly.** Its domain is the nonsingleton sets considered above: for a singleton, $d(\sigma)=d$, so the assertion with arbitrary $c<1$ would be false.

A family of [hypergraph containers](../../../../../hypergraph-container.md) is a collection $\mathcal C$ of vertex subsets such that every [hypergraph independent set](../../../../../hypergraph-independent-set.md) of the [hypergraph](../../../../../hypergraph-split.md) is contained in some $C\in\mathcal C$. Here a [hypergraph independent set](../../../../../hypergraph-independent-set.md) is exactly the edge set of a $K_t$-free [graph](../../../../../graph-split.md) on $[N]$.

We use the following edge-sparse form of the [hypergraph container theorem](../../../../../hypergraph-container-theorem.md). For fixed uniformity $R\ge2$ and $\varepsilon>0$, there are constants $b,K>0$ such that an $R$-uniform [hypergraph](../../../../../hypergraph-split.md) on $m$ vertices with positive average [hypergraph vertex degree](../../../../../hypergraph-vertex-degree.md) $d$, $0<\tau$ sufficiently small, and

$$
d(\sigma)\le b d\tau^{|\sigma|-1}\quad(2\le|\sigma|\le R)
$$

has a family $\mathcal C$ covering its [hypergraph independent sets](../../../../../hypergraph-independent-set.md) with

$$
e(G[C])\le\varepsilon e(G)\quad(C\in\mathcal C),\qquad
\log_2|\mathcal C|\le K m\tau\log(1/\tau).
$$

One obtains this form by iterating a degree-measure [hypergraph container theorem](../../../../../hypergraph-container-theorem.md), recording small [container fingerprints](../../../../../container-fingerprint.md) at each step. To ensure the requested strict edge inequality, apply it with $\varepsilon/2$.

For our [clique](../../../../../clique-graph-theory.md) [hypergraph](../../../../../hypergraph-split.md), $m=\binom N2$, $R=\binom t2$ and $e(G)=\binom Nt$. The established [codegree](../../../../../hypergraph-codegree.md) bound permits this choice of $\tau$, and

$$
\log_2|\mathcal C|=O\left(N^{2-2/(t+1)}\log N\right)=o(N^2).
$$

Every container, viewed as an ordinary [graph](../../../../../graph-split.md), has at most $\varepsilon\binom Nt$ copies of $K_t$.

We also use [clique](../../../../../clique-graph-theory.md) [supersaturation](../../../../../supersaturation.md): for each fixed $\gamma>0$, [graphs](../../../../../graph-split.md) with at least $(1-1/(t-1)+\gamma)\binom N2$ edges have at least $b_\gamma N^t$ copies of $K_t$, for some $b_\gamma>0$ and all sufficiently large $N$. For clarity, this follows already from the [Erdős-Stone theorem](../../../../../erdos-stone-theorem.md): choose a fixed sample size $q$ with $\operatorname{ex}(q,K_t)\le(1-1/(t-1)+\gamma/2)\binom q2$. A uniformly sampled $q$-set has [expected value](../../../../../expected-value.md) of the edge count above this bound by at least $(\gamma/2)\binom q2$, forcing a positive proportion of samples to contain a [clique](../../../../../clique-graph-theory.md). Counting each [clique](../../../../../clique-graph-theory.md)'s extensions to $q$-sets then gives the claimed $b_\gamma N^t$ bound.

Choose $\varepsilon$ smaller than the corresponding supersaturation constant after converting $\binom Nt$ to $N^t$. Each container has fewer than $(1-1/(t-1)+\gamma)\binom N2$ ordinary edges. Every $K_t$-free [graph](../../../../../graph-split.md) is a subgraph of one of these containers, so their number is at most

$$
|\mathcal C|\,2^{(1-1/(t-1)+\gamma)\binom N2}.
$$

Conversely, every subgraph of a balanced [Turán graph](../../../../../turan-graph.md) with $t-1$ parts is $K_t$-free, giving at least $2^{(1-1/(t-1))\binom N2-O(N)}$ possibilities. Letting $\gamma$ be arbitrarily small proves **the enumeration formula**:

$$
\boxed{\#\{K_t\text{-free graphs on }[N]\}=2^{(1-1/(t-1)+o(1))\binom N2}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 110](../../paper-110-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
