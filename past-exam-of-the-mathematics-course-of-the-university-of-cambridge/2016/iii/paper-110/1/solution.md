<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Erdős-Stone theorem](../../../../../erdos-stone-theorem.md) says that, for a fixed [graph](../../../../../graph-split.md) $F$ with [chromatic number](../../../../../chromatic-number.md) $q\ge2$,

$$
\boxed{\operatorname{ex}(n,F)=\left(1-\frac1{q-1}+o(1)\right)\binom n2.}
$$

The lower bound comes from the balanced [Turán graph](../../../../../turan-graph.md) with $q-1$ parts; the theorem supplies the matching asymptotic upper bound. Here and below, all forbidden [graphs](../../../../../graph-split.md) and blow-up parameters are fixed as $n\to\infty$.

**First obtain an almost spanning, almost complete multipartite core.** Put $\alpha_r=1-1/r$. We give the stability argument, rather than infer pointwise degree bounds by differentiating an asymptotic edge-count formula. Suppose first $r\ge2$.

We need two elementary ingredients. First, positive [homomorphism density](../../../../../homomorphism-density.md) of $K_{r+1}$ forces a fixed [complete multipartite graph](../../../../../complete-multipartite-graph.md) $K_{r+1}(t)$. To see this, perform [vertex cloning in a graph](../../../../../vertex-cloning-in-a-graph.md), replacing one vertex by $t$ independent twins. Conditional on the images of the other vertices, its contribution to the [homomorphism density](../../../../../homomorphism-density.md) changes from a number $p$ to $p^t$; [Jensen inequality](../../../../../jensen-s-inequality.md) gives $\mathbb E p^t\ge(\mathbb E p)^t$. Duplicating each original vertex therefore gives

$$
t(K_{r+1}(t),G)\ge t(K_{r+1},G)^{\,t^{r+1}}.
$$

A positive lower bound on the right supplies a positive proportion of all maps of the blow-up. Only $O(n^{(r+1)t-1})$ maps fail to be injective, so for large $n$ at least one map is an embedding. Consequently a $K_{r+1}(t)$-free sequence has $o(n^{r+1})$ copies of $K_{r+1}$. The [clique removal lemma](../../../../../clique-removal-lemma.md), proved in the next solution, then deletes $o(n^2)$ edges to give a $K_{r+1}$-free [graph](../../../../../graph-split.md) $J_n$ with $e(J_n)=\alpha_r n^2/2-o(n^2)$.

Second, we prove the required stability for $K_{r+1}$-free [graphs](../../../../../graph-split.md) by induction on $r$. For $r=1$ such a [graph](../../../../../graph-split.md) is edgeless. In an $m$-vertex $K_{r+1}$-free [graph](../../../../../graph-split.md) $J$, take a vertex of maximum [vertex degree](../../../../../degree-graph-theory.md) $D$, put $A=N(v)$ and $B=V(J)\setminus A$, and note that $J[A]$ is $K_r$-free. The [Turan theorem](../../../../../turan-s-theorem.md) and the maximum-degree bound give

$$
\begin{aligned}
e(J)&=e(J[A])+\sum_{u\in B}d(u)-e(J[B])\\
&\le\frac{r-2}{2(r-1)}D^2+(m-D)D-e(J[B])\\
&=\frac{r-1}{2r}m^2-\frac{r}{2(r-1)}\left(D-\frac{r-1}{r}m\right)^2-e(J[B]).
\end{aligned}
$$

If $e(J)=\alpha_r m^2/2-o(m^2)$, both nonnegative error terms are $o(m^2)$: $D=\alpha_r m+o(m)$ and $e(J[B])=o(m^2)$. The deficit in the bound for $e(J[A])$ is likewise $o(m^2)$. Induction partitions $A$ into $r-1$ classes with a total of $o(m^2)$ internal edges; adjoining $B$ gives an $r$-class partition with the same property. Applying this to $J_n$ and restoring the removed edges gives such a partition $V_1,\ldots,V_r$ of $G_n$.

