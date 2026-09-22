<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $K_j(t)$ for a [balanced complete multipartite blow-up](../../../../../balanced-complete-multipartite-blow-up.md), with $j$ parts each containing $t$ [vertices](../../../../../vertex-graph-theory.md). Its occurrence is a [subgraph](../../../../../subgraph.md) condition, so additional internal [edges](../../../../../edge-of-a-graph.md) in the host are harmless. The coefficient multiplying $\log n$ is essential: the PDF has $t=\lfloor d\log n\rfloor$, although it is lost in the converted TeX.

First prove the [common neighbourhood from bipartite density](../../../../../common-neighbourhood-from-bipartite-density.md) estimate. Suppose a [bipartite graph](../../../../../bipartite-graph.md) has parts of sizes $m,N$ and at least $\beta mN$ [edges](../../../../../edge-of-a-graph.md). For an integer $s\le\beta m/2$, count incidences between $s$-subsets of the first part and their [common neighbours](../../../../../common-neighbour.md) in the second. The discrete [convexity](../../../../../convex-function.md) of $k\mapsto\binom ks$, with value zero for $k<s$, gives

$$
\max_{|S|=s}|N(S)|\binom ms\ge\sum_{v}\binom{\deg(v)}s\ge N\binom{\lfloor\beta m\rfloor}s.
$$

The [convexity](../../../../../convex-function.md) assertion follows directly from $\binom{k+1}s-\binom ks=\binom{k}{s-1}$, which is increasing in $k$; smoothing two unequal degrees cannot increase the sum. In the binomial ratio every factor is at least $\beta/2$, because $\lfloor\beta m\rfloor-s+1\ge\beta m-s\ge\beta m/2$. Consequently some $S$ satisfies

$$
|N(S)|\ge N(\beta/2)^s.
$$

We prove the [logarithmic clique blow-up from minimum degree](../../../../../logarithmic-clique-blow-up-from-minimum-degree.md) by induction on $r$. When $\varepsilon\ge1/r$, the degree hypothesis is impossible for a loopless [graph](../../../../../graph-split.md), so any positive $d$ works vacuously. Assume $0<\varepsilon<1/r$. For $r=1$, take two copies of the [vertex set](../../../../../vertex-set.md) and join the copies of adjacent [vertices](../../../../../vertex-graph-theory.md). This [bipartite graph](../../../../../bipartite-graph.md) has [edge density of a bipartite graph](../../../../../edge-density-of-a-bipartite-graph.md) at least $\varepsilon$. Choose

$$
d(1,\varepsilon)\le\frac1{2\log(2/\varepsilon)}.
$$

For sufficiently large $n$, $t=\lfloor d\log n\rfloor\le\varepsilon n/2$, and the estimate supplies at least $\sqrt n$ [common neighbours](../../../../../common-neighbour.md). Choose $t$ of them. The two selected sets are disjoint in the original [graph](../../../../../graph-split.md), since a selected vertex cannot be adjacent to itself. They give $K_2(t)$.

