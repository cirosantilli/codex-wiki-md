# Probabilistic combinatorics

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Probabilistic_combinatorics)

Probabilistic combinatorics uses probability to prove the existence and typical properties of discrete structures.

**Table of contents**

- [Semi-random method](#semi-random-method)
  - [Rödl nibble](#rodl-nibble)
- [Probabilistic method](#probabilistic-method)
  - [Triangle deletion in the alteration method](#triangle-deletion-in-the-alteration-method)
  - [Dense integer sets with only logarithmic-length progressions](#dense-integer-sets-with-only-logarithmic-length-progressions)
- [With high probability](#with-high-probability)
- [Subcritical component bound for a binomial random graph](#subcritical-component-bound-for-a-binomial-random-graph)
  - [Sharp subcritical largest-component scale](#sharp-subcritical-largest-component-scale)
  - [Unicyclic component](#unicyclic-component)
    - [Labelled unicyclic graph count](#labelled-unicyclic-graph-count)
- [Hamiltonicity-to-pancyclicity sprinkling principle](#hamiltonicity-to-pancyclicity-sprinkling-principle)
- [Random alteration method](#random-alteration-method)
- [Lovász local lemma](#lovasz-local-lemma)
  - [Local lemma Ramsey lower bound](#local-lemma-ramsey-lower-bound)
  - [Dependency-degree obstruction on a rooted tree](#dependency-degree-obstruction-on-a-rooted-tree)
  - [Compactness extension of the Lovász local lemma](#compactness-extension-of-the-lovasz-local-lemma)
  - [Asymmetric Lovász local lemma](#asymmetric-lovasz-local-lemma)
  - [Dependency graph of events](#dependency-graph-of-events)
    - [Independence digraph of events](#independence-digraph-of-events)
  - [Lopsided Lovász local lemma](#lopsided-lovasz-local-lemma)
    - [Correlation graph of events](#correlation-graph-of-events)
- [Dependent random choice](#dependent-random-choice)
  - [Dense bipartite common-neighbour lemma](#dense-bipartite-common-neighbour-lemma)
  - [Bounded-degree bipartite Ramsey bound](#bounded-degree-bipartite-ramsey-bound)
  - [Common-neighbourhood sampling bound](#common-neighbourhood-sampling-bound)
  - [Complete-bipartite Ramsey completion lemma](#complete-bipartite-ramsey-completion-lemma)
  - [Rich set in a graph](#rich-set-in-a-graph)
    - [Rich-set embedding lemma](#rich-set-embedding-lemma)
- [Edge density of a bipartite graph](#edge-density-of-a-bipartite-graph)
  - [Bipartite four-cycle count](#bipartite-four-cycle-count)
    - [Bipartite four-cycle density](#bipartite-four-cycle-density)
  - [Regular pair of vertex sets](#regular-pair-of-vertex-sets)
    - [Dense regular pair from edge surplus](#dense-regular-pair-from-edge-surplus)
    - [Irregular pair of vertex sets](#irregular-pair-of-vertex-sets)
    - [Regular clique counting lemma](#regular-clique-counting-lemma)
      - [Regular triangle counting lemma](#regular-triangle-counting-lemma)
    - [Regular pair of bipartite partitions](#regular-pair-of-bipartite-partitions)
      - [Bipartite Szemerédi regularity lemma](#bipartite-szemeredi-regularity-lemma)
    - [Szemerédi regularity lemma](#szemeredi-regularity-lemma)
      - [Weighted Szemerédi regularity lemma](#weighted-szemeredi-regularity-lemma)
        - [Small-cell deletion in weighted regularity](#small-cell-deletion-in-weighted-regularity)
      - [Energy-increment proof of Szemerédi regularity](#energy-increment-proof-of-szemeredi-regularity)
      - [Induced regularity template lemma](#induced-regularity-template-lemma)
      - [Clique removal lemma](#clique-removal-lemma)
        - [Triangle removal lemma](#triangle-removal-lemma)
      - [Equitable regularity energy](#equitable-regularity-energy)
        - [Equalization with a controlled exceptional set](#equalization-with-a-controlled-exceptional-set)
        - [Refinement variance identity for regularity energy](#refinement-variance-identity-for-regularity-energy)
    - [Graph embedding lemma for regular pairs](#graph-embedding-lemma-for-regular-pairs)
      - [Odd-cycle copies from positive triangle density](#odd-cycle-copies-from-positive-triangle-density)
      - [Triangle embedding lemma for regular pairs](#triangle-embedding-lemma-for-regular-pairs)
    - [Reduced graph of a regularity partition](#reduced-graph-of-a-regularity-partition)
- [Szemerédi's theorem](#szemeredi-s-theorem)
  - [Dense three-term progressions force four-term progressions](#dense-three-term-progressions-force-four-term-progressions)
- [Locally dense graph thinning lemma](#locally-dense-graph-thinning-lemma)
- [Minimum-degree Ramsey lower bound](#minimum-degree-ramsey-lower-bound)

## Semi-random method

↑ **Parent:** [Probabilistic combinatorics](probabilistic-combinatorics.md)

The semi-random method constructs a combinatorial object in many small random rounds, discarding incompatible proposals and updating the remaining constraints after each round. Independent proposals give calculable expected changes; concentration and deterministic corrections preserve the statistics needed for subsequent rounds. Unlike a single random sample, this combines repeated randomness with a structured evolving state. The [Rödl nibble](#rodl-nibble) is a [matching in a hypergraph](hypergraph.md#matching-in-a-hypergraph) version of this method.

<h3 id="rodl-nibble">Rödl nibble</h3>

↑ **Parent:** [Semi-random method](#semi-random-method)

For a nearly $D$-regular $s$-uniform [hypergraph](hypergraph.md), sample each edge independently with [probability](probability-theory.md#probability) $\alpha/D$, where $\alpha$ is small. Retain the isolated sampled edges as a [matching in a hypergraph](hypergraph.md#matching-in-a-hypergraph), and delete every vertex incident to any sampled edge before the next round. A vertex survives with [probability](probability-theory.md#probability) $(1-\alpha/D)^{d(v)}\approx e^{-\alpha}$; a sampled edge meets another sampled edge with [probability](probability-theory.md#probability) at most $s\alpha(1+o(1))$. Thus accepted edges cover order $\alpha$ of the vertices and collision waste is order $\alpha^2$. Small [hypergraph codegrees](hypergraph.md#hypergraph-codegree) control the overlap terms in residual-degree calculations. Repeating a bounded number of rounds while tracking near-regularity is the characteristic [Rödl nibble](#rodl-nibble) mechanism.

## Probabilistic method

↑ **Parent:** [Probabilistic combinatorics](probabilistic-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Probabilistic_method)

The probabilistic method proves that a combinatorial object exists by defining a random object and showing that the desired property has positive probability. No efficient procedure for finding the object is required.

### Triangle deletion in the alteration method

↑ **Parent:** [Probabilistic method](#probabilistic-method)

If a graph has $E$ edges and $T$ triangles, successively delete one edge from a remaining triangle. No new triangle is created and at most $T$ deletions are needed, so a triangle-free subgraph has at least $E-T$ edges. A random-graph expectation lower bound on $E-T$ therefore proves existence of a large triangle-free graph. With edge probability $n^{-1/2}$, the expectation is $(n^2-1)/(3\sqrt n)$; this is a useful existence bound but is not within a constant factor of the sharp quadratic [Mantel theorem](graph-theory.md#mantel-theorem) bound.

### Dense integer sets with only logarithmic-length progressions

↑ **Parent:** [Probabilistic method](#probabilistic-method)

For any fixed density strictly below one, random subsets of an integer interval can have that density yet avoid [arithmetic progressions](arithmetic.md#arithmetic-progression) longer than a constant times the logarithm of the interval length. A [union bound](probability-inequality.md#boole-s-inequality) over possible progressions bounds their occurrence, while concentration of the random cardinality supplies a dense realization. Passing to a subset gives an exact prescribed cardinality.

## With high probability

↑ **Parent:** [Probabilistic combinatorics](probabilistic-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/With_high_probability)

An event depending on $n$ holds with high probability when its probability tends to one as $n\to\infty$.

## Subcritical component bound for a binomial random graph

↑ **Parent:** [Probabilistic combinatorics](probabilistic-combinatorics.md)

For every fixed $\varepsilon>0$, every [component](graph.md#component-graph-theory) of $G(n,(1-\varepsilon)/n)$ has $O_\varepsilon(\log n)$ vertices [with high probability](#with-high-probability). A breadth-first exploration is dominated by a branching process of mean $1-\varepsilon$; its total progeny has an exponentially decreasing tail.

### Sharp subcritical largest-component scale

↑ **Parent:** [Subcritical component bound for a binomial random graph](#subcritical-component-bound-for-a-binomial-random-graph)

For fixed $0<\lambda<1$ in $G(n,\lambda/n)$, the [largest component of a graph](graph.md#largest-component-of-a-graph) has the displayed order [with high probability](#with-high-probability). A dominating [Galton-Watson process](probability-and-statistics.md#galton-watson-process) gives the tail bound $\mathbb P(T\geq j)\leq e^{-(\lambda-1-\log\lambda)(j-1)}$ by the exponential [Markov inequality](probability-inequality.md#markov-inequality). For the lower bound, the [tree-component expectation in the Erdős-Rényi model](graph-theory.md#tree-component-expectation-in-the-erdos-renyi-model) diverges at $j=\lfloor(1-\eta)\log n/(\lambda-1-\log\lambda)\rfloor$. The disjoint-set covariance factor and the exclusion of overlaps give relative [variance](variance.md) tending to zero, so the [second moment method](probability-inequality.md#second-moment-method) supplies a [tree component](graph.md#tree-component) of that order.

### Unicyclic component

↑ **Parent:** [Subcritical component bound for a binomial random graph](#subcritical-component-bound-for-a-binomial-random-graph)

A connected graph is unicyclic when it contains exactly one cycle, equivalently when its numbers of vertices and edges agree.

A [pseudoforest](graph-theory.md#pseudoforest) permits both these components and acyclic [tree](combinatorics.md#tree-graph-theory) components.

#### Labelled unicyclic graph count

↑ **Parent:** [Unicyclic component](#unicyclic-component)

A labelled [unicyclic component](#unicyclic-component) has a unique cycle of length $k\geq3$, with a rooted forest attached to its vertices. Choose its vertices in $\binom nk$ ways and its unoriented cycle in $(k-1)!/2$ ways. The [labelled forest count with prescribed roots](combinatorics.md#labelled-forest-count-with-prescribed-roots) gives $kn^{n-k-1}$ attachments. Summing over $k$ and putting $j=n-k$ yields the displayed identity.

## Hamiltonicity-to-pancyclicity sprinkling principle

↑ **Parent:** [Probabilistic combinatorics](probabilistic-combinatorics.md)

For a decreasing probability sequence $p(n)$, if $G(n,p(n))$ contains a [Hamilton cycle](graph-theory.md#hamilton-cycle) [with high probability](#with-high-probability), then $G(n,Cp(n))$ is [pancyclic](graph-theory.md#pancyclic-graph) with high probability for every fixed sufficiently large $C$; three independent rounds suffice. One first exposes a Hamiltonian round and uses the independent sprinkled edges to create cycles of every shorter length.

## Random alteration method

↑ **Parent:** [Probabilistic combinatorics](probabilistic-combinatorics.md)

The random alteration method samples a random object and then deletes a small number of offending elements. If few forbidden configurations occur while the desired global property already holds, the altered object witnesses existence.

<h2 id="lovasz-local-lemma">Lovász local lemma</h2>

↑ **Parent:** [Probabilistic combinatorics](probabilistic-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lovász_local_lemma)

For bad events with a dependency graph of maximum degree $D$, the symmetric Lovász local lemma guarantees positive probability that none occurs whenever each event has probability at most $p$ and $ep(D+1)\leq1$.

### Local lemma Ramsey lower bound

↑ **Parent:** [Lovász local lemma](#lovasz-local-lemma)

In an independent random two-colouring of $K_N$, a given $k$-vertex [set](set.md) is monochromatic with [probability](probability-theory.md#probability) $2^{1-\binom k2}$. [Events](probability-theory.md#event) on [sets](set.md) intersecting in at most one vertex use disjoint edges. Thus dependency degree is at most $\binom k2\binom{N-2}{k-2}$. The [Lovász local lemma](#lovasz-local-lemma) gives a colouring avoiding all monochromatic $K_k$ when $e\,2^{1-\binom k2}(1+\binom k2\binom{N-2}{k-2})\leq1$. For $N=ck2^{k/2}$ the expression is $O(k^{3/2}(ec/\sqrt2)^k)$, by [Stirling's approximation](real-analysis.md#stirling-formula). Taking $c$ tending sufficiently slowly to $\sqrt2/e$ proves $R(k)\geq(\sqrt2/e+o(1))k2^{k/2}$.

### Dependency-degree obstruction on a rooted tree

↑ **Parent:** [Lovász local lemma](#lovasz-local-lemma)

Let $B_v$ be independent [Bernoulli random variables](discrete-probability-distribution.md#bernoulli-distribution) on a rooted $d$-ary [tree](combinatorics.md#tree-graph-theory), and put $A_v=\{B_v=1,\ B_w=0\text{ for every child }w\}$. Events at nonadjacent vertices use disjoint variables, giving a [dependency graph of events](#dependency-graph-of-events) of maximum degree $d+1$. Assign leaf success probability $p$ and successive probabilities $r_{j+1}=p/(1-r_j)^d$. If $p>\max_{0\leq r\leq1}r(1-r)^d=p_d$, the recursion eventually reaches one. Set the final root success probability to one. Each event has probability at most $p$, but following success vertices down from the root must reach an occurring event. Thus the bad events cover the sample space. This gives an upper bound for uniform avoidance thresholds without assuming a converse to the [Lovász local lemma](#lovasz-local-lemma).

<h3 id="compactness-extension-of-the-lovasz-local-lemma">Compactness extension of the Lovász local lemma</h3>

↑ **Parent:** [Lovász local lemma](#lovasz-local-lemma)

For countably many constraints on finite-valued variables, each involving finitely many variables, apply the finite [Lovász local lemma](#lovasz-local-lemma) to every finite constraint subfamily. Partial satisfying assignments on increasing finite variable sets form a finitely branching [tree](combinatorics.md#tree-graph-theory) with nonempty levels. The [König infinity lemma](combinatorics.md#konig-s-lemma) gives an infinite branch, producing one assignment satisfying all constraints. This existence argument does not assert positive probability of simultaneous avoidance in an infinite product space.

<h3 id="asymmetric-lovasz-local-lemma">Asymmetric Lovász local lemma</h3>

↑ **Parent:** [Lovász local lemma](#lovasz-local-lemma)

For a finite family with a [dependency graph of events](#dependency-graph-of-events), if $0\le x_i<1$ satisfy $\mathbb P(E_i)\le x_i\prod_{j\in N(i)}(1-x_j)$, then $\mathbb P(\bigcap_iE_i^c)\ge\prod_i(1-x_i)>0$. Choosing equal $x_i$ gives the familiar symmetric criterion $eq(d+1)\le1$ when event probabilities are at most $q$ and the maximum dependency degree is $d$.

### Dependency graph of events

↑ **Parent:** [Lovász local lemma](#lovasz-local-lemma)

A [dependency graph of events](#dependency-graph-of-events) joins potentially dependent events. Each event must be independent of the [sigma-algebra](measure-theory.md#sigma-algebra) generated by all its nonneighbors, a joint condition stronger than pairwise independence. In a product probability space, joining events whose sets of underlying independent variables overlap gives such a graph. This supplies the hypothesis of the [Lovász local lemma](#lovasz-local-lemma).

#### Independence digraph of events

↑ **Parent:** [Dependency graph of events](#dependency-graph-of-events)

For events $A_i$, a directed [graph](graph.md) is an independence digraph if $A_i$ is independent of the [sigma-algebra](measure-theory.md#sigma-algebra) generated by the events indexed by its non-outneighbors, excluding $i$. The direction records which joint independence condition is available. A cyclically oriented triangle imposes pairwise independence; it does not impose independence of all three events together.

<h3 id="lopsided-lovasz-local-lemma">Lopsided Lovász local lemma</h3>

↑ **Parent:** [Lovász local lemma](#lovasz-local-lemma)

Let $A_1,\ldots,A_m$ be bad events with a lopsidependency graph. If numbers $x_i\in[0,1)$ satisfy

$$
\mathbb P(A_i)\leq x_i\prod_{j\sim i}(1-x_j)
$$

for every $i$, then $\mathbb P(\bigcap_iA_i^c)>0$. Unlike the ordinary [Lovász local lemma](#lovasz-local-lemma), a lopsidependency graph may omit pairs whose interaction can only make their simultaneous avoidance easier.

#### Correlation graph of events

↑ **Parent:** [Lopsided Lovász local lemma](#lopsided-lovasz-local-lemma)

For bad events $A_i$, a correlation graph is sufficient for the [Lopsided Lovász local lemma](#lopsided-lovasz-local-lemma) when, for every set $S$ of nonneighbors and every positive-probability conditioning event, $\mathbb P(A_i\mid\bigcap_{j\in S}A_j^c)\leq\mathbb P(A_i)$. A [dependency graph of events](#dependency-graph-of-events) satisfies this with equality. The condition concerns simultaneous avoidance, not just signs of pairwise correlations.

## Dependent random choice

↑ **Parent:** [Probabilistic combinatorics](probabilistic-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dependent_random_choice)

Dependent random choice finds a large vertex set whose small subsets have large common neighbourhoods. In a bipartite graph with parts $A,B$, choose random vertices of $B$ with repetition and take their common neighbourhood $X\subseteq A$; convexity gives a lower bound for $\mathbb E|X|$, while counting subsets of $X$ with small common neighbourhood allows their deletion.

### Dense bipartite common-neighbour lemma

↑ **Parent:** [Dependent random choice](#dependent-random-choice)

In a [bipartite graph](graph-theory.md#bipartite-graph) with parts of sizes $m,n$ and density $\delta>0$, a neighbourhood $V'$ of size at least $\delta m/2$ can be chosen so that at least a proportion $1-2\epsilon/\delta^2$ of its ordered pairs have at least $\epsilon n$ [common neighbours](graph-theory.md#common-neighbour). Choose a random vertex on the other side, use the second moment of its degree, and penalize pairs with few [common neighbours](graph-theory.md#common-neighbour). This is a simple [dependent random choice](#dependent-random-choice) tool for controlling [restricted sumsets](additive-combinatorics.md#restricted-sumset).

### Bounded-degree bipartite Ramsey bound

↑ **Parent:** [Dependent random choice](#dependent-random-choice)

If a bipartite graph $H$ has $k$ vertices and [maximum degree](graph-theory.md#maximum-degree-of-a-graph) $d$, then

$$
R(H)=O(d^{2d}k).
$$

A [dependent random choice](#dependent-random-choice) argument finds, in one colour, enough vertices whose every subset of at most $d$ vertices has a large common neighbourhood; a greedy embedding then places $H$.

### Common-neighbourhood sampling bound

↑ **Parent:** [Dependent random choice](#dependent-random-choice)

If a bipartite graph with parts $A,B$ has density at least $p$, then averaging ordered distinct $t$-tuples gives a common neighbourhood of size at least

$$
|B|\left(p-\frac{t-1}{|A|}\right)^t.
$$

In particular this is at least $p^t|B|/2$ when $|A|$ is sufficiently large compared with $t^2/p$.

### Complete-bipartite Ramsey completion lemma

↑ **Parent:** [Dependent random choice](#dependent-random-choice)

The completion form of dependent random choice starts with $t=k-O(\log k)$ vertices having at least $c2^{-t}n$ common neighbours in one colour. Reapplying common-neighbourhood sampling inside the remaining polynomial-size set either completes these vertices to a monochromatic $K_{k,k}$ in that colour or produces a $K_{k,k}$ in the other colour. It yields

$$
R(K_{k,k})=O((\log k)2^k).
$$

### Rich set in a graph

↑ **Parent:** [Dependent random choice](#dependent-random-choice)

A vertex set $R$ is $(s,k)$-rich when every $s$-element subset of $R$ has at least $k$ common neighbours.

#### Rich-set embedding lemma

↑ **Parent:** [Rich set in a graph](#rich-set-in-a-graph)

If a bipartite graph $H$ has $k$ vertices and maximum degree at most $d$, then every graph containing a $(d,k)$-rich set of at least $k$ vertices contains a copy of $H$.

## Edge density of a bipartite graph

↑ **Parent:** [Probabilistic combinatorics](probabilistic-combinatorics.md)

For disjoint nonempty vertex sets $A,B$, their edge density is

$$
d(A,B)=\frac{e(A,B)}{|A||B|}.
$$

### Bipartite four-cycle count

↑ **Parent:** [Edge density of a bipartite graph](#edge-density-of-a-bipartite-graph)

If a [bipartite graph](graph-theory.md#bipartite-graph) with parts $X,Y$ has at least $\delta|X||Y|$ [edges](graph-theory.md#edge-of-a-graph), then the number of ordered tuples $(x_1,x_2,y_1,y_2)\in X^2\times Y^2$ for which every $x_iy_j$ is an edge is at least

$$
\delta^4|X|^2|Y|^2.
$$

Indeed, if $d(x_1,x_2)$ is the number of common neighbours of $x_1,x_2$ in $Y$, two applications of the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) give

$$
\sum_{x_1,x_2}d(x_1,x_2)^2
\geq\frac1{|X|^2}\left(\sum_y\deg(y)^2\right)^2
\geq\frac1{|X|^2|Y|^2}\left(\sum_y\deg(y)\right)^4.
$$

#### Bipartite four-cycle density

↑ **Parent:** [Bipartite four-cycle count](#bipartite-four-cycle-count)

This is the part-preserving [homomorphism density](graph-theory.md#homomorphism-density) of a four-cycle in a [bipartite graph](graph-theory.md#bipartite-graph) with independently uniform labels $x,x'$ in the first part and $y,y'$ in the second. Repeated labels are included. It equals the fourth power of the [four-cycle norm](additive-combinatorics.md#box-norm) of the adjacency [indicator function](measure-theory.md#indicator-function). It differs at finite sizes from a count requiring four distinct [vertices](graph.md#vertex-graph-theory).

### Regular pair of vertex sets

↑ **Parent:** [Edge density of a bipartite graph](#edge-density-of-a-bipartite-graph)

A pair $(A,B)$ is $\varepsilon$-regular when

$$
|d(X,Y)-d(A,B)|\leq\varepsilon
$$

whenever $X\subseteq A$, $Y\subseteq B$, $|X|\geq\varepsilon|A|$, and $|Y|\geq\varepsilon|B|$.

#### Dense regular pair from edge surplus

↑ **Parent:** [Regular pair of vertex sets](#regular-pair-of-vertex-sets)

The [Szemerédi regularity lemma](#szemeredi-regularity-lemma) gives equal cells. If every regular cross-cell pair had density at most $1/4$, their total edge contribution would be at most $n^2/8$. Exceptional vertices, within-cell edges and irregular pairs contribute at most $(2\eta+1/(2m_0))n^2$. Choosing $\eta=1/100$ and $m_0=100$ contradicts $e(G)=n^2/6$. The dense pair is $1/8$-regular since it is already $\eta$-regular.

#### Irregular pair of vertex sets

↑ **Parent:** [Regular pair of vertex sets](#regular-pair-of-vertex-sets)

For disjoint nonempty [vertex](graph.md#vertex-graph-theory) [sets](set.md) $U,V$ of a [graph](graph.md), an $\varepsilon$-irregular pair is one that is not an $\varepsilon$-[regular pair of vertex sets](#regular-pair-of-vertex-sets). Equivalently there are witnesses $U'\subseteq U$, $V'\subseteq V$ with $|U'|\geq\varepsilon|U|$, $|V'|\geq\varepsilon|V|$ and $|d(U',V')-d(U,V)|>\varepsilon$. Splitting both cells by these witnesses increases their contribution to the [regularity energy](#equitable-regularity-energy) by at least $\varepsilon^4|U||V|/n^2$: the witness rectangle has relative weight at least $\varepsilon^2$, its mean discrepancy has magnitude greater than $\varepsilon$, and the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) bounds the weighted sum of squared discrepancies below by the rectangle weight times its squared mean. This is the local increment in the [energy-increment proof of Szemerédi regularity](#energy-increment-proof-of-szemeredi-regularity).

#### Regular clique counting lemma

↑ **Parent:** [Regular pair of vertex sets](#regular-pair-of-vertex-sets)

For fixed $r$ and positive density threshold $\lambda$, sufficiently regular pairwise dense bipartite graphs between $r$ disjoint equal-sized vertex classes contain at least $\delta n^r$ transversal [cliques](graph-theory.md#clique-graph-theory), for some $\delta>0$. A greedy embedding maintains common neighbourhoods and discards the small set of vertices with atypical degrees into them. The constants depend only on $r,\lambda$.

##### Regular triangle counting lemma

↑ **Parent:** [Regular clique counting lemma](#regular-clique-counting-lemma)

If three disjoint [vertex](graph.md#vertex-graph-theory) classes have size $L$, and their three pairs are $\varepsilon$-[regular pairs of vertex sets](#regular-pair-of-vertex-sets) of [edge density of a bipartite graph](#edge-density-of-a-bipartite-graph) at least $d$, where $0<\varepsilon\leq d/2$ and $\varepsilon<1/2$, they contain at least the displayed number of transversal [triangles in a graph](graph.md#triangle-in-a-graph). All but $2\varepsilon L$ [vertices](graph.md#vertex-graph-theory) in the first class have at least $(d-\varepsilon)L$ neighbours in both other classes. Regularity between those two neighbour sets supplies the third [edge](graph-theory.md#edge-of-a-graph). This strengthens a mere [triangle embedding lemma for regular pairs](#triangle-embedding-lemma-for-regular-pairs) to a cubic lower count.

#### Regular pair of bipartite partitions

↑ **Parent:** [Regular pair of vertex sets](#regular-pair-of-vertex-sets)

Let $X=X_1\sqcup\cdots\sqcup X_r$ and $Y=Y_1\sqcup\cdots\sqcup Y_s$ be [set partitions](combinatorics.md#set-partition) of the two parts of a [bipartite graph](graph-theory.md#bipartite-graph). The pair of partitions is $\varepsilon$-regular when

$$
\sum_{(i,j):\,(X_i,Y_j)\text{ is not }\varepsilon\text{-regular}}|X_i||Y_j|
\leq\varepsilon|X||Y|.
$$

Thus a uniformly random pair in $X\times Y$ lies in an irregular cell pair with [probability](probability-theory.md#probability) at most $\varepsilon$.

<h5 id="bipartite-szemeredi-regularity-lemma">Bipartite Szemerédi regularity lemma</h5>

↑ **Parent:** [Regular pair of bipartite partitions](#regular-pair-of-bipartite-partitions)

For every $\varepsilon>0$ there is a positive [integer](number-theory.md#integer) $K(\varepsilon)$ such that every finite [bipartite graph](graph-theory.md#bipartite-graph) has an $\varepsilon$-regular pair of partitions with at most $K(\varepsilon)$ cells on each side.

To prove this, give $X\times Y$ the uniform [probability measure](probability-theory.md#probability-measure), let $f$ be the [indicator function](measure-theory.md#indicator-function) of the edge set, and for partitions $\mathcal P,\mathcal Q$ define their energy by

$$
\mathcal E(\mathcal P,\mathcal Q)
=\left\|\mathbb E(f\mid\mathcal P\otimes\mathcal Q)\right\|_2^2
=\sum_{i,j}\frac{|X_i||Y_j|}{|X||Y|}d(X_i,Y_j)^2.
$$

This [conditional expectation](measure-theory.md#conditional-expectation) is an [orthogonal projection](hilbert-space.md#orthogonal-projection), so $0\leq\mathcal E\leq\|f\|_2^2\leq1$. If the partitions are not $\varepsilon$-regular, choose witnesses $A_{ij}\subseteq X_i$ and $B_{ij}\subseteq Y_j$ in every irregular cell pair and refine each $X_i$ by all its $A_{ij}$ and each $Y_j$ by all its $B_{ij}$. The refined energy exceeds the old energy by

$$
\left\|\mathbb E(f\mid\mathcal P'\otimes\mathcal Q')-
\mathbb E(f\mid\mathcal P\otimes\mathcal Q)\right\|_2^2.
$$

On $A_{ij}\times B_{ij}$ the [absolute value function](real-analysis.md#absolute-value) of the mean of the difference is greater than $\varepsilon$, while this rectangle occupies at least an $\varepsilon^2$ fraction of $X_i\times Y_j$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) therefore contributes more than $\varepsilon^4|X_i||Y_j|/(|X||Y|)$ from that cell pair. Irregular pairs have total weight greater than $\varepsilon$, so every refinement raises the energy by more than $\varepsilon^5$. The process stops after at most $\lceil\varepsilon^{-5}\rceil$ refinements. If the current cell counts are $r,s$, the construction gives at most $r2^s,s2^r$ new cells, so a finite iterated bound depending only on $\varepsilon$ supplies $K(\varepsilon)$.

<h4 id="szemeredi-regularity-lemma">Szemerédi regularity lemma</h4>

↑ **Parent:** [Regular pair of vertex sets](#regular-pair-of-vertex-sets)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Szemerédi_regularity_lemma)

For every $\varepsilon>0$ and $m_0$ there are $M,n_0$ such that every graph on at least $n_0$ vertices has a partition

$$
V=V_0\sqcup V_1\sqcup\cdots\sqcup V_m,
$$

where $m_0\leq m\leq M$, $|V_0|\leq\varepsilon|V|$, the other parts have equal size, and all but at most $\varepsilon m^2$ pairs $(V_i,V_j)$ are $\varepsilon$-regular.

<h5 id="weighted-szemeredi-regularity-lemma">Weighted Szemerédi regularity lemma</h5>

↑ **Parent:** [Szemerédi regularity lemma](#szemeredi-regularity-lemma)

For every $\varepsilon>0$, all sufficiently large finite [graphs](graph.md) admit a [set partition](combinatorics.md#set-partition) into at most $M(\varepsilon)$ nonempty cells, each of size at most $\varepsilon n$, with the displayed ordered irregular-pair weight bound. Start with small cells. Use [regularity energy](#equitable-regularity-energy) including diagonal rectangles, refine simultaneously by the witness subsets of all [irregular pairs](#irregular-pair-of-vertex-sets), and apply the [refinement variance identity for regularity energy](#refinement-variance-identity-for-regularity-energy). Each failing round raises energy by more than $\varepsilon^5$, while energy lies in $[0,1]$. The recurrence $k\mapsto k2^k$ bounds the final cell count. Equitability is unnecessary for this weighted version.

###### Small-cell deletion in weighted regularity

↑ **Parent:** [Weighted Szemerédi regularity lemma](#weighted-szemeredi-regularity-lemma)

A partition with at most $M$ cells has at most $\varepsilon n$ vertices in cells smaller than $\varepsilon n/M$. Deleting all edges incident to those vertices costs at most $\varepsilon n^2$ edges. Every remaining cell has a fixed positive fraction of all vertices, which permits a [regular triangle counting lemma](#regular-triangle-counting-lemma) to give a cubic count without requiring equal cell sizes.

<h5 id="energy-increment-proof-of-szemeredi-regularity">Energy-increment proof of Szemerédi regularity</h5>

↑ **Parent:** [Szemerédi regularity lemma](#szemeredi-regularity-lemma)

Use [equitable regularity energy](#equitable-regularity-energy) with exceptional vertices retained as singleton cells. The [refinement variance identity for regularity energy](#refinement-variance-identity-for-regularity-energy) shows that splitting along an irregular pair's witnesses raises energy by more than $\varepsilon^4|V_i||V_j|/n^2$. More than $\varepsilon k^2$ irregular ordered pairs therefore raise energy by more than $\varepsilon^5/4$ when the exceptional set occupies at most half the vertices.

For [equalization with a controlled exceptional set](#equalization-with-a-controlled-exceptional-set), cut each of the at most $k2^k$ witness atoms into pieces of size $\lfloor L/4^k\rfloor$ and put leftovers into singleton exceptional cells. This is a refinement, so it cannot decrease energy. At most $n2^{-k}$ vertices are lost. Start with enough cells that this loss, over $\lceil4\varepsilon^{-5}\rceil$ rounds, is at most $\varepsilon n/2$; the initial exceptional set uses the other half. The number of cells grows by a bounded recurrence depending only on $\varepsilon$ and the prescribed minimum. Energy lies in $[0,1]$, so the process terminates.

##### Induced regularity template lemma

↑ **Parent:** [Szemerédi regularity lemma](#szemeredi-regularity-lemma)

For fixed forbidden induced patterns, a regularity and Ramsey refinement uses internal [clique](graph-theory.md#clique-graph-theory)/independent types and sparse, almost-complete, or intermediate cross pairs. A [clique](graph-theory.md#clique-graph-theory) of intermediate pairs realizes every bounded induced pattern consistent with those internal types, using both [edge](graph-theory.md#edge-of-a-graph) and nonedge regularity. This is the induced embedding consequence used in [hereditary graph enumeration theorem](graph-theory.md#hereditary-graph-enumeration-theorem); the exceptional-pair budget can be arbitrarily small.

##### Clique removal lemma

↑ **Parent:** [Szemerédi regularity lemma](#szemeredi-regularity-lemma)

For fixed $r\ge2$ and every $\varepsilon>0$, some $\delta>0$ has the following property for all sufficiently large $n$: a [graph](graph.md) with fewer than $\delta n^r$ copies of $K_r$ can be made $K_r$-free by deleting at most $\varepsilon n^2$ edges. A [Szemerédi regularity lemma](#szemeredi-regularity-lemma) partition and the [regular clique counting lemma](#regular-clique-counting-lemma) prove this. It converts sparse counts of a forbidden clique into a small edit distance from clique-freeness.

###### Triangle removal lemma

↑ **Parent:** [Clique removal lemma](#clique-removal-lemma)

For every $\eta>0$, some $\rho>0$ and $N_0$ have this property: a [graph](graph.md) on $N\geq N_0$ [vertices](graph.md#vertex-graph-theory) with fewer than $\rho N^3$ unordered [triangles in a graph](graph.md#triangle-in-a-graph) can be made [triangle-free](graph.md#triangle-free-graph) by deleting at most $\eta N^2$ [edges](graph-theory.md#edge-of-a-graph). A [Szemerédi regularity lemma](#szemeredi-regularity-lemma) partition deletes exceptional, intraclass, irregular and sparse-pair [edges](graph-theory.md#edge-of-a-graph) cheaply. A surviving [triangle in a graph](graph.md#triangle-in-a-graph) would force a positive cubic count by the [regular triangle counting lemma](#regular-triangle-counting-lemma).

##### Equitable regularity energy

↑ **Parent:** [Szemerédi regularity lemma](#szemeredi-regularity-lemma)

For a [set partition](combinatorics.md#set-partition) $\mathcal P$ of the [vertices](graph.md#vertex-graph-theory) of a [graph](graph.md) of order $n$, define

$$
q(\mathcal P)=\frac1{n^2}\sum_{A,B\in\mathcal P}|A||B|d(A,B)^2,
$$

where the sum is ordered, the adjacency indicator defines the density also on diagonal pairs, and exceptional [vertices](graph.md#vertex-graph-theory) are treated as singleton parts. Refinement cannot decrease this energy, by the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). An irregular pair of equal cells of size $m$, with witnesses of relative size at least $\varepsilon$ and density discrepancy greater than $\varepsilon$, increases the energy by more than $\varepsilon^4m^2/n^2$ for each orientation. Splitting refined atoms into equal chunks and leftover singleton parts is a further refinement, so restoring equitability causes no energy loss.

###### Equalization with a controlled exceptional set

↑ **Parent:** [Equitable regularity energy](#equitable-regularity-energy)

In a proof of the [Szemerédi regularity lemma](#szemeredi-regularity-lemma), suppose $k$ equal classes have size $L$ and witness splitting creates at most $2^k$ atoms per class. Divide every atom into blocks of size $\ell=\lfloor L/4^k\rfloor$, putting leftovers into the exceptional set. At most $k2^k\ell\leq kL2^{-k}$ [vertices](graph.md#vertex-graph-theory) are lost. When $L\geq2\cdot4^k$, at most $2k4^k$ blocks remain. For [equitable regularity energy](#equitable-regularity-energy) defined by omitting exceptional [vertices](graph.md#vertex-graph-theory), the loss from discarding a fraction $r$ is at most $2r$: only ordered pairs incident with discarded [vertices](graph.md#vertex-graph-theory) are removed, and every squared [edge density of a bipartite graph](#edge-density-of-a-bipartite-graph) is at most one. This provides a quantitative way to restore equal class sizes after each energy increment.

###### Refinement variance identity for regularity energy

↑ **Parent:** [Equitable regularity energy](#equitable-regularity-energy)

If a [set partition](combinatorics.md#set-partition) refines a rectangle $U\times V$ of a [graph](graph.md) into rectangles $U_a\times V_b$, write $d=d(U,V)$ for its [edge density of a bipartite graph](#edge-density-of-a-bipartite-graph). The weighted [variance](variance.md) identity is

$$
\sum_{a,b}|U_a||V_b|d(U_a,V_b)^2-|U||V|d^2
=\sum_{a,b}|U_a||V_b|\bigl(d(U_a,V_b)-d\bigr)^2.
$$

It follows by expanding the square and using $\sum_{a,b}|U_a||V_b|d(U_a,V_b)=|U||V|d$. In particular, [equitable regularity energy](#equitable-regularity-energy) cannot decrease under refinement. If a witness rectangle has relative sizes at least $\varepsilon$ and [edge density of a bipartite graph](#edge-density-of-a-bipartite-graph) discrepancy greater than $\varepsilon$, its contribution, after division by the squared total [vertex](graph.md#vertex-graph-theory) count, exceeds $\varepsilon^4|U||V|/N^2$.

#### Graph embedding lemma for regular pairs

↑ **Parent:** [Regular pair of vertex sets](#regular-pair-of-vertex-sets)

For every finite graph $H$ and density $\delta>0$, sufficiently large vertex classes joined according to $H$ by regular pairs of density at least $\delta$ contain a copy of $H$. The regularity parameter must be sufficiently small in terms of $H$ and $\delta$.

##### Odd-cycle copies from positive triangle density

↑ **Parent:** [Graph embedding lemma for regular pairs](#graph-embedding-lemma-for-regular-pairs)

For any fixed odd length $\ell\ge3$, positive [triangle in a graph](graph.md#triangle-in-a-graph) density forces positive density of $\ell$-cycles. A [Szemerédi regularity lemma](#szemeredi-regularity-lemma) partition retains a [triangle in a graph](graph.md#triangle-in-a-graph) of regular dense pairs after the sparse and exceptional pairs are removed. Count embeddings of a proper three-colouring of $C_\ell$ into those three clusters. The constants depend on $\beta$ and $\ell$, not on [graph](graph.md) order.

##### Triangle embedding lemma for regular pairs

↑ **Parent:** [Graph embedding lemma for regular pairs](#graph-embedding-lemma-for-regular-pairs)

If the three pairs among vertex sets $A,B,C$ are $\varepsilon$-regular and each has density at least $2\varepsilon$, where $0<\varepsilon<1/2$, then the graph contains a triangle with one vertex in each set.

#### Reduced graph of a regularity partition

↑ **Parent:** [Regular pair of vertex sets](#regular-pair-of-vertex-sets)

Given a regularity partition and a density cutoff $\delta$, its reduced graph has one vertex for each nonexceptional class and joins two classes when their pair is regular and has density at least $\delta$.

<h2 id="szemeredi-s-theorem">Szemerédi's theorem</h2>

↑ **Parent:** [Probabilistic combinatorics](probabilistic-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Szemerédi's_theorem)

For every positive density $\alpha$ and positive integer $r$, every sufficiently large subset of $[n]$ of size at least $\alpha n$ contains a nonconstant arithmetic progression of length $r$.

### Dense three-term progressions force four-term progressions

↑ **Parent:** [Szemerédi's theorem](#szemeredi-s-theorem)

For every $c>0$, all sufficiently large finite integer sets $A$ with at least $c|A|^2$ ordered three-term [arithmetic progressions](arithmetic.md#arithmetic-progression) contain a nonconstant four-term [arithmetic progression](arithmetic.md#arithmetic-progression). [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $E(A)\ge c^2|A|^3$. The [Balog-Szemerédi-Gowers theorem](additive-combinatorics.md#balog-szemeredi-gowers-theorem) supplies a large small-doubling subset. A bounded-modulus [Freiman 2-isomorphism](additive-combinatorics.md#freiman-2-isomorphism) gives a positive-density cyclic model; apply the assumed four-term case of [Szemerédi's theorem](#szemeredi-s-theorem) to representatives, then lift the two consecutive second-difference relations.

## Locally dense graph thinning lemma

↑ **Parent:** [Probabilistic combinatorics](probabilistic-combinatorics.md)

For every $\varepsilon>0$ there is $\delta>0$ such that a graph satisfying $e(A,B)\geq p|A||B|$ whenever $|A|,|B|\geq\delta n$, with $p\geq\delta$, has a spanning subgraph $G'$ satisfying

$$
|e_{G'}(A,B)-p|A||B||\leq\varepsilon n^2
$$

for all disjoint $A,B$. Partition into a fixed large number of nearly equal parts, independently thin each cross-pair to expected density $p$, and apply a concentration inequality and a union bound over all pairs $A,B$.

## Minimum-degree Ramsey lower bound

↑ **Parent:** [Probabilistic combinatorics](probabilistic-combinatorics.md)

If a graph $H$ has [minimum degree](graph-theory.md#minimum-degree-of-a-graph) $d$, then its [graph Ramsey number](graph-theory.md#graph-ramsey-number) satisfies $R(H)\geq2^{d/2}$. The probabilistic proof chooses a red-blue edge colouring and applies the local lemma to its monochromatic copies of $H$.

## ↑ Ancestors (5)

1. [Graph theory](graph-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)
