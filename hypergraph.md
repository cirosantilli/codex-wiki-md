# Hypergraph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hypergraph)

A hypergraph consists of a [vertex set](graph.md#vertex-set) $V$ and a family $E$ of subsets of $V$, called hyperedges. Unlike a [graph](graph.md), a hyperedge may contain more than two vertices. A [uniform hypergraph](#uniform-hypergraph) restricts all hyperedges to one fixed size.

**Table of contents**

- [Subhypergraph](#subhypergraph)
  - [Induced subhypergraph](#induced-subhypergraph)
- [Matching in a hypergraph](#matching-in-a-hypergraph)
- [Hypergraph link graph](#hypergraph-link-graph)
  - [Fano completion through three matchings](#fano-completion-through-three-matchings)
- [Hypergraph colouring](#hypergraph-colouring)
  - [Hypergraph chromatic index](#hypergraph-chromatic-index)
    - [Auxiliary matching construction for hypergraph edge colouring](#auxiliary-matching-construction-for-hypergraph-edge-colouring)
  - [Property B](#property-b)
    - [Bipartite three-uniform hypergraph](#bipartite-three-uniform-hypergraph)
  - [Hypergraph chromatic number](#hypergraph-chromatic-number)
- [Linear hypergraph](#linear-hypergraph)
- [Vertex of a hypergraph](#vertex-of-a-hypergraph)
- [Labelled hypergraph copy count](#labelled-hypergraph-copy-count)
- [Multipartite hypergraph](#multipartite-hypergraph)
- [Edge of a hypergraph](#edge-of-a-hypergraph)
- [Polychromatic hypergraph colouring](#polychromatic-hypergraph-colouring)
  - [Four-vertex obstruction to polychromatic three-colouring](#four-vertex-obstruction-to-polychromatic-three-colouring)
- [Hypergraph isomorphism](#hypergraph-isomorphism)
- [Hyperedge](#hyperedge)
- [Polychromatic coloring of a hypergraph](#polychromatic-coloring-of-a-hypergraph)
  - [Polychromatic coloring of integer translates](#polychromatic-coloring-of-integer-translates)
- [Extremal hypergraph theory](#extremal-hypergraph-theory)
  - [Fano-plane Turán theorem](#fano-plane-turan-theorem)
    - [Fano stability](#fano-stability)
  - [Cyclic Turán covering construction](#cyclic-turan-covering-construction)
  - [Turán density](#turan-density)
    - [Hypergraph supersaturation by sampling](#hypergraph-supersaturation-by-sampling)
    - [de Caen bound for hypergraph Turán density](#de-caen-bound-for-hypergraph-turan-density)
- [Multihypergraph](#multihypergraph)
- [Hypergraph independent set](#hypergraph-independent-set)
  - [Hypergraph container](#hypergraph-container)
    - [Hypergraph container theorem](#hypergraph-container-theorem)
    - [Golden rule for container algorithms](#golden-rule-for-container-algorithms)
    - [Container fingerprint](#container-fingerprint)
- [Hypergraph vertex degree](#hypergraph-vertex-degree)
  - [Hypergraph degree measure](#hypergraph-degree-measure)
  - [Hypergraph codegree](#hypergraph-codegree)
- [Uniform hypergraph](#uniform-hypergraph)
  - [Hereditary hypergraph property](#hereditary-hypergraph-property)
    - [Normalized speed of a hereditary hypergraph property](#normalized-speed-of-a-hereditary-hypergraph-property)
  - [Octahedral quasirandomness of a three-uniform hypergraph](#octahedral-quasirandomness-of-a-three-uniform-hypergraph)
    - [Counting lemma for octahedrally quasirandom three-uniform hypergraphs](#counting-lemma-for-octahedrally-quasirandom-three-uniform-hypergraphs)
  - [Link hypergraph](#link-hypergraph)
  - [Countable random uniform hypergraph](#countable-random-uniform-hypergraph)
  - [Hypergraph extension property](#hypergraph-extension-property)
    - [Universal countable uniform hypergraph](#universal-countable-uniform-hypergraph)
      - [Maximal-vertex deletion in a countable universal hypergraph](#maximal-vertex-deletion-in-a-countable-universal-hypergraph)
  - [Strong regularity for three-uniform hypergraphs](#strong-regularity-for-three-uniform-hypergraphs)
    - [Triad in a hypergraph regularity partition](#triad-in-a-hypergraph-regularity-partition)
      - [Tetrahedron counting lemma](#tetrahedron-counting-lemma)
  - [Hypergraph removal](#hypergraph-removal)
    - [Tetrahedron removal lemma](#tetrahedron-removal-lemma)
  - [Complete uniform hypergraph](#complete-uniform-hypergraph)
    - [Strong saturation of a uniform hypergraph](#strong-saturation-of-a-uniform-hypergraph)
      - [Exterior-power quotient bound for strong hypergraph saturation](#exterior-power-quotient-bound-for-strong-hypergraph-saturation)
    - [Three-uniform tetrahedron](#three-uniform-tetrahedron)
  - [Hypergraph complement](#hypergraph-complement)

## Subhypergraph

↑ **Parent:** [Hypergraph](hypergraph.md)

A subhypergraph restricts the [vertex set](graph.md#vertex-set) of a [hypergraph](hypergraph.md) and retains some of its edges contained in that vertex set. Retaining every such edge gives an [induced subhypergraph](#induced-subhypergraph).

### Induced subhypergraph

↑ **Parent:** [Subhypergraph](#subhypergraph)

For a subset $W$ of the [vertex set](graph.md#vertex-set) of a [hypergraph](hypergraph.md) $H$, the induced subhypergraph retains exactly the edges wholly contained in $W$. This is the restriction used by a [hereditary hypergraph property](#hereditary-hypergraph-property); it differs from intersecting every edge with $W$, which can change uniformity.

## Matching in a hypergraph

↑ **Parent:** [Hypergraph](hypergraph.md)

A [matching in a hypergraph](#matching-in-a-hypergraph) is a family of pairwise vertex-disjoint [hypergraph edges](#edge-of-a-hypergraph). A perfect [matching in a hypergraph](#matching-in-a-hypergraph) covers every vertex; an almost-perfect [matching in a hypergraph](#matching-in-a-hypergraph) leaves a small proportion uncovered. In a proper edge colouring, each colour class is a [matching in a hypergraph](#matching-in-a-hypergraph).

## Hypergraph link graph

↑ **Parent:** [Hypergraph](hypergraph.md)

For a three-[uniform hypergraph](#uniform-hypergraph), the link of a vertex $v$ is the ordinary [graph](graph.md) on the remaining vertices in which $xy$ is an edge precisely when $vxy$ is a [hyperedge](#hyperedge). Its edge count is the [hypergraph vertex degree](#hypergraph-vertex-degree) of $v$.

### Fano completion through three matchings

↑ **Parent:** [Hypergraph link graph](#hypergraph-link-graph)

If $xyz$ is a [hyperedge](#hyperedge) and the links of $x,y,z$ on four other vertices contain the three perfect matchings of a $K_4$, then those seven vertices contain a [Fano plane](projective-space.md#fano-plane). There is a second completion: if the link of $v$ contains three disjoint pairs, and the other six vertices contain all transversal triples through those pairs, take four triples of even parity and the three triples containing $v$. This again gives a Fano plane. These finite templates convert forbidden Fano copies into missing cross-part triples.

## Hypergraph colouring

↑ **Parent:** [Hypergraph](hypergraph.md)

A proper [hypergraph colouring](#hypergraph-colouring) assigns colours to the [vertices of a hypergraph](#vertex-of-a-hypergraph) so that no [hypergraph edge](#edge-of-a-hypergraph) is [monochromatic](ramsey-theory.md#monochromatic-set). Each [colour class](ramsey-theory.md#colour-class) is a [hypergraph independent set](#hypergraph-independent-set). This is often called weak colouring, to distinguish it from requiring every pair of vertices in each [edge](graph-theory.md#edge-of-a-graph) to have different colours.

### Hypergraph chromatic index

↑ **Parent:** [Hypergraph colouring](#hypergraph-colouring)

The chromatic index of a [hypergraph](hypergraph.md) is the minimum number of colours needed to colour its edges so that intersecting edges have different colours. Each colour class is a [matching in a hypergraph](#matching-in-a-hypergraph). It is at least the maximum [hypergraph vertex degree](#hypergraph-vertex-degree), and at most $r(\Delta-1)+1$ for an $r$-uniform [hypergraph](hypergraph.md) of maximum degree $\Delta$, by greedily colouring edges: an edge meets at most $r(\Delta-1)$ others.

#### Auxiliary matching construction for hypergraph edge colouring

↑ **Parent:** [Hypergraph chromatic index](#hypergraph-chromatic-index)

Given an $r$-uniform [hypergraph](hypergraph.md) $H$ and $K$ colours, construct an $(r+1)$-uniform auxiliary [hypergraph](hypergraph.md) with one task vertex for every $e\in E(H)$ and one resource vertex $(v,c)$ for every original vertex and colour. The assignment edge for $(e,c)$ contains the task $e$ and all resources $(v,c)$ with $v\in e$. A [matching in a hypergraph](#matching-in-a-hypergraph) of assignments is exactly a proper partial edge colouring. Task degrees are $K$; resource degrees are $d_H(v)$. Pairwise auxiliary [hypergraph codegrees](#hypergraph-codegree) are at most $\max(1,\max_{v\ne w}d_H(v,w))$. Thus nearly equal original degrees and small original [hypergraph codegrees](#hypergraph-codegree) transfer to the setting of a [Rödl nibble](probabilistic-combinatorics.md#rodl-nibble). A locally balanced [Rödl nibble](probabilistic-combinatorics.md#rodl-nibble) must control the unmatched task count in every original star, not merely the total uncovered proportion.

### Property B

↑ **Parent:** [Hypergraph colouring](#hypergraph-colouring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Property_B)

A [hypergraph](hypergraph.md) has [Property B](#property-b) if its [vertices of a hypergraph](#vertex-of-a-hypergraph) can be coloured with two colours so that every [hypergraph edge](#edge-of-a-hypergraph) meets both [colour classes](ramsey-theory.md#colour-class). An $r$-[uniform hypergraph](#uniform-hypergraph) with fewer than $2^{r-1}$ [edges](graph-theory.md#edge-of-a-graph) has [Property B](#property-b), by a fair [independent](random-variable.md#independent-random-variables) colouring and the [union bound](probability-inequality.md#boole-s-inequality). Conversely, for $r\geq2$, take $N=2r^2$ vertices and independently sample $m=\lceil(N\log2+1)2^r\rceil$ uniformly random $r$-subsets. In any fixed colouring an [edge](graph-theory.md#edge-of-a-graph) is [monochromatic](ramsey-theory.md#monochromatic-set) with [probability](probability-theory.md#probability) at least $2^{-r}$: [convexity](real-analysis.md#convex-function) of [binomial coefficients](combinatorics.md#binomial-coefficient) reduces to the balanced colouring, and $\binom{r^2}{r}/\binom{2r^2}{r}\geq2^{-r-1}$. The [union bound](probability-inequality.md#boole-s-inequality) over $2^N$ colourings gives a [probability](probability-theory.md#probability) at most $2^N e^{-m2^{-r}}<1$ of any proper colouring. Removing repeated [edges](graph-theory.md#edge-of-a-graph) leaves a [hypergraph](hypergraph.md) without [Property B](#property-b) and with $O(r^22^r)$ [edges](graph-theory.md#edge-of-a-graph).

#### Bipartite three-uniform hypergraph

↑ **Parent:** [Property B](#property-b)

A three-[uniform hypergraph](#uniform-hypergraph) is bipartite when its vertex set has a partition into two parts such that every [hyperedge](#hyperedge) meets both parts. All such triples on parts of sizes $a,b$ number $a\binom b2+b\binom a2=ab(a+b-2)/2$. For fixed total order this is maximized by balanced parts.

### Hypergraph chromatic number

↑ **Parent:** [Hypergraph colouring](#hypergraph-colouring)

The [hypergraph chromatic number](#hypergraph-chromatic-number) is the minimum number of colours in a proper [hypergraph colouring](#hypergraph-colouring). If $H$ has $N$ vertices and maximum [hypergraph independent set](#hypergraph-independent-set) size $a$, then $\chi(H)\geq N/a$, since the [colour classes](ramsey-theory.md#colour-class) partition its [vertex set](graph.md#vertex-set) into [hypergraph independent sets](#hypergraph-independent-set).

## Linear hypergraph

↑ **Parent:** [Hypergraph](hypergraph.md)

A [hypergraph](hypergraph.md) is linear when two distinct [hypergraph edges](#edge-of-a-hypergraph) intersect in at most one [vertex of a hypergraph](#vertex-of-a-hypergraph). Equivalently, every pair of distinct [vertices of a hypergraph](#vertex-of-a-hypergraph) has [hypergraph codegree](#hypergraph-codegree) at most one. This restricts local overlap without bounding the [hypergraph chromatic number](#hypergraph-chromatic-number): the [random alteration method](probabilistic-combinatorics.md#random-alteration-method) gives linear three-uniform [hypergraphs](hypergraph.md) of arbitrarily large [hypergraph chromatic number](#hypergraph-chromatic-number).

## Vertex of a hypergraph

↑ **Parent:** [Hypergraph](hypergraph.md)

A vertex of a [hypergraph](hypergraph.md) $H=(V,E)$ is an element of its ground set $V$. Each [hypergraph edge](#edge-of-a-hypergraph) is a subset of $V$, and isolated vertices may belong to no edge. In a [multipartite hypergraph](#multipartite-hypergraph), each vertex additionally lies in exactly one of the specified parts. This is the hypergraph analogue of a [vertex of a graph](graph.md#vertex-graph-theory), allowing edges of cardinality other than two.

## Labelled hypergraph copy count

↑ **Parent:** [Hypergraph](hypergraph.md)

For [hypergraphs](hypergraph.md) $F,H$, a labelled copy is an [injective function](algebra.md#injective-function) $\phi:V(F)\to V(H)$ taking every [hypergraph edge](#edge-of-a-hypergraph) of $F$ to an [hypergraph edge](#edge-of-a-hypergraph) of $H$. Specified [vertex of a hypergraph](#vertex-of-a-hypergraph) classes may additionally require $\phi(i)\in V_i$. The count is the sum, over these [injective](algebra.md#injective-function) maps, of the product of the host [hypergraph edge](#edge-of-a-hypergraph) indicators. Without injectivity the same expression counts [hypergraph](hypergraph.md) homomorphisms. On a common host of size $n$, their counts differ by at most $\binom{|V(F)|}{2}n^{|V(F)|-1}$: every noninjective map identifies at least one pair of abstract [vertices of a hypergraph](#vertex-of-a-hypergraph), each prescribed equality permits at most $n^{|V(F)|-1}$ maps, and the [union bound](probability-inequality.md#boole-s-inequality) completes the estimate. An induced copy additionally preserves nonedges, so its indicator product includes nonedge factors. The [counting lemma for octahedrally quasirandom three-uniform hypergraphs](#counting-lemma-for-octahedrally-quasirandom-three-uniform-hypergraphs) estimates these labelled products when the requisite centered triple indicators have small box [norm](functional-analysis.md#norm).

## Multipartite hypergraph

↑ **Parent:** [Hypergraph](hypergraph.md)

A multipartite [hypergraph](hypergraph.md) has a specified partition of its [vertex of a hypergraph](#vertex-of-a-hypergraph) [set](set.md) into parts, and every [hypergraph edge](#edge-of-a-hypergraph) meets each part in at most one [vertex of a hypergraph](#vertex-of-a-hypergraph). For an $r$-[uniform hypergraph](#uniform-hypergraph) with $r$ parts, an [hypergraph edge](#edge-of-a-hypergraph) chooses exactly one [vertex of a hypergraph](#vertex-of-a-hypergraph) from each part; its indicator is therefore a [function](function.md) on the [Cartesian product](set-theory.md#cartesian-product) of those parts. A quadripartite three-uniform [hypergraph](hypergraph.md) instead has four possible types of [hypergraph edge](#edge-of-a-hypergraph), according to the omitted part. A choice of one [vertex of a hypergraph](#vertex-of-a-hypergraph) from each of its four parts is a [three-uniform tetrahedron](#three-uniform-tetrahedron) exactly when all four triples are [hypergraph edges](#edge-of-a-hypergraph). Specifying the parts makes both [subset density](additive-combinatorics.md#density-of-a-finite-subset) and labelled counting precise.

## Edge of a hypergraph

↑ **Parent:** [Hypergraph](hypergraph.md)

An edge of a [hypergraph](hypergraph.md) is one of its specified subsets of the vertex set. In a [uniform hypergraph](#uniform-hypergraph) all edges have the same cardinality; unlike an ordinary [edge of a graph](graph-theory.md#edge-of-a-graph), an edge may contain more than two vertices.

## Polychromatic hypergraph colouring

↑ **Parent:** [Hypergraph](hypergraph.md)

A colouring is polychromatic with $r$ colours if every [hypergraph edge](#edge-of-a-hypergraph) contains a vertex of every colour. This is stronger than requiring every edge to be nonmonochromatic. Under independent uniform colours, a $k$-element edge misses at least one of three colours with probability $3(2/3)^k-3(1/3)^k$. If each edge meets at most $m$ other edges, the edge-intersection [dependency graph of events](probabilistic-combinatorics.md#dependency-graph-of-events) and the [Lovász local lemma](probabilistic-combinatorics.md#lovasz-local-lemma) therefore give a polychromatic three-colouring whenever $e(m+1)[3(2/3)^k-3(1/3)^k]\leq1$.

### Four-vertex obstruction to polychromatic three-colouring

↑ **Parent:** [Polychromatic hypergraph colouring](#polychromatic-hypergraph-colouring)

Take every three-element subset of a four-element vertex set as a [hypergraph edge](#edge-of-a-hypergraph). Any three-colouring repeats a colour on two vertices. A triple containing that pair cannot contain all three colours. Thus this [uniform hypergraph](#uniform-hypergraph) has no polychromatic three-colouring, although each edge meets only three other edges.

## Hypergraph isomorphism

↑ **Parent:** [Hypergraph](hypergraph.md)

A hypergraph isomorphism is a [bijection](function.md#bijection) of the [vertex sets](graph.md#vertex-set) such that a subset is a [hyperedge](#hyperedge) of the first [hypergraph](hypergraph.md) if and only if its image is a [hyperedge](#hyperedge) of the second. The condition preserves both edges and nonedges. In the two-uniform case it is the usual relation of [isomorphic graphs](graph.md#graph-isomorphism).

## Hyperedge

↑ **Parent:** [Hypergraph](hypergraph.md)

A hyperedge is a member of the edge family of a [hypergraph](hypergraph.md). In an $r$-[uniform hypergraph](#uniform-hypergraph) it is an $r$-element subset of the [vertex set](graph.md#vertex-set). For $r=2$ it is an ordinary [edge of a graph](graph-theory.md#edge-of-a-graph). A simple [hypergraph](hypergraph.md) has no repeated hyperedges; a [multihypergraph](#multihypergraph) records multiplicities.

## Polychromatic coloring of a hypergraph

↑ **Parent:** [Hypergraph](hypergraph.md)

A [polychromatic coloring of a hypergraph](#polychromatic-coloring-of-a-hypergraph) assigns $k$ colors to vertices so that every hyperedge contains all $k$ colors. It is stronger than merely requiring each hyperedge to be nonmonochromatic. Independently random colors and the [Lovász local lemma](probabilistic-combinatorics.md#lovasz-local-lemma) can construct such colorings when edges are sufficiently large relative to their overlap degrees.

### Polychromatic coloring of integer translates

↑ **Parent:** [Polychromatic coloring of a hypergraph](#polychromatic-coloring-of-a-hypergraph)

For finite $S\subset\mathbb Z$, use vertices $\mathbb Z$ and hyperedges $S+t$. Independent uniform $k$-coloring gives missing-color probability at most $ke^{-|S|/k}$, and the [dependency graph of events](probabilistic-combinatorics.md#dependency-graph-of-events) has degree at most $|S|(|S|-1)$. For $k\ge20$ and $|S|\ge6k\log k$, the symmetric [Lovász local lemma](probabilistic-combinatorics.md#lovasz-local-lemma) condition holds. The [compactness extension of the Lovász local lemma](probabilistic-combinatorics.md#compactness-extension-of-the-lovasz-local-lemma) gives a coloring in which every translate contains every color.

## Extremal hypergraph theory

↑ **Parent:** [Hypergraph](hypergraph.md)

Extremal hypergraph theory studies the largest or smallest possible size of a [hypergraph](hypergraph.md) under prescribed forbidden-subhypergraph or covering conditions. It generalizes [extremal graph theory](graph-theory.md#extremal-graph-theory). The [Turán density](#turan-density) describes the asymptotic maximum edge proportion for a fixed uniform forbidden hypergraph.

<h3 id="fano-plane-turan-theorem">Fano-plane Turán theorem</h3>

↑ **Parent:** [Extremal hypergraph theory](#extremal-hypergraph-theory)

For all sufficiently large $n$, the extremal number of the [Fano plane](projective-space.md#fano-plane) as a three-[uniform hypergraph](#uniform-hypergraph) is the displayed count of all triples crossing a balanced bipartition. The plane has no [Property B](#property-b), so this construction avoids it. A stability argument makes near-extremal Fano-free hypergraphs nearly bipartite; vertex deletion obtains high minimum degree. Optimizing the approximate bipartition and applying [Fano completion through three matchings](#fano-completion-through-three-matchings) then rules out all internal triples. The large-order qualification matters: for $n=5,6$ the complete hypergraph has no Fano copy but exceeds the displayed count.

#### Fano stability

↑ **Parent:** [Fano-plane Turán theorem](#fano-plane-turan-theorem)

For every $\rho>0$, some $\delta>0$ makes every sufficiently large Fano-free three-[uniform hypergraph](#uniform-hypergraph) of density at least $3/4-\delta$ admit a partition with at most $\rho n^3$ internal triples. The argument compares four [hypergraph link graphs](#hypergraph-link-graph) around a tetrahedron. Forbidden rainbow perfect matchings in their edge-coloured union force an approximate pattern with multiplicity two within the parts and four between them. A positive internal triple density would produce a complete tripartite six-vertex template, and its pairs together with a link vertex would complete a Fano plane.

<h3 id="cyclic-turan-covering-construction">Cyclic Turán covering construction</h3>

↑ **Parent:** [Extremal hypergraph theory](#extremal-hypergraph-theory)

With $r$ balanced cyclically ordered vertex classes and $2\le\ell\le r+1$, include an $\ell$-set if some start has at least $k+1$ vertices in its first $k$ classes for every $1\le k\le\ell-1$. The [cycle lemma](combinatorics.md#cycle-lemma) implies every $(r+1)$-set contains an edge. Its asymptotic density is $((\ell-1)/r)^{\ell-1}$; taking the [hypergraph complement](#hypergraph-complement) gives a lower bound for the [Turán density](#turan-density) of a complete uniform hypergraph.

<h3 id="turan-density">Turán density</h3>

↑ **Parent:** [Extremal hypergraph theory](#extremal-hypergraph-theory)

For a fixed $\ell$-uniform forbidden hypergraph $F$, its Turán density is the limit of $\operatorname{ex}(n,F)/\binom n\ell$. Averaging over smaller vertex subsets shows these normalized extremal numbers are nonincreasing, so the limit exists. For ordinary [graphs](graph.md), the [Erdős-Stone theorem](graph-theory.md#erdos-stone-theorem) determines it from the [chromatic number](graph-theory.md#chromatic-number).

#### Hypergraph supersaturation by sampling

↑ **Parent:** [Turán density](#turan-density)

Normalized hypergraph extremal numbers decrease under [vertex](graph.md#vertex-graph-theory) sampling and converge to [Turán density](#turan-density). At a fixed sample size where the extremal density is close to that limit, excess density forces a positive fraction of samples to contain $H$. Counting incidences of copies and samples proves the displayed lower bound. Shrinking $\delta$ also handles the finitely many small orders when the required count is rounded down.

<h4 id="de-caen-bound-for-hypergraph-turan-density">de Caen bound for hypergraph Turán density</h4>

↑ **Parent:** [Turán density](#turan-density)

For the complete $\ell$-uniform hypergraph $K_r^\ell$, with $r\ge\ell\ge2$, the bound is $\pi(K_r^\ell)\le1-1/\binom{r-1}{\ell-1}$. In the complementary covering formulation, every $r$-set containing an edge forces asymptotic edge density at least $1/\binom{r-1}{\ell-1}$. It follows from clique-extension incidence inequalities and [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) estimates on link degrees.

## Multihypergraph

↑ **Parent:** [Hypergraph](hypergraph.md)

A multihypergraph has a [multiset](set.md#multiset) of hyperedges, allowing the same subset of vertices to appear more than once. Its [hypergraph vertex degrees](#hypergraph-vertex-degree) and [hypergraph codegrees](#hypergraph-codegree) count multiplicity. Such multiplicity is important when several original hyperedges produce the same link in a [hypergraph container theorem](#hypergraph-container-theorem).

## Hypergraph independent set

↑ **Parent:** [Hypergraph](hypergraph.md)

A subset $I$ of the vertices of a [hypergraph](hypergraph.md) is independent when no hyperedge lies wholly inside $I$. This generalizes an [independent set](graph-theory.md#independent-set-graph-theory) in an ordinary [graph](graph.md). If a hypergraph has ordinary graph edges as its vertices and forbidden copies as its hyperedges, these independent sets encode graphs without those forbidden copies.

### Hypergraph container

↑ **Parent:** [Hypergraph independent set](#hypergraph-independent-set)

A container family is a collection of vertex subsets such that every [hypergraph independent set](#hypergraph-independent-set) lies in at least one member. A useful family has few members and each member is small in [hypergraph degree measure](#hypergraph-degree-measure) or induces few hyperedges. [Container fingerprints](#container-fingerprint) encode the members and permit bounds on the number of independent sets.

#### Hypergraph container theorem

↑ **Parent:** [Hypergraph container](#hypergraph-container)

For fixed uniformity, sufficiently small nonsingleton [hypergraph codegrees](#hypergraph-codegree) relative to $d\tau^{|\sigma|-1}$ permit a family of containers whose degree measures are bounded below one by a fixed amount. Each container has a [container fingerprint](#container-fingerprint) of size $O(\tau n)$. Iteration gives containers inducing at most an arbitrary fixed proportion of all hyperedges, with logarithmic family size $O(n\tau\log(1/\tau))$. The constants depend on the uniformity and desired edge proportion, and the average degree must be positive.

#### Golden rule for container algorithms

↑ **Parent:** [Hypergraph container](#hypergraph-container)

A container algorithm may use membership in the unknown independent set only through information recorded in its [container fingerprint](#container-fingerprint). With a deterministic ordering and deterministic tests, record every positive queried vertex; queried negative vertices can be excluded. All state updates must be recoverable from the fingerprint alone, so replaying the algorithm constructs a container without knowing the independent set.

#### Container fingerprint

↑ **Parent:** [Hypergraph container](#hypergraph-container)

A container fingerprint is a small vertex subset $T$, usually contained in a [hypergraph independent set](#hypergraph-independent-set) $I$, which determines a container $C(T)$ containing $I$. A deterministic membership-query algorithm records positive answers in $T$ and uses negative answers to remove vertices from the container. Reconstruction from $T$ follows the [golden rule for container algorithms](#golden-rule-for-container-algorithms).

## Hypergraph vertex degree

↑ **Parent:** [Hypergraph](hypergraph.md)

The degree of a vertex $u$ in a [hypergraph](hypergraph.md) is the number of hyperedges containing $u$. For a [uniform hypergraph](#uniform-hypergraph), summing degrees counts each hyperedge once for each of its vertices, so $\sum_u d_H(u)=r e(H)$. In a [multihypergraph](#multihypergraph), incidences are counted with multiplicity.

### Hypergraph degree measure

↑ **Parent:** [Hypergraph vertex degree](#hypergraph-vertex-degree)

For a [uniform hypergraph](#uniform-hypergraph) with positive average [hypergraph vertex degree](#hypergraph-vertex-degree) $d$, the degree measure is $\mu(S)=(nd)^{-1}\sum_{u\in S}d_H(u)$. It is a [probability measure](probability-theory.md#probability-measure) and equals $|S|/n$ in a regular hypergraph. Every [hypergraph independent set](#hypergraph-independent-set) has degree measure at most $1-1/r$, even when its fraction of all vertices is close to one.

### Hypergraph codegree

↑ **Parent:** [Hypergraph vertex degree](#hypergraph-vertex-degree)

The codegree of a vertex set $\sigma$ in a [hypergraph](hypergraph.md) is the number of hyperedges containing every vertex in $\sigma$. For a singleton this is the [hypergraph vertex degree](#hypergraph-vertex-degree); for two vertices it measures how often those vertices occur together. Subset codegrees of all sizes control the overlap relevant to the [hypergraph container theorem](#hypergraph-container-theorem).

## Uniform hypergraph

↑ **Parent:** [Hypergraph](hypergraph.md)

A hypergraph is $r$-uniform if each hyperedge has exactly $r$ vertices. Ordinary simple [graphs](graph.md) are 2-uniform hypergraphs. Its average [hypergraph vertex degree](#hypergraph-vertex-degree) is $r|E|/|V|$.

### Hereditary hypergraph property

↑ **Parent:** [Uniform hypergraph](#uniform-hypergraph)

A property of [uniform hypergraphs](#uniform-hypergraph) is hereditary if every [induced subhypergraph](#induced-subhypergraph) of a hypergraph with that property also has the property. It is understood to be invariant under relabelling the [vertex set](graph.md#vertex-set). For example, excluding a specified induced [hypergraph](hypergraph.md) is hereditary. This permits counting restrictions to smaller vertex sets using the same counting function.

#### Normalized speed of a hereditary hypergraph property

↑ **Parent:** [Hereditary hypergraph property](#hereditary-hypergraph-property)

For a [hereditary hypergraph property](#hereditary-hypergraph-property) of $r$-[uniform hypergraphs](#uniform-hypergraph), $\mathcal P_n$ is the family on the labelled [vertex set](graph.md#vertex-set) $[n]$. For $n\geq r$, its normalized speed lies between zero and two and is nonincreasing. Choose a uniformly random member on $n+1$ vertices and record its edge indicators. Each edge occurs in $n+1-r$ vertex-deletion restrictions. The [Shearer inequality](information-theory.md#shearer-s-inequality) bounds its [information entropy](information-theory.md#information-entropy) by the sum of the restriction entropies divided by $n+1-r$. Each restriction has at most $|\mathcal P_n|$ possible values. Division by $\binom{n+1}r$ gives $\log d_{n+1}\leq\log d_n$. Empty families are handled directly by heredity.

### Octahedral quasirandomness of a three-uniform hypergraph

↑ **Parent:** [Uniform hypergraph](#uniform-hypergraph)

For a tripartite three-[uniform hypergraph](#uniform-hypergraph) on nonempty finite parts $X,Y,Z$, let $h:X\times Y\times Z\to\{0,1\}$ be its [hypergraph edge](#edge-of-a-hypergraph) indicator, let $p=\mathbb Eh$ and put $g=h-p$. In the eighth-power convention, $\alpha$-quasirandomness means

$$
\|g\|_{\square^3}^8=\mathbb E_{x_0,x_1,y_0,y_1,z_0,z_1}\prod_{i,j,k\in\{0,1\}}g(x_i,y_j,z_k)\leq\alpha.
$$

All averages are uniform and independent, with repeated sampled [vertices of a hypergraph](#vertex-of-a-hypergraph) allowed. This expression is nonnegative because it equals $\mathbb E_{x_0,x_1,y_0,y_1}(\mathbb E_z\prod_{i,j}g(x_i,y_j,z))^2$. It measures correlations across the eight faces of a tripartite octahedral configuration. If instead the [norm](functional-analysis.md#norm) itself is used as the quasirandomness parameter, the parameter in this definition is its eighth power.

#### Counting lemma for octahedrally quasirandom three-uniform hypergraphs

↑ **Parent:** [Octahedral quasirandomness of a three-uniform hypergraph](#octahedral-quasirandomness-of-a-three-uniform-hypergraph)

Let a fixed simple three-[uniform hypergraph](#uniform-hypergraph) $F$ have $m$ [hypergraph edges](#edge-of-a-hypergraph), with one host [vertex of a hypergraph](#vertex-of-a-hypergraph) class $V_i$ for each [vertex of a hypergraph](#vertex-of-a-hypergraph). Assume each [hypergraph edge](#edge-of-a-hypergraph) triple has indicator $h_e$, [subset density](additive-combinatorics.md#density-of-a-finite-subset) $p_e$, and balanced [three-dimensional box norm](additive-combinatorics.md#three-dimensional-box-norm) at most $\alpha^{1/8}$. The normalized [labelled hypergraph copy count](#labelled-hypergraph-copy-count) is $\mathbb E\prod_{e\in E(F)}h_e$. Telescope this product against $\prod_ep_e$. In each error term, fix all variables outside the three [vertices of a hypergraph](#vertex-of-a-hypergraph) of its balanced [hypergraph edge](#edge-of-a-hypergraph). Every other [hypergraph edge](#edge-of-a-hypergraph) intersects that triple in at most two [vertices of a hypergraph](#vertex-of-a-hypergraph), so the remaining factors group into three pair [functions](function.md) bounded by one. The [pair-factor correlation bound for the three-dimensional box norm](additive-combinatorics.md#pair-factor-correlation-bound-for-the-three-dimensional-box-norm) bounds the error by $\alpha^{1/8}$. Summing gives

$$
\left|\#F-\left(\prod_ep_e\right)\left(\prod_i|V_i|\right)\right|\leq m\alpha^{1/8}\prod_i|V_i|.
$$

For the [three-uniform tetrahedron](#three-uniform-tetrahedron), $m=4$. The same argument with a common host [set](set.md) counts homomorphisms; excluding collisions of distinct abstract [vertices of a hypergraph](#vertex-of-a-hypergraph) changes the count by at most $\binom{|V(F)|}{2}|V|^{|V(F)|-1}$.

### Link hypergraph

↑ **Parent:** [Uniform hypergraph](#uniform-hypergraph)

The link at a fixed vertex $v$ of an $r$-[uniform hypergraph](#uniform-hypergraph) has vertex set $V(H)\setminus\{v\}$ and the displayed $(r-1)$-element [hyperedges](#hyperedge). For a [universal countable uniform hypergraph](#universal-countable-uniform-hypergraph), its link has the [hypergraph extension property](#hypergraph-extension-property): include $v$ in the finite set of vertices and prescribe only those $r$-edges containing $v$, completing the remaining prescription arbitrarily. Thus the link is a universal countable $(r-1)$-[uniform hypergraph](#uniform-hypergraph). In particular the link at a fixed vertex in the three-uniform case is the [Rado graph](graph-theory.md#rado-graph). This operation retains a specified vertex; deleting the maximum from every edge is a different operation.

### Countable random uniform hypergraph

↑ **Parent:** [Uniform hypergraph](#uniform-hypergraph)

Choose each $r$-element subset of the [natural numbers](arithmetic.md#natural-number) as a [hyperedge](#hyperedge) independently with [probability](probability-theory.md#probability) $p$, where $0<p<1$. This defines a countable random uniform hypergraph. For any finite pattern in the [hypergraph extension property](#hypergraph-extension-property), an outside vertex realizes it with probability $q=p^{|\mathcal A|}(1-p)^{|\binom S{r-1}\setminus\mathcal A|}>0$. Distinct outside vertices use disjoint edge decisions, so the probability that the first $N$ candidates all fail is $(1-q)^N\to0$. Taking a countable intersection over all finite patterns proves the extension property [almost surely](convergence-of-random-variables.md#almost-sure-convergence). The bounds $0<p<1$ are necessary for all patterns to have positive probability.

### Hypergraph extension property

↑ **Parent:** [Uniform hypergraph](#uniform-hypergraph)

An $r$-[uniform hypergraph](#uniform-hypergraph) has the extension property when, for every finite vertex set $S$ and every subfamily $\mathcal A\subseteq\binom S{r-1}$, there is a vertex $v\notin S$ such that $F\cup\{v\}$ is a [hyperedge](#hyperedge) exactly for $F\in\mathcal A$, among all $F\in\binom S{r-1}$. Every prescribed pattern has infinitely many witnesses: enlarge $S$ by any finite set of witnesses already found and prescribe the original pattern on its old $(r-1)$-subsets, with arbitrary choices on the new ones. For $r=2$, this says that any finite adjacency and nonadjacency prescription has a new realizing vertex.

#### Universal countable uniform hypergraph

↑ **Parent:** [Hypergraph extension property](#hypergraph-extension-property)

The universal countable uniform hypergraph is the unique, up to [hypergraph isomorphism](#hypergraph-isomorphism), countably infinite $r$-[uniform hypergraph](#uniform-hypergraph) with the [hypergraph extension property](#hypergraph-extension-property). To prove uniqueness, enumerate two such structures and construct finite partial [hypergraph isomorphisms](#hypergraph-isomorphism). Alternately add the least unused vertex of the first enumeration to the domain and the least unused vertex of the second to the range. Prescribe its incidences with every $(r-1)$-subset of the already matched vertices and apply the extension property in the other structure. The resulting union is a [bijection](function.md#bijection) preserving every [hyperedge](#hyperedge) and nonedge. Existence follows from the [countable random uniform hypergraph](#countable-random-uniform-hypergraph) construction. A construction with only the forward steps embeds every countable $r$-[uniform hypergraph](#uniform-hypergraph) as an induced subhypergraph, explaining the word universal. Its isomorphism type is independent of $p\in(0,1)$.

##### Maximal-vertex deletion in a countable universal hypergraph

↑ **Parent:** [Universal countable uniform hypergraph](#universal-countable-uniform-hypergraph)

Label the vertices of a [universal countable uniform hypergraph](#universal-countable-uniform-hypergraph) by the [natural numbers](arithmetic.md#natural-number) and remove the largest vertex of each [hyperedge](#hyperedge). The resulting $(r-1)$-[uniform hypergraph](#uniform-hypergraph) is complete. For any prescribed $(r-1)$-set $F$, apply the [hypergraph extension property](#hypergraph-extension-property) to a finite initial segment containing $F$, prescribing that $F$ extend to an edge. The resulting vertex is larger than every member of $F$, so this deletion produces $F$. This supplies a useful example of a projection that destroys the nonedge information of a random structure.

### Strong regularity for three-uniform hypergraphs

↑ **Parent:** [Uniform hypergraph](#uniform-hypergraph)

Strong regularity refines both the vertex classes and the pair graphs supporting triple hyperedges. The resulting [triads in a hypergraph regularity partition](#triad-in-a-hypergraph-regularity-partition) have nearly constant relative triple density outside a small exceptional weight. Pair and triple errors must be chosen in a hierarchy strong enough for a relative [tetrahedron counting lemma](#tetrahedron-counting-lemma); ordinary graph regularity on the vertex partition alone is insufficient. Refinement raises bounded conditional-density energies.

#### Triad in a hypergraph regularity partition

↑ **Parent:** [Strong regularity for three-uniform hypergraphs](#strong-regularity-for-three-uniform-hypergraphs)

A triad is the set of triples supported on one prescribed pair cell for each of the three pairs of vertex classes. Relative triple density is measured among those supported triples. In [strong hypergraph regularity](#strong-regularity-for-three-uniform-hypergraphs), the pair cells must themselves be sufficiently regular and have controlled density before a small relative [three-dimensional box norm](additive-combinatorics.md#three-dimensional-box-norm) can give a [tetrahedron counting lemma](#tetrahedron-counting-lemma).

##### Tetrahedron counting lemma

↑ **Parent:** [Triad in a hypergraph regularity partition](#triad-in-a-hypergraph-regularity-partition)

A sufficiently regular four-partite three-[uniform hypergraph](#uniform-hypergraph), supported on sufficiently regular pair cells of positive density and with positive relative triple densities, has a positive fourth-power number of [three-uniform tetrahedra](#three-uniform-tetrahedron). On complete pair supports, telescoping the four edge functions shows that an error of at most $\xi$ in each [three-dimensional box norm](additive-combinatorics.md#three-dimensional-box-norm) gives a counting error at most $4\xi$. The relative version additionally requires control of the pair-support densities.

### Hypergraph removal

↑ **Parent:** [Uniform hypergraph](#uniform-hypergraph)

For each fixed finite [uniform hypergraph](#uniform-hypergraph) $F$, having few copies of $F$ forces small edge-edit distance from an $F$-free [hypergraph](hypergraph.md). More precisely, for every $\eta>0$ there is $\rho>0$ such that fewer than $\rho v^{|V(F)|}$ copies can be eliminated by deleting fewer than $\eta v^r$ edges in an $r$-uniform [hypergraph](hypergraph.md). [Strong regularity for three-uniform hypergraphs](#strong-regularity-for-three-uniform-hypergraphs) and a relative counting lemma prove the case $r=3$.

#### Tetrahedron removal lemma

↑ **Parent:** [Hypergraph removal](#hypergraph-removal)

For every $\eta>0$, some $\rho>0$ has this property: a three-[uniform hypergraph](#uniform-hypergraph) on $v$ vertices with fewer than $\rho v^4$ copies of the [three-uniform tetrahedron](#three-uniform-tetrahedron) can be made tetrahedron-free by removing fewer than $\eta v^3$ hyperedges. The [four-term progression hypergraph encoding](additive-combinatorics.md#four-term-progression-hypergraph-encoding) converts this into the length-four case of the [Szemerédi theorem](probabilistic-combinatorics.md#szemeredi-s-theorem).

### Complete uniform hypergraph

↑ **Parent:** [Uniform hypergraph](#uniform-hypergraph)

The complete $\ell$-uniform hypergraph on $r$ vertices contains every $\ell$-subset of its [vertex set](graph.md#vertex-set). A hypergraph clique here means a restriction to a vertex subset of this form, rather than merely a clique in the pairwise shadow. For $\ell=2$, it is an ordinary [complete graph](graph-theory.md#complete-graph).

#### Strong saturation of a uniform hypergraph

↑ **Parent:** [Complete uniform hypergraph](#complete-uniform-hypergraph)

An $r$-[uniform hypergraph](#uniform-hypergraph) is strongly saturated with respect to a complete uniform hypergraph of order $r+t$ when every missing edge immediately completes such a clique. Existing cliques are allowed. All $r$-sets meeting a fixed $t$-set give an example: the witness for a missing edge is its union with that fixed set. It has $\binom nr-\binom{n-t}{r}$ edges, and the [exterior-power quotient bound for strong hypergraph saturation](#exterior-power-quotient-bound-for-strong-hypergraph-saturation) proves optimality.

##### Exterior-power quotient bound for strong hypergraph saturation

↑ **Parent:** [Strong saturation of a uniform hypergraph](#strong-saturation-of-a-uniform-hypergraph)

Take $U$ to be the kernel of a $t$-row [Vandermonde matrix](galois-theory.md#vandermonde-matrix) on distinct coordinates. For each $(r+t)$-set $T$, $U$ intersects its coordinate subspace in dimension $r$. Wedge a basis of that intersection: its coefficient on every $r$-subset of $T$ is nonzero, because projection onto that subset is an isomorphism by independence of the complementary $t$ columns. Modulo the [exterior power](linear-algebra.md#exterior-power) of $U$, this gives a dependence involving every clique edge with nonzero coefficient. Strong saturation expresses every missing-edge vector in the span of present ones. Since all coordinate-edge vectors span the quotient, edge count is at least its dimension.

#### Three-uniform tetrahedron

↑ **Parent:** [Complete uniform hypergraph](#complete-uniform-hypergraph)

The three-uniform tetrahedron is the [hypergraph](hypergraph.md) on four vertices with all four possible triple hyperedges. It is the [complete uniform hypergraph](#complete-uniform-hypergraph) $K_4^3$, and differs from its geometric realization as a [tetrahedron](geometry-and-topology.md#tetrahedron). Its edge pattern encodes four-term [arithmetic progressions](arithmetic.md#arithmetic-progression).

### Hypergraph complement

↑ **Parent:** [Uniform hypergraph](#uniform-hypergraph)

The complement of an $\ell$-uniform hypergraph on $V$ has all $\ell$-subsets of $V$ that are not hyperedges of the original hypergraph. An edge in every $r$-set of one hypergraph is equivalent to the absence of a complete $\ell$-uniform $r$-vertex hypergraph in its complement.

## ↑ Ancestors (5)

1. [Graph theory](graph-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (34)

- [Auxiliary matching construction for hypergraph edge colouring](#auxiliary-matching-construction-for-hypergraph-edge-colouring)
- [Edge of a hypergraph](#edge-of-a-hypergraph)
- [Extremal hypergraph theory](#extremal-hypergraph-theory)
- [Hereditary hypergraph property](#hereditary-hypergraph-property)
- [Hyperedge](#hyperedge)
- [Hypergraph chromatic index](#hypergraph-chromatic-index)
- [Hypergraph codegree](#hypergraph-codegree)
- [Hypergraph independent set](#hypergraph-independent-set)
- [Hypergraph isomorphism](#hypergraph-isomorphism)
- [Hypergraph removal](#hypergraph-removal)
- [Hypergraph vertex degree](#hypergraph-vertex-degree)
- [Induced subhypergraph](#induced-subhypergraph)
- [Labelled hypergraph copy count](#labelled-hypergraph-copy-count)
- [Linear hypergraph](#linear-hypergraph)
- [Multipartite hypergraph](#multipartite-hypergraph)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-1.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-11.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-14.md#2/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-14.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-14.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-10.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-79.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-110.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-110.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-110.md#5/solution)
- [Property B](#property-b)
- [Rödl nibble](probabilistic-combinatorics.md#rodl-nibble)
- [Subhypergraph](#subhypergraph)
- [Three-uniform tetrahedron](#three-uniform-tetrahedron)
- [Vertex of a hypergraph](#vertex-of-a-hypergraph)
- [Vertex set](graph.md#vertex-set)