For $r\ge2$, put $\varepsilon'=\varepsilon+1/(r-1)-1/r$. The same [minimum degree of a graph](../../../../../minimum-degree-of-a-graph.md) exceeds $(1-1/(r-1)+\varepsilon')n$. By induction there is a $K_r(m)$ with $m=\lfloor d'\log n\rfloor$, where $d'=d(r-1,\varepsilon')>0$. Pair the [vertices](../../../../../vertex-graph-theory.md) of its $r$ parts into $m$ disjoint transversal [cliques](../../../../../clique-graph-theory.md) $C_1,\ldots,C_m$. Each has at least

$$
n-r(n-\delta(G))\ge r\varepsilon n
$$

[common neighbours](../../../../../common-neighbour.md), by bounding the union of the non-neighbour sets of its $r$ [vertices](../../../../../vertex-graph-theory.md). Set $\beta=\min\{r\varepsilon,1/2\}$. Form the [bipartite graph](../../../../../bipartite-graph.md) whose first part is these $m$ [cliques](../../../../../clique-graph-theory.md), with $C_i$ joined to a vertex when that vertex is a [common neighbour](../../../../../common-neighbour.md) of all of $C_i$. It has density at least $\beta$. Choose

$$
0<d\le\min\left\{\frac{\beta d'}4,\frac1{2\log(2/\beta)}\right\}.
$$

For large $n$, $m\ge d'\log n/2$ and $t=\lfloor d\log n\rfloor\le\beta m/2$. The estimate gives $t$ selected [cliques](../../../../../clique-graph-theory.md) and at least $\sqrt n\ge t$ common [vertices](../../../../../vertex-graph-theory.md). The selected [cliques](../../../../../clique-graph-theory.md) supply $t$ [vertices](../../../../../vertex-graph-theory.md) in each of the original $r$ parts, and their common [vertices](../../../../../vertex-graph-theory.md) supply the final part. No common vertex belongs to a selected [clique](../../../../../clique-graph-theory.md), again because there are no loops. All required cross-part [edges](../../../../../edge-of-a-graph.md) are present. Increasing $n_0(r,\varepsilon)$ to satisfy these finitely many inequalities completes the induction:

$$
\boxed{K_{r+1}(\lfloor d(r,\varepsilon)\log n\rfloor)\subseteq G.}
$$

The [Erdős-Stone theorem](../../../../../erdos-stone-theorem.md) states that for a fixed [graph](../../../../../graph-split.md) $H$ with [chromatic number](../../../../../chromatic-number.md) $r+1\ge2$,

$$
\boxed{\operatorname{ex}(n,H)=\left(1-\frac1r+o(1)\right)\binom n2.}
$$

The lower bound comes from the [Turán graph](../../../../../turan-graph.md) $T_r(n)$, which cannot contain an $(r+1)$-chromatic [subgraph](../../../../../subgraph.md). To obtain the upper bound from our minimum-degree result, suppose $e(G)\ge(a+\eta)n^2/2$, where $a=1-1/r$ and $0<\eta<1-a$. Repeatedly delete a vertex of degree less than $b$ times the current order, where $b=a+\eta/2$, until no such vertex remains. If the remaining order is $m$, then

$$
e(G)\le\frac b2(n^2-m^2+n)+\frac{m^2}2,
\qquad
(1-b)m^2\ge\frac\eta2n^2-bn.
$$

Thus $m\ge c_\eta n$ for large $n$, with $c_\eta>0$, and the remaining [subgraph](../../../../../subgraph.md) has [minimum degree of a graph](../../../../../minimum-degree-of-a-graph.md) at least $(a+\eta/2)m$. It contains $K_{r+1}(\lfloor d\log m\rfloor)$. A proper [graph colouring](../../../../../graph-coloring.md) of $H$ places its [vertices](../../../../../vertex-graph-theory.md) in the $r+1$ parts once their size exceeds $|V(H)|$. This contradicts $H$-freeness. Adjusting a fixed positive density margin absorbs the difference between $n^2/2$ and $\binom n2$, proving the upper bound.

The six-vertex forbidden [graph](../../../../../graph-split.md) is the [octahedral graph](../../../../../octahedral-graph.md) $K_{2,2,2}$: the deleted [matching in a graph](../../../../../matching-graph-theory.md) gives its three independent pairs. Its [chromatic number](../../../../../chromatic-number.md) is three, so

$$
\boxed{\lim_{n\to\infty}\frac{\operatorname{ex}(n,F)}{\binom n2}=\frac12.}
$$

The printed notation uses $H$ for the extremal-number argument while its defining condition forbids $F$; the answer uses that explicitly defined forbidden [graph](../../../../../graph-split.md). For the strict finite inequality, take $T_2(n)$ and add one [edge](../../../../../edge-of-a-graph.md) inside its larger part, which has at least two [vertices](../../../../../vertex-graph-theory.md) for $n\ge3$. Every [triangle in a graph](../../../../../triangle-in-a-graph.md) then uses this added edge. However, $K_{2,2,2}$ contains two vertex-disjoint [triangles in a graph](../../../../../triangle-in-a-graph.md), obtained by taking one vertex from each pair and then the other three. It therefore cannot occur in the constructed [graph](../../../../../graph-split.md). Hence

$$
\boxed{\operatorname{ex}(n,F)\ge t_2(n)+1>t_2(n)\qquad(n\ge3).}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
