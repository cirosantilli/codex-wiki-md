# Bond percolation

↑ **Parent:** [Percolation theory](probability-theory.md#percolation-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bond_percolation)

In bond percolation with parameter $p$, every edge of a graph is independently open with probability $p$ and closed with probability $1-p$.

**Table of contents**

- [Rectangle crossing in bond percolation](#rectangle-crossing-in-bond-percolation)
  - [Finite-torus crossing amplification](#finite-torus-crossing-amplification)
- [Open path in bond percolation](#open-path-in-bond-percolation)
- [Uniform random orientation out-cluster comparison](#uniform-random-orientation-out-cluster-comparison)
- [Percolation triangle condition](#percolation-triangle-condition)
- [Percolation two-point connection probability](#percolation-two-point-connection-probability)
  - [Reflection lower bound for two-point percolation](#reflection-lower-bound-for-two-point-percolation)
- [Connection decay rate in a percolation strip](#connection-decay-rate-in-a-percolation-strip)
  - [Strip approximation to the planar connection decay rate](#strip-approximation-to-the-planar-connection-decay-rate)
  - [Closed-cut bound for percolation in a strip](#closed-cut-bound-for-percolation-in-a-strip)
- [Translation ergodicity of Bernoulli percolation](#translation-ergodicity-of-bernoulli-percolation)
- [Percolation cluster](#percolation-cluster)
  - [Maximum cluster radius under exponential one-arm decay](#maximum-cluster-radius-under-exponential-one-arm-decay)
  - [Infinite percolation cluster](#infinite-percolation-cluster)
  - [Uniqueness of the infinite percolation cluster](#uniqueness-of-the-infinite-percolation-cluster)
    - [Percolation uniqueness on an amenable quasi-transitive graph](#percolation-uniqueness-on-an-amenable-quasi-transitive-graph)
    - [Boundary counting proof of percolation uniqueness](#boundary-counting-proof-of-percolation-uniqueness)
      - [Encounter box in percolation](#encounter-box-in-percolation)
    - [Trifurcation vertex in percolation](#trifurcation-vertex-in-percolation)
      - [Trifurcation boundary-counting lemma](#trifurcation-boundary-counting-lemma)
        - [Forest proof of trifurcation boundary counting](#forest-proof-of-trifurcation-boundary-counting)
- [Percolation susceptibility](#percolation-susceptibility)
  - [Tree-graph moment bound for a percolation cluster](#tree-graph-moment-bound-for-a-percolation-cluster)
  - [Exponential one-arm decay from finite susceptibility](#exponential-one-arm-decay-from-finite-susceptibility)
- [Russo-Seymour-Welsh theorem](#russo-seymour-welsh-theorem)
  - [Uniform RSW crossing estimate](#uniform-rsw-crossing-estimate)
  - [RSW reflection extension lemma](#rsw-reflection-extension-lemma)
    - [Reflected attachment estimate for percolation](#reflected-attachment-estimate-for-percolation)
  - [One-arm probability](#one-arm-probability)
    - [Weighted BK boundary-splitting estimate](#weighted-bk-boundary-splitting-estimate)
    - [Polynomial critical one-arm upper bound](#polynomial-critical-one-arm-upper-bound)
    - [Independent annular barriers for percolation](#independent-annular-barriers-for-percolation)
    - [BK boundary-splitting estimate](#bk-boundary-splitting-estimate)
    - [Percolation one-arm decay rate](#percolation-one-arm-decay-rate)
      - [Almost-subadditive percolation decay rate](#almost-subadditive-percolation-decay-rate)
    - [One-arm extension estimate](#one-arm-extension-estimate)
      - [RSW gluing lemma for two one-arm events](#rsw-gluing-lemma-for-two-one-arm-events)
- [Van den Berg-Kesten inequality](#van-den-berg-kesten-inequality)
  - [Coordinate-splitting proof of the BK inequality](#coordinate-splitting-proof-of-the-bk-inequality)
  - [Square-lattice one-arm lower bound from disjoint occurrence](#square-lattice-one-arm-lower-bound-from-disjoint-occurrence)
  - [Disjoint occurrence of increasing events](#disjoint-occurrence-of-increasing-events)

## Rectangle crossing in bond percolation

↑ **Parent:** [Bond percolation](bond-percolation.md)

For the induced [square lattice](graph.md#square-lattice) subgraph in $[0,m]\times[0,n]$, $h_p(m,n)$ is the [probability](probability-theory.md#probability) of an open [graph path](graph-theory.md#path-in-a-graph) from its left boundary to its right boundary under independent [bond percolation](bond-percolation.md) of density $p$. Width and height count lattice spacings. [Dual bond percolation](graph-theory.md#dual-bond-percolation) exchanges failure with a top-to-bottom dual crossing of dimensions $(m-1)\times(n+1)$, with the usual exterior boundary vertices.

### Finite-torus crossing amplification

↑ **Parent:** [Rectangle crossing in bond percolation](#rectangle-crossing-in-bond-percolation)

Take the increasing event that a finite square [torus graph](graph.md#torus-graph) contains some long horizontal or vertical rectangle crossing. Translations and a quarter turn make this a [transitive increasing event](probability-inequality.md#transitive-increasing-event) on its bonds. A positive critical crossing bound and the [Friedgut-Kalai sharp threshold theorem](combinatorics.md#friedgut-kalai-sharp-threshold-theorem) make its supercritical probability tend to one. A bounded family of shorter, thicker rectangles intercepts every possible long crossing. The [square-root trick for positively associated events](probability-inequality.md#square-root-trick-for-positively-associated-events) transfers the high probability to each fixed intercepting rectangle. Using every possible translate would lose the useful bounded exponent.

## Open path in bond percolation

↑ **Parent:** [Bond percolation](bond-percolation.md)

A path in the underlying graph all of whose [edges](graph-theory.md#edge-of-a-graph) are open. Connectivity of [open paths](#open-path-in-bond-percolation) determines the [percolation clusters](#percolation-cluster). A [ray in a graph](graph-theory.md#ray-in-a-graph) with all [edges](graph-theory.md#edge-of-a-graph) open is an infinite [ray in a graph](graph-theory.md#ray-in-a-graph).

## Uniform random orientation out-cluster comparison

↑ **Parent:** [Bond percolation](bond-percolation.md)

If independent [edges](graph-theory.md#edge-of-a-graph) of a [locally finite graph](graph-theory.md#locally-finite-graph) receive fair orientations, exploring outward from a root tests each fresh reached-to-unreached boundary [edge](graph-theory.md#edge-of-a-graph) with success [probability](probability-theory.md#probability) $1/2$. Deferred decisions give exactly the exploration law of the root cluster in [bond percolation](bond-percolation.md) of density $1/2$. Thus the two reachable [graph vertex](graph.md#vertex-graph-theory) sets have the same distribution. An infinite out-cluster contains an infinite simple directed ray by the [König infinity lemma](combinatorics.md#konig-s-lemma). Geometrically biased orientations do not generally give the same uniform edge-success law.

## Percolation triangle condition

↑ **Parent:** [Bond percolation](bond-percolation.md)

Here $\tau(x,y)=P_{p_c}(x\leftrightarrow y)$ is critical two-point connectivity. The condition controls the intersection effects that spoil a branching approximation. It is a sufficient criterion for important [mean-field percolation exponents](critical-phenomenon.md#mean-field-percolation-exponents), including the order-parameter, [percolation susceptibility](#percolation-susceptibility) and cluster-tail exponents. Establishing detailed spatial asymptotics is a further task, commonly addressed by [lace expansion](probability-theory.md#lace-expansion).

## Percolation two-point connection probability

↑ **Parent:** [Bond percolation](bond-percolation.md)

The two-point [percolation two-point connection probability](#percolation-two-point-connection-probability) $\tau_p(x,y)=\mathbb P_p(x\leftrightarrow y)$ is the [probability](probability-theory.md#probability) that two fixed [graph vertices](graph.md#vertex-graph-theory) belong to the same [percolation cluster](#percolation-cluster). On a translation-invariant lattice it depends on their displacement. Restricting the permitted connecting [graph paths](graph-theory.md#path-in-a-graph) to a subgraph gives the corresponding confined [percolation two-point connection probability](#percolation-two-point-connection-probability). The [Harris-FKG inequality](probability-inequality.md#harris-fkg-inequality) implies $\tau_p(x,z)\geq\tau_p(x,y)\tau_p(y,z)$.

### Reflection lower bound for two-point percolation

↑ **Parent:** [Percolation two-point connection probability](#percolation-two-point-connection-probability)

For [bond percolation](bond-percolation.md) on the [square lattice](graph.md#square-lattice), write $h_n=\mathbb P_p(0\leftrightarrow(n,0))$ and $g_k=\mathbb P_p(0\leftrightarrow\partial[-k,k]^2)$. A maximal-probability boundary [graph vertex](graph.md#vertex-graph-theory) can be placed at $(k,j)$ by symmetry. Reflection about $x=k$ identifies its connection [probability](probability-theory.md#probability) from $0$ with that from $(2k,0)$. The [Harris-FKG inequality](probability-inequality.md#harris-fkg-inequality) yields $(g_k/(8k))^2\leq h_{2k}\leq g_{2k}$ for $k\geq1$.

## Connection decay rate in a percolation strip

↑ **Parent:** [Bond percolation](bond-percolation.md)

For nearest-neighbour [bond percolation](bond-percolation.md) with $0<p<1$ on the strip $T_k=\mathbb Z\times\{-k,\ldots,k\}$, put $q_k(n)=\mathbb P_p((0,0)\leftrightarrow(n,0)\text{ in }T_k)$. The [Harris-FKG inequality](probability-inequality.md#harris-fkg-inequality) and translation invariance imply $q_k(n+m)\geq q_k(n)q_k(m)$. Thus $-\log q_k(n)$ is a [subadditive sequence](real-analysis.md#subadditive-sequence), and the [Fekete lemma](real-analysis.md#fekete-s-lemma) gives

$$
f_k(p)=\inf_{n\geq1}-\frac1n\log q_k(n),\qquad q_k(n)\leq e^{-nf_k(p)}.
$$

The direct horizontal [graph path](graph-theory.md#path-in-a-graph) gives $0\leq f_k(p)\leq-\log p$. Enlarging the strip increases every [percolation two-point connection probability](#percolation-two-point-connection-probability), so $f_k(p)$ is nonincreasing in $k$ and has a nonnegative [limit of a sequence](real-analysis.md#limit-of-a-sequence).

### Strip approximation to the planar connection decay rate

↑ **Parent:** [Connection decay rate in a percolation strip](#connection-decay-rate-in-a-percolation-strip)

Let $q(n)$ be the unrestricted planar two-point [percolation two-point connection probability](#percolation-two-point-connection-probability). Every finite connecting [graph path](graph-theory.md#path-in-a-graph) is contained in some strip, so $q_k(n)\uparrow q(n)$ for each fixed $n$. Therefore

$$
\lim_{k\to\infty}f_k(p)=\inf_{k\geq1}\inf_{n\geq1}\frac{-\log q_k(n)}n=\inf_{n\geq1}\frac{-\log q(n)}n.
$$

The equality uses commuting infima and monotonicity, not an unjustified interchange of two general limits. The right-hand side is the whole-plane connection decay rate by the [Fekete lemma](real-analysis.md#fekete-s-lemma).

### Closed-cut bound for percolation in a strip

↑ **Parent:** [Connection decay rate in a percolation strip](#connection-decay-rate-in-a-percolation-strip)

A vertical cut between consecutive columns of $T_k$ contains $2k+1$ [edges](graph-theory.md#edge-of-a-graph). All are closed with [probability](probability-theory.md#probability) $(1-p)^{2k+1}$. Cuts in different columns use disjoint [edges](graph-theory.md#edge-of-a-graph), so their closed-cut events are independent. A connection from column zero to column $n$ must cross each of the intervening $n$ cuts. Consequently

$$
q_k(n)\leq\bigl(1-(1-p)^{2k+1}\bigr)^n,\qquad f_k(p)\geq-\log\bigl(1-(1-p)^{2k+1}\bigr)>0.
$$

This finite-width obstruction persists even when the unrestricted planar percolation is supercritical.

## Translation ergodicity of Bernoulli percolation

↑ **Parent:** [Bond percolation](bond-percolation.md)

The independent edge law of [bond percolation](bond-percolation.md) on $\mathbb Z^d$ is ergodic under lattice translations: every translation-invariant event has probability zero or one.

## Percolation cluster

↑ **Parent:** [Bond percolation](bond-percolation.md)

In [bond percolation](bond-percolation.md), a [percolation cluster](#percolation-cluster) is a [connected component of a graph](graph.md#component-graph-theory) formed by the open [edges](graph-theory.md#edge-of-a-graph), with every [graph vertex](graph.md#vertex-graph-theory) retained. In [site percolation](site-percolation.md), it is a [connected component of a graph](graph.md#component-graph-theory) of the subgraph induced by the open [graph vertices](graph.md#vertex-graph-theory). Write $C(x)$ for the cluster containing $x$; for [site percolation](site-percolation.md) set $C(x)=\varnothing$ when $x$ is closed.

### Maximum cluster radius under exponential one-arm decay

↑ **Parent:** [Percolation cluster](#percolation-cluster)

Suppose the [one-arm probability](#one-arm-probability) on the [cubic lattice](graph.md#cubic-lattice) satisfies $\beta_r=\exp(-\lambda r+o(r))$ with $\lambda>0$. Define $M_n$ as the largest maximum-norm radius of any cluster rooted in $[-n,n]^d$. Then $M_n/\log n\to d/\lambda$ [convergence in probability](convergence-of-random-variables.md#convergence-in-probability). An upper bound is a [union bound](probability-inequality.md#boole-s-inequality) over $O(n^d)$ roots. For a lower bound, pack $\Theta((n/\log n)^d)$ disjoint radius-$O(\log n)$ boxes and use the independent first-hit connection events inside them. Clusters are finite almost surely under the positive-rate hypothesis.

### Infinite percolation cluster

↑ **Parent:** [Percolation cluster](#percolation-cluster)

An infinite [percolation cluster](#percolation-cluster) is an open [connected component of a graph](graph.md#component-graph-theory) with infinitely many [graph vertices](graph.md#vertex-graph-theory). On a countable translation-invariant lattice, a zero root [percolation probability](probability-theory.md#percolation-probability) implies that no [infinite percolation cluster](#infinite-percolation-cluster) exists [almost surely](convergence-of-random-variables.md#almost-sure-convergence), by the countable union over all [graph vertices](graph.md#vertex-graph-theory). A positive root [probability](probability-theory.md#probability) implies almost-sure existence by [translation ergodicity of Bernoulli percolation](#translation-ergodicity-of-bernoulli-percolation); uniqueness is an additional theorem.

### Uniqueness of the infinite percolation cluster

↑ **Parent:** [Percolation cluster](#percolation-cluster)

For independent [site percolation](site-percolation.md) or [bond percolation](bond-percolation.md) on the [cubic lattice](graph.md#cubic-lattice) $\mathbb Z^d$, there is [almost surely](convergence-of-random-variables.md#almost-sure-convergence) at most one [infinite percolation cluster](#infinite-percolation-cluster) at every fixed parameter. Above the [percolation critical probability](probability-theory.md#percolation-critical-probability), there is exactly one [almost surely](convergence-of-random-variables.md#almost-sure-convergence). This theorem is called the [Burton-Keane theorem](#uniqueness-of-the-infinite-percolation-cluster). Existence uses translation ergodicity together with positive [percolation probability](probability-theory.md#percolation-probability); uniqueness is a separate conclusion. At $p=1$ uniqueness is deterministic.

#### Percolation uniqueness on an amenable quasi-transitive graph

↑ **Parent:** [Uniqueness of the infinite percolation cluster](#uniqueness-of-the-infinite-percolation-cluster)

For a connected infinite [locally finite graph](graph-theory.md#locally-finite-graph) that is also an [amenable graph](graph.md#amenable-graph) and a [quasi-transitive graph](graph.md#quasi-transitive-graph), an invariant independent [site percolation](site-percolation.md) law with every orbit parameter strictly between $0$ and $1$ has either no [infinite percolation cluster](#infinite-percolation-cluster) or exactly one, almost surely. Invariance and independence give a zero–one law. The [finite-energy property of Bernoulli percolation](probability-theory.md#finite-energy-property-of-bernoulli-percolation) excludes a fixed finite number greater than one by opening a finite joining region. Infinitely many clusters would create an [encounter box in percolation](#encounter-box-in-percolation) with positive probability; translated disjoint boxes then have positive density, contradicting the boundary count in a [Følner sequence](geometric-group-theory.md#folner-sequence). The finite-energy hypothesis matters if some orbit parameters are $0$ or $1$.

#### Boundary counting proof of percolation uniqueness

↑ **Parent:** [Uniqueness of the infinite percolation cluster](#uniqueness-of-the-infinite-percolation-cluster)

Independent [bond percolation](bond-percolation.md) on $\mathbb Z^2$ has at most one [infinite percolation cluster](#infinite-percolation-cluster) at every parameter, including a possible critical parameter. The number of [infinite percolation clusters](#infinite-percolation-cluster) is constant [almost surely](convergence-of-random-variables.md#almost-sure-convergence) by [translation ergodicity of Bernoulli percolation](#translation-ergodicity-of-bernoulli-percolation). A finite constant larger than one is impossible: a box meeting two clusters can be made entirely open, joining them and decreasing that number with positive [probability](probability-theory.md#probability) by [finite modification of Bernoulli percolation](probability-theory.md#finite-modification-of-bernoulli-percolation).

If infinitely many clusters existed, a box would meet three with positive [probability](probability-theory.md#probability). Preserve one infinite exterior arm from each and replace the finitely many interior and boundary [edges](graph-theory.md#edge-of-a-graph) by a three-armed [tree](combinatorics.md#tree-graph-theory) joining them, closing the remaining [edges](graph-theory.md#edge-of-a-graph). Its branch [graph vertex](graph.md#vertex-graph-theory) becomes a [trifurcation vertex in percolation](#trifurcation-vertex-in-percolation). Translation invariance therefore gives a positive density $q$. But the [trifurcation boundary-counting lemma](#trifurcation-boundary-counting-lemma) gives $q|W|\leq|\partial^+W|$ for every large box, contradicting vanishing boundary-to-volume ratio. This proves uniqueness without assuming absence of an [infinite percolation cluster](#infinite-percolation-cluster) at criticality.

##### Encounter box in percolation

↑ **Parent:** [Boundary counting proof of percolation uniqueness](#boundary-counting-proof-of-percolation-uniqueness)

An encounter box is a finite connected set of open vertices whose removal from its [infinite percolation cluster](#infinite-percolation-cluster) leaves at least three infinite connected components. Unlike a [trifurcation vertex in percolation](#trifurcation-vertex-in-percolation), it allows branching to occur across several vertices, which is useful for [site percolation](site-percolation.md) on graphs with local cycles. Contract disjoint encounter boxes to junctions. In a finite region, each junction must connect at least three different exits. Pruning to a forest gives at most as many junctions as boundary exits, by the identity $\sum_v(\deg(v)-2)=-2$ for a finite [tree](combinatorics.md#tree-graph-theory). Positive density of encounter boxes is therefore incompatible with an [amenable graph](graph.md#amenable-graph).

#### Trifurcation vertex in percolation

↑ **Parent:** [Uniqueness of the infinite percolation cluster](#uniqueness-of-the-infinite-percolation-cluster)

A trifurcation [graph vertex](graph.md#vertex-graph-theory) is a [graph vertex](graph.md#vertex-graph-theory) of an infinite [percolation cluster](#percolation-cluster) whose deletion separates that cluster into at least three infinite [connected components of a graph](graph.md#component-graph-theory). In a finite modification argument one may make it have exactly three open incident [edges](graph-theory.md#edge-of-a-graph) leading to three different infinite components. On a translation-invariant lattice, a positive [probability](probability-theory.md#probability) of trifurcation at one [graph vertex](graph.md#vertex-graph-theory) gives a positive expected density of trifurcations.

##### Trifurcation boundary-counting lemma

↑ **Parent:** [Trifurcation vertex in percolation](#trifurcation-vertex-in-percolation)

For a finite [graph vertex](graph.md#vertex-graph-theory) [set](set.md) $W$ in a [locally finite graph](graph-theory.md#locally-finite-graph), let $\partial^+W$ be its exterior [graph neighbours](graph-theory.md#neighbour-of-a-vertex). The number of [trifurcation vertices in percolation](#trifurcation-vertex-in-percolation) lying in $W$ is at most $|\partial^+W|$.

For each cluster meeting $W$, contract its [connected components of a graph](graph.md#component-graph-theory) outside $W$ to terminal [graph vertices](graph.md#vertex-graph-theory), keeping only those adjacent to $W$. The resulting incidence [graph](graph.md) is finite and connected. Each trifurcation [graph vertex](graph.md#vertex-graph-theory) in $W$ separates at least three groups of terminals, because every infinite branch must leave the [finite set](set.md#finite-set) $W$. Take a minimal subtree connecting all terminals. Each such trifurcation is unavoidable in that subtree and has [degree of a vertex](graph-theory.md#degree-graph-theory) at least three. All leaves are terminals. The [tree](combinatorics.md#tree-graph-theory) identity $\sum_v(\deg(v)-2)=-2$ bounds the number of these branching [graph vertices](graph.md#vertex-graph-theory) by the number of leaves minus two, hence by the number of terminals. Different terminals, even across different clusters, can be assigned different exterior [graph neighbours](graph-theory.md#neighbour-of-a-vertex). Summing proves the bound. For square boxes in $\mathbb Z^2$, the boundary has order $n$ and the volume has order $n^2$.

###### Forest proof of trifurcation boundary counting

↑ **Parent:** [Trifurcation boundary-counting lemma](#trifurcation-boundary-counting-lemma)

Delete a finite set of degree-three [trifurcation vertices in percolation](#trifurcation-vertex-in-percolation) in each [infinite percolation cluster](#infinite-percolation-cluster) and contract the remaining components to nodes. The incidence graph is a [tree](combinatorics.md#tree-graph-theory): a cycle would bypass an original [trifurcation vertex in percolation](#trifurcation-vertex-in-percolation). All leaf components are infinite, otherwise a [graph vertex](graph.md#vertex-graph-theory) would have a finite branch after deletion. The [tree](combinatorics.md#tree-graph-theory) degree identity gives at least two more infinite leaves than degree-three [graph vertices](graph.md#vertex-graph-theory). Distinct infinite components escape a containing box through distinct outer boundary [graph vertices](graph.md#vertex-graph-theory). Hence the number of counted trifurcations is at most the outer boundary size.

## Percolation susceptibility

↑ **Parent:** [Bond percolation](bond-percolation.md)

The percolation susceptibility is the expected size of the open cluster containing a specified root:

$$
\chi(p)=\mathbb E_p|C(o)|.
$$

### Tree-graph moment bound for a percolation cluster

↑ **Parent:** [Percolation susceptibility](#percolation-susceptibility)

For translation-invariant independent [bond percolation](bond-percolation.md) with finite [percolation susceptibility](#percolation-susceptibility) $\chi=\sum_y\mathbb P(0\leftrightarrow y)$, the [BK inequality](#van-den-berg-kesten-inequality) gives $\mathbb E|C_0|^k\le(2k-3)!!\chi^{2k-1}$ for $k\ge1$, with $(-1)!!=1$. Prune a connecting open [tree](combinatorics.md#tree-graph-theory) for the $k+1$ labelled vertices, suppress unmarked degree-two vertices, and split higher branching into binary branching with zero-length connections. There are $(2k-3)!!$ binary tree topologies and $2k-1$ connections. The connections have disjoint bond witnesses, so the [BK inequality](#van-den-berg-kesten-inequality) bounds their joint [probability](probability-theory.md#probability) by a product of two-point connection [probabilities](probability-theory.md#probability). Summing successive leaves contributes $\chi$ for each connection. Since $(2k-3)!!\le2^{k-1}(k-1)!$, this proves $\mathbb E e^{t|C_0|}\le1-(2\chi)^{-1}\log(1-2t\chi^2)$ for $0<t<(2\chi^2)^{-1}$. Finite [percolation susceptibility](#percolation-susceptibility) therefore gives an exponential cluster-volume tail.

### Exponential one-arm decay from finite susceptibility

↑ **Parent:** [Percolation susceptibility](#percolation-susceptibility)

The [percolation susceptibility](#percolation-susceptibility) is $\chi(p)=1+\sum_{m\geq1}\sum_{y\in\partial\Lambda_m}\tau_p(0,y)$. Finiteness gives a boundary sum $a<1$. The [weighted BK boundary-splitting estimate](#weighted-bk-boundary-splitting-estimate) then gives $g_k\leq a^{\lfloor k/m\rfloor}$. The strict bound $g_1=1-(1-p)^{2d}<1$ absorbs the finitely many smaller radii into a positive exponential rate with unit prefactor. At $p=0$, all positive-radius connection [probabilities](probability-theory.md#probability) are zero.

## Russo-Seymour-Welsh theorem

↑ **Parent:** [Bond percolation](bond-percolation.md)

At critical planar percolation, the probability of an open crossing of a rectangle of any fixed aspect ratio stays bounded away from zero and one uniformly over its scale.

### Uniform RSW crossing estimate

↑ **Parent:** [Russo-Seymour-Welsh theorem](#russo-seymour-welsh-theorem)

For independent [bond percolation](bond-percolation.md) on the [square lattice](graph.md#square-lattice), a positive uniform lower bound for square crossings implies a positive uniform lower bound for rectangle crossings of every fixed aspect ratio $\rho>1$. The [RSW reflection extension lemma](#rsw-reflection-extension-lemma) first extends a square to aspect ratio $3/2$. Overlapping rectangles and transverse overlap-square crossings then glue using the [Harris-FKG inequality](probability-inequality.md#harris-fkg-inequality). The required constant depends on $\delta$ and $\rho$, not on scale. At a self-dual parameter, dual crossings also give a uniform upper bound below one.

### RSW reflection extension lemma

↑ **Parent:** [Russo-Seymour-Welsh theorem](#russo-seymour-welsh-theorem)

For independent [bond percolation](bond-percolation.md) on the [square lattice](graph.md#square-lattice) at $p=1/2$, square crossing [probabilities](probability-theory.md#probability) bounded below by self-duality extend to a uniform positive bound for rectangles of aspect ratio $3/2$. Expose an extremal vertical square crossing, reflect its geometry, and attach it to an exterior side through an unexposed independent region. Reflection symmetry bounds the attachment [probability](probability-theory.md#probability) below. Two attachments and a horizontal square crossing join by the [Harris-FKG inequality](probability-inequality.md#harris-fkg-inequality). Overlapping rectangles and transverse overlap-square crossings then give all fixed aspect ratios. Reflecting a geometrical [graph path](graph-theory.md#path-in-a-graph) does not require its reflected [edges](graph-theory.md#edge-of-a-graph) to be open.

#### Reflected attachment estimate for percolation

↑ **Parent:** [RSW reflection extension lemma](#rsw-reflection-extension-lemma)

In a rectangle $[0,m]\times[0,2n]$, $m\geq n$, let $X$ require an open vertical crossing of the corner square $[0,n]^2$ attached to the rectangle's right side. Explore the leftmost vertical crossing of the square without inspecting edges to its right. Reflect its geometry in the line $y=n$, obtaining a deterministic separator. Every horizontal rectangle crossing reaches this separator from the right; reflection divides these possible attachments into two equally probable choices, so the lower-half attachment has probability at least half the horizontal crossing probability. The required edges remain unexposed and independent of the explored crossing. Averaging proves the estimate. Reflected geometry need not be open.

### One-arm probability

↑ **Parent:** [Russo-Seymour-Welsh theorem](#russo-seymour-welsh-theorem)

The one-arm probability $\pi(r)$ is the probability that a specified vertex has an open path to distance $r$.

#### Weighted BK boundary-splitting estimate

↑ **Parent:** [One-arm probability](#one-arm-probability)

For independent [bond percolation](bond-percolation.md) on the [cubic lattice](graph.md#cubic-lattice), define $\tau_p(x,y)=\mathbb P_p(x\leftrightarrow y)$ and $g_n=\mathbb P_p(0\leftrightarrow\partial\Lambda_n)$, with $g_0=1$. Split an open [self-avoiding walk](combinatorics.md#self-avoiding-walk) at its first radius-$m$ boundary vertex $y$. The remaining segment reaches distance at least $n-m$ from $y$, using disjoint edges. The [BK inequality](#van-den-berg-kesten-inequality), translation invariance and the [union bound](probability-inequality.md#boole-s-inequality) yield the displayed estimate. Keeping the individual connection weights can be stronger than replacing their sum by $|\partial\Lambda_m|g_m$.

#### Polynomial critical one-arm upper bound

↑ **Parent:** [One-arm probability](#one-arm-probability)

At $p=1/2$ for independent [bond percolation](bond-percolation.md) on the [square lattice](graph.md#square-lattice), there exist $C<\infty$ and $\alpha>0$ with $\mathbb P_{1/2}(0\leftrightarrow\partial[-n,n]^2)\leq Cn^{-\alpha}$. The [Russo-Seymour-Welsh theorem](#russo-seymour-welsh-theorem) and the [Harris-FKG inequality](probability-inequality.md#harris-fkg-inequality) give a uniform positive [probability](probability-theory.md#probability) of a closed dual [graph cycle](graph-theory.md#cycle-in-a-graph) around each geometrically spaced square ring. The [independent annular barriers for percolation](#independent-annular-barriers-for-percolation) give the polynomial bound and imply zero critical [percolation probability](probability-theory.md#percolation-probability). This does not determine the exact critical exponent.

#### Independent annular barriers for percolation

↑ **Parent:** [One-arm probability](#one-arm-probability)

Closed dual [graph cycles](graph-theory.md#cycle-in-a-graph) in disjoint square rings depend on disjoint primal [edge](graph-theory.md#edge-of-a-graph) sets. In independent [bond percolation](bond-percolation.md) their barrier events are independent. If each event has [probability](probability-theory.md#probability) at least $\delta>0$, an open [graph path](graph-theory.md#path-in-a-graph) from the origin across $k$ rings has [probability](probability-theory.md#probability) at most $(1-\delta)^k$. A geometric sequence of radii turns this estimate into the [polynomial critical one-arm upper bound](#polynomial-critical-one-arm-upper-bound).

#### BK boundary-splitting estimate

↑ **Parent:** [One-arm probability](#one-arm-probability)

For [bond percolation](bond-percolation.md) on the [square lattice](graph.md#square-lattice), put $g_n=\mathbb P_p(0\leftrightarrow\partial[-n,n]^2)$. Splitting an open [self-avoiding walk](combinatorics.md#self-avoiding-walk) at its first visit to the radius-$m$ boundary gives disjoint certificates for reaching a boundary [graph vertex](graph.md#vertex-graph-theory) and then reaching radius $n$ about that [graph vertex](graph.md#vertex-graph-theory). The [Van den Berg-Kesten inequality](#van-den-berg-kesten-inequality) and the [union bound](probability-inequality.md#boole-s-inequality) give $g_{m+n}\leq8m g_mg_n$ for positive $m,n$. With $g_0=1$ and $|\partial\Lambda_0|=1$, the boundary-cardinality form holds for zero indices as well.

#### Percolation one-arm decay rate

↑ **Parent:** [One-arm probability](#one-arm-probability)

For [bond percolation](bond-percolation.md) on the [square lattice](graph.md#square-lattice), the [one-arm probability](#one-arm-probability) $g_n=\mathbb P_p(0\leftrightarrow\partial[-n,n]^2)$ has a root [limit of a sequence](real-analysis.md#limit-of-a-sequence) $\gamma(p)\in[p,1]$. The [BK boundary-splitting estimate](#bk-boundary-splitting-estimate) implies that $32n^2g_n$ is submultiplicative for positive integers. Applying the [Fekete lemma](real-analysis.md#fekete-s-lemma) to its logarithm proves existence when $p>0$; at $p=0$ the rate is zero. The same rate is the root limit of the [percolation two-point connection probability](#percolation-two-point-connection-probability) along a coordinate axis, by the [reflection lower bound for two-point percolation](#reflection-lower-bound-for-two-point-percolation).

##### Almost-subadditive percolation decay rate

↑ **Parent:** [Percolation one-arm decay rate](#percolation-one-arm-decay-rate)

For independent [bond percolation](bond-percolation.md) of density $0<p<1$ on the [cubic lattice](graph.md#cubic-lattice) in dimension $d\geq2$, let $\beta_n$ be the [one-arm probability](#one-arm-probability) for reaching maximum-norm distance $n$. The [weighted BK boundary-splitting estimate](#weighted-bk-boundary-splitting-estimate) gives $\beta_{m+n}\leq|\partial\Lambda_n|\beta_m\beta_n$. Since the logarithm of this boundary size is $o(n)$, the [asymmetrically almost-subadditive sequence](real-analysis.md#asymmetrically-almost-subadditive-sequence) argument applies to $\log\beta_n$. The rate exists and lies in $[0,-\log p]$; positive rate gives exponential decay.

#### One-arm extension estimate

↑ **Parent:** [One-arm probability](#one-arm-probability)

The [Russo-Seymour-Welsh theorem](#russo-seymour-welsh-theorem) and the [Harris-FKG inequality](probability-inequality.md#harris-fkg-inequality) imply $\pi(2r)\geq c\pi(r)$ for a scale-independent constant $c>0$.

##### RSW gluing lemma for two one-arm events

↑ **Parent:** [One-arm extension estimate](#one-arm-extension-estimate)

RSW rectangle crossings and positive association join two separated one-arm events with probability bounded below uniformly over scale.

## Van den Berg-Kesten inequality

↑ **Parent:** [Bond percolation](bond-percolation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Van_den_Berg–Kesten_inequality)

For increasing events $A,B$ in a product percolation measure, their disjoint occurrence satisfies $\mathbb P(A\mathbin\square B)\leq\mathbb P(A)\mathbb P(B)$.

### Coordinate-splitting proof of the BK inequality

↑ **Parent:** [Van den Berg-Kesten inequality](#van-den-berg-kesten-inequality)

For [increasing events](probability-inequality.md#increasing-event) $A,B$ under a finite [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) [product measure](probability-theory.md#product-measure), first assume all parameters are at most $1/2$. Write $A_0\subseteq A_1$ and $B_0\subseteq B_1$ for last-coordinate sections. The zero-section of their [disjoint occurrence of increasing events](#disjoint-occurrence-of-increasing-events) is $A_0\square B_0$; its one-section is $(A_1\square B_0)\cup(A_0\square B_1)$. The intersection in this union contains $A_0\square B_0$. If $a_i=\mathbb P(A_i)$, $b_i=\mathbb P(B_i)$ and the last parameter is $p\leq1/2$, [mathematical induction](foundations-of-mathematics.md#mathematical-induction) bounds disjoint occurrence by $(1-2p)a_0b_0+p a_1b_0+p a_0b_1$. The product of the two marginal [probabilities](probability-theory.md#probability) exceeds this bound by $p^2(a_1-a_0)(b_1-b_0)\geq0$. For a larger parameter $p_i<1$, replace that coordinate by the [logical disjunction](mathematical-logic.md#logical-disjunction) of $m_i$ [independent](random-variable.md#independent-random-variables) bits with parameter $1-(1-p_i)^{1/m_i}\leq1/2$. Disjoint original witnesses lift to disjoint bit witnesses. Apply the small-parameter inequality and then pass to degenerate parameters by continuity.

### Square-lattice one-arm lower bound from disjoint occurrence

↑ **Parent:** [Van den Berg-Kesten inequality](#van-den-berg-kesten-inequality)

At density $1/2$, planar duality gives crossing probability $1/2$ for the $2n$-by-$(2n-1)$ lattice rectangle. A self-avoiding left-right crossing passes through one of its $2n$ middle-column vertices. At that vertex its two halves are disjoint edge witnesses for two copies of the radius-$n$ connection event. The [BK inequality](#van-den-berg-kesten-inequality) and the [union bound](probability-inequality.md#boole-s-inequality) give $1/2\leq2n\mathbb P_{1/2}(0\leftrightarrow\partial[-n,n]^2)^2$, proving the estimate.

### Disjoint occurrence of increasing events

↑ **Parent:** [Van den Berg-Kesten inequality](#van-den-berg-kesten-inequality)

A finite open coordinate [set](set.md) witnesses an [increasing event](probability-inequality.md#increasing-event) when prescribing those coordinates open forces the event, regardless of the remaining configuration. The [disjoint occurrence of increasing events](#disjoint-occurrence-of-increasing-events) $A\square B$ means that $A$ and $B$ have disjoint finite witnesses. For finite-coordinate events this is the usual disjoint-occurrence definition. The [Van den Berg-Kesten inequality](#van-den-berg-kesten-inequality) bounds its [probability](probability-theory.md#probability) by $\mathbb P(A)\mathbb P(B)$ under an independent [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) [product measure](probability-theory.md#product-measure).

## ↑ Ancestors (6)

1. [Percolation theory](probability-theory.md#percolation-theory)
2. [Probability theory](probability-theory.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (65)

- [Almost-subadditive percolation decay rate](#almost-subadditive-percolation-decay-rate)
- [BK boundary-splitting estimate](#bk-boundary-splitting-estimate)
- [Boundary counting proof of percolation uniqueness](#boundary-counting-proof-of-percolation-uniqueness)
- [Cluster weight in the random-cluster model](site-percolation.md#cluster-weight-in-the-random-cluster-model)
- [Conformal invariance of planar percolation](probability-theory.md#conformal-invariance-of-planar-percolation)
- [Connection decay rate in a percolation strip](#connection-decay-rate-in-a-percolation-strip)
- [Connective-constant lower bound for percolation](probability-theory.md#connective-constant-lower-bound-for-percolation)
- [Connective-constant Peierls bound](probability-theory.md#connective-constant-peierls-bound)
- [Directed percolation](probability-theory.md#directed-percolation)
- [Dual bond percolation](graph-theory.md#dual-bond-percolation)
- [Dual contour bound for a finite planar cluster](graph-theory.md#dual-contour-bound-for-a-finite-planar-cluster)
- [Exponential tail of subcritical cluster size](probability-theory.md#exponential-tail-of-subcritical-cluster-size)
- [Finite-box comparison for percolation parameters](probability-theory.md#finite-box-comparison-for-percolation-parameters)
- [Harris-Kesten theorem](probability-theory.md#harris-kesten-theorem)
- [Incoming-edge coupling of site and bond percolation](probability-theory.md#incoming-edge-coupling-of-site-and-bond-percolation)
- [Independent annular barriers for percolation](#independent-annular-barriers-for-percolation)
- [Martini lattice](graph-theory.md#martini-lattice)
- [Near-critical percolation power upper bound](probability-theory.md#near-critical-percolation-power-upper-bound)
- [One-independent bond percolation](site-percolation.md#one-independent-bond-percolation)
- [Parallel-bond ray with different site and bond thresholds](probability-theory.md#parallel-bond-ray-with-different-site-and-bond-thresholds)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-28.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-37.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-37.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-13.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-2.md#10f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-30.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-30.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-30.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-26.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-26.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-28.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-28.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-28.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-214.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-214.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-214.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-214.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-212.md#1/a/solution)
- [Percolation cluster](#percolation-cluster)
- [Percolation one-arm decay rate](#percolation-one-arm-decay-rate)
- [Percolation universality hypothesis](critical-phenomenon.md#percolation-universality-hypothesis)
- [Polynomial critical one-arm upper bound](#polynomial-critical-one-arm-upper-bound)
- [Rectangle crossing in bond percolation](#rectangle-crossing-in-bond-percolation)
- [Reflection lower bound for two-point percolation](#reflection-lower-bound-for-two-point-percolation)
- [Right continuity of percolation probability](probability-theory.md#right-continuity-of-percolation-probability)
- [Root-moment bound for open self-avoiding walks](combinatorics.md#root-moment-bound-for-open-self-avoiding-walks)
- [RSW reflection extension lemma](#rsw-reflection-extension-lemma)
- [Sharpness of the percolation transition](probability-theory.md#sharpness-of-the-percolation-transition)
- [Supercritical continuity of percolation probability](probability-theory.md#supercritical-continuity-of-percolation-probability)
- [Survival and susceptibility thresholds for directed percolation](probability-theory.md#survival-and-susceptibility-thresholds-for-directed-percolation)
- [Three-fold symmetric primal-dual noncoexistence](probability-theory.md#three-fold-symmetric-primal-dual-noncoexistence)
- [Translation ergodicity of Bernoulli percolation](#translation-ergodicity-of-bernoulli-percolation)
- [Tree-graph moment bound for a percolation cluster](#tree-graph-moment-bound-for-a-percolation-cluster)
- [Uniform random orientation out-cluster comparison](#uniform-random-orientation-out-cluster-comparison)
- [Uniform RSW crossing estimate](#uniform-rsw-crossing-estimate)
- [Uniqueness of the infinite percolation cluster](#uniqueness-of-the-infinite-percolation-cluster)
- [Weighted BK boundary-splitting estimate](#weighted-bk-boundary-splitting-estimate)
