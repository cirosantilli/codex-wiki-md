<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Burton-Keane theorem](../../../../../uniqueness-of-the-infinite-percolation-cluster.md) says that for independent [bond percolation](../../../../../bond-percolation-split.md) on the [hypercubic lattice](../../../../../cubic-lattice.md) $\mathbb Z^d$, $d\ge2$, at every fixed $p\in[0,1]$, there is almost surely **at most one [infinite percolation cluster](../../../../../infinite-percolation-cluster.md)**. It does not assert that such a cluster exists, nor does it assert absence of percolation at the critical parameter. The cases $p=0$ and $p=1$ are immediate; assume $0<p<1$ for the proof.

Let $N_\infty$ be the number of [infinite percolation clusters](../../../../../infinite-percolation-cluster.md). This [random variable](../../../../../random-variable-split.md) is translation invariant. By [translation ergodicity of Bernoulli percolation](../../../../../translation-ergodicity-of-bernoulli-percolation.md), it is almost surely a constant $k\in\{0,1,2,\ldots,\infty\}$. One way to see ergodicity is to approximate an invariant event by events on finite sets of [edges](../../../../../edge-of-a-graph.md), translate one approximation far enough to make the two approximations independent, and then let the approximation error vanish. Its [probability](../../../../../probability.md) equals its square, hence is zero or one.

The other probabilistic input is the [finite-energy property of Bernoulli percolation](../../../../../finite-energy-property-of-bernoulli-percolation.md). Conditionally on all [edges](../../../../../edge-of-a-graph.md) outside a finite set, every prescribed inside configuration has positive [probability](../../../../../probability.md), namely a product of powers of $p$ and $1-p$. Thus an event of positive [probability](../../../../../probability.md) can be followed by a specified finite modification and still gives a positive-probability image event. Outside infinite arms are unaffected.

First exclude a finite $k\ge2$. Some finite box meets at least two [infinite percolation clusters](../../../../../infinite-percolation-cluster.md) with positive [probability](../../../../../probability.md). Open all [edges](../../../../../edge-of-a-graph.md) in and incident to that box. These clusters merge. Opening finitely many [edges](../../../../../edge-of-a-graph.md) cannot create an [infinite percolation cluster](../../../../../infinite-percolation-cluster.md) solely out of finite clusters, since it joins only finitely many such clusters. Hence the number of [infinite percolation clusters](../../../../../infinite-percolation-cluster.md) decreases with positive [probability](../../../../../probability.md), contradicting its almost-sure constant value. This rules out every finite multiplicity greater than one.

Now suppose $k=\infty$. With positive [probability](../../../../../probability.md) a finite box meets at least three distinct [infinite percolation clusters](../../../../../infinite-percolation-cluster.md). Retain an exterior infinite ray from each of three of them. Replace the finitely many interior and boundary [edges](../../../../../edge-of-a-graph.md) by a minimal [tree](../../../../../tree-graph-theory.md) joining their three attachment [graph vertices](../../../../../vertex-graph-theory.md), and close all unused [edges](../../../../../edge-of-a-graph.md) there. The exterior rays belong to distinct original clusters, so have no outside connections to each other. The resulting joined cluster has a branch [graph vertex](../../../../../vertex-graph-theory.md) $v$ with exactly three incident open [edges](../../../../../edge-of-a-graph.md), and deleting $v$ leaves three infinite components. If a terminal lies in the middle of the interior connecting path, its exterior ray supplies the third branch there. Such a [graph vertex](../../../../../vertex-graph-theory.md) is a [trifurcation vertex in percolation](../../../../../trifurcation-vertex-in-percolation.md). A finite box has only finitely many candidate locations and modifications; therefore some fixed [graph vertex](../../../../../vertex-graph-theory.md) has positive trifurcation [probability](../../../../../probability.md). By translation invariance, that [probability](../../../../../probability.md) is a common number $\tau>0$ at every [graph vertex](../../../../../vertex-graph-theory.md).

The decisive deterministic input is the [trifurcation boundary-counting lemma](../../../../../trifurcation-boundary-counting-lemma.md). Let $T$ be all these degree-three [trifurcation vertices in percolation](../../../../../trifurcation-vertex-in-percolation.md) in a finite box $B_n$. In each [infinite percolation cluster](../../../../../infinite-percolation-cluster.md) meeting $T$, delete the [graph vertices](../../../../../vertex-graph-theory.md) of $T$, contract each remaining [connected component of a graph](../../../../../component-graph-theory.md) adjacent to $T$ to a node, and retain the incidences with the deleted [graph vertices](../../../../../vertex-graph-theory.md), including direct [edges](../../../../../edge-of-a-graph.md) between [graph vertices](../../../../../vertex-graph-theory.md) of $T$. This is a finite [tree](../../../../../tree-graph-theory.md): a cycle would connect two neighbours of an original [trifurcation vertex in percolation](../../../../../trifurcation-vertex-in-percolation.md) without passing through it, contradicting its three-way separation. Every deleted [graph vertex](../../../../../vertex-graph-theory.md) has degree three. Every leaf component is infinite, since a finite leaf would give a finite branch after removing its adjacent [trifurcation vertex in percolation](../../../../../trifurcation-vertex-in-percolation.md). The elementary [tree](../../../../../tree-graph-theory.md) degree identity therefore supplies at least $|T\cap C|+2$ infinite leaf components for a cluster containing $T$.

Each such infinite component reaches the outer [graph vertex](../../../../../vertex-graph-theory.md) boundary $\partial^+B_n$, and different components reach different boundary [graph vertices](../../../../../vertex-graph-theory.md). Summing over the clusters yields, in particular,

$$
|T|\le|\partial^+B_n|.
$$

For a nearest-neighbour lattice box,

$$
|B_n|=(2n+1)^d,\qquad
|\partial^+B_n|=2d(2n+1)^{d-1}.
$$

Taking expectations and using the common trifurcation [probability](../../../../../probability.md) gives

$$
\tau(2n+1)^d\le2d(2n+1)^{d-1},\qquad
\tau\le\frac{2d}{2n+1}\longrightarrow0.
$$

This contradicts $\tau>0$ and excludes infinitely many [infinite percolation clusters](../../../../../infinite-percolation-cluster.md). Thus only $k=0$ or $k=1$ remains:

$$
\boxed{\mathbb P_p(N_\infty\in\{0,1\})=1\quad\text{for every }p\in[0,1].}
$$

The proof explains the role of the [amenable boundary growth of lattice boxes](../../../../../amenable-boundary-growth-of-lattice-boxes.md): [finite-energy property of Bernoulli percolation](../../../../../finite-energy-property-of-bernoulli-percolation.md) would make branching points have positive volume density, while their disjoint infinite branches can only be supplied through a boundary of lower order. It uses no planar duality and works in every indicated dimension.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