The number of possible crossing edges is $\tfrac12(n^2-\sum_i|V_i|^2)\le\alpha_r n^2/2$. Since the actual crossing-edge count is within $o(n^2)$ of this maximum, $|V_i|=n/r+o(n)$ for every $i$, and there are $o(n^2)$ missing crossing edges. Choose $a_n\to0$ so slowly that the number of vertices missing more than $a_n n$ neighbours in other classes is $o(n)$. Delete those vertices and all internal edges. The remaining [r-partite graph](../../../../../multipartite-graph.md) $Q_n$ has $n-o(n)$ vertices and every vertex has crossing [vertex degree](../../../../../degree-graph-theory.md) at least $\alpha_r n-o(n)$. The [Turan theorem](../../../../../turan-s-theorem.md), or the size of a largest part, supplies the matching upper bound for its minimum [vertex degree](../../../../../degree-graph-theory.md). Thus

$$
\boxed{\delta(Q_n)=\left(1-\frac1r+o(1)\right)n.}
$$

This is a [high-minimum-degree multipartite stability subgraph](../../../../../high-minimum-degree-multipartite-stability-subgraph.md). The subgraph need not be spanning; deleting the exceptional $o(n)$ vertices is essential. For $r=1$, the spanning edgeless subgraph already proves the assertion.

**Extremality forces the minimum degree.** Choose $t\ge|V(F)|$. A proper $(r+1)$-[graph colouring](../../../../../graph-coloring.md) embeds $F$ in $K_{r+1}(t)$, so every $F$-free $H_n$ is also $K_{r+1}(t)$-free. By the [Erdős-Stone theorem](../../../../../erdos-stone-theorem.md), its extremal edge count has the needed asymptotic size. The preceding proof supplies core classes $W_1,\ldots,W_r$ of size $n/r+o(n)$ in which every vertex misses only $o(n)$ crossing neighbours, uniformly over the core.

Delete an arbitrary vertex $x$ from $H_n$ and introduce a new vertex $z$ adjacent precisely to $W_2\cup\cdots\cup W_r$ with $x$ removed if necessary. The new [graph](../../../../../graph-split.md) is still $F$-free. Indeed any new copy would use $z$, all its neighbours in that copy would be in the specified core classes, and their set of [common neighbours](../../../../../common-neighbour.md) in $W_1$ has size $n/r-o(n)$. A vertex of this common neighbourhood outside the bounded vertex set of the copy replaces $z$, producing an existing copy of $F$ in $H_n$, a contradiction. For $r=1$ the new vertex is isolated and the same conclusion is immediate.

The replacement adds $\alpha_r n-o(n)$ edges. Since $H_n$ has the maximum possible number of edges, $d_{H_n}(x)\ge\alpha_r n-o(n)$. As $x$ was arbitrary and the minimum [vertex degree](../../../../../degree-graph-theory.md) is at most the average [vertex degree](../../../../../degree-graph-theory.md),

$$
\boxed{\delta(H_n)=\left(1-\frac1r+o(1)\right)n.}
$$

This proves the [minimum degree of an extremal forbidden-subgraph graph](../../../../../minimum-degree-of-an-extremal-forbidden-subgraph-graph.md). The replacement argument avoids the invalid implication $\operatorname{ex}(n,F)-\operatorname{ex}(n-1,F)=\alpha_r n+o(n)$ based solely on the asymptotic formula.

**A [colour-critical vertex](../../../../../colour-critical-vertex.md) also bounds the maximum degree.** Suppose a vertex $x$ of $H_n$ has $d(x)\ge\alpha_r n+\varepsilon n$ for some fixed $\varepsilon>0$. Since the core omits only $o(n)$ vertices and all its classes have size $n/r+o(n)$, $x$ has at least $\varepsilon n-o(n)$ neighbours in each $W_i$. Otherwise, even counting every vertex in all other classes and outside the core would give too small a [vertex degree](../../../../../degree-graph-theory.md).

Inside these $r$ neighbourhood sets, greedily choose a fixed number $t\ge|V(F)|$ of vertices in each class. Every previously chosen vertex excludes only $o(n)$ crossing nonneighbours, so each next candidate set still has positive linear size. This produces $K_r(t)$ inside $N(x)$. A proper $r$-[graph colouring](../../../../../graph-coloring.md) of $F-v$ embeds it in that [complete multipartite graph](../../../../../complete-multipartite-graph.md); map $v$ to $x$. All required incident edges exist, so this embeds $F$, a contradiction. The case $r=1$ simply uses enough neighbours to embed the edgeless $F-v$. Hence $\Delta(H_n)\le\alpha_r n+o(n)$, and the average-degree lower bound completes the answer:

$$
\boxed{\Delta(H_n)=\left(1-\frac1r+o(1)\right)n.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 110](../../paper-110-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
