# Random graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Random_graph)

A random graph is a graph sampled from a probability distribution on graphs.

**Table of contents**

- [Watts-Strogatz model](#watts-strogatz-model)
- [Configuration model](#configuration-model)
  - [Bounded-degree pairing avoidance estimate](#bounded-degree-pairing-avoidance-estimate)
  - [Half-edge of a graph](#half-edge-of-a-graph)
- [Preferential attachment](#preferential-attachment)
  - [Barabási-Albert model](#barabasi-albert-model)
  - [Linearized chord diagram model](#linearized-chord-diagram-model)
    - [First-vertex degree in the LCD model](#first-vertex-degree-in-the-lcd-model)
    - [Uniform linearized chord diagram](#uniform-linearized-chord-diagram)
- [Random k-out graph](#random-k-out-graph)
  - [Connectivity of random k-out graphs](#connectivity-of-random-k-out-graphs)
- [Rado graph](#rado-graph)
- [Achlioptas process](#achlioptas-process)
  - [Continuity of fixed-choice percolation](#continuity-of-fixed-choice-percolation)
  - [Persistence of unsampled graph components](#persistence-of-unsampled-graph-components)
  - [Forced merging of large components](#forced-merging-of-large-components)
  - [Component-band vertex count](#component-band-vertex-count)
- [Simultaneous giant for fixed random-edge choice](#simultaneous-giant-for-fixed-random-edge-choice)
- [Giant component](#giant-component)
  - [Barely-supercritical largest-component expectation](#barely-supercritical-largest-component-expectation)
  - [Logarithmic-regime giant component](#logarithmic-regime-giant-component)
- [Isolated vertex](#isolated-vertex)
- [Erdős-Rényi model](#erdos-renyi-model)
  - [Breadth-first exploration of a binomial random graph](#breadth-first-exploration-of-a-binomial-random-graph)
  - [Uniform random graph process](#uniform-random-graph-process)
    - [Connectivity hitting time equals disappearance of isolated vertices](#connectivity-hitting-time-equals-disappearance-of-isolated-vertices)
    - [Marked-set connectivity threshold](#marked-set-connectivity-threshold)
  - [Tree-component expectation in the Erdős-Rényi model](#tree-component-expectation-in-the-erdos-renyi-model)
    - [Fixed-order tree-component window](#fixed-order-tree-component-window)
  - [Monotone graph property](#monotone-graph-property)
    - [Threshold function for a monotone graph property](#threshold-function-for-a-monotone-graph-property)
    - [Monotone coupling of binomial random graphs](#monotone-coupling-of-binomial-random-graphs)
  - [Sprinkling of a binomial random graph](#sprinkling-of-a-binomial-random-graph)
  - [Isolated vertices in the Erdős-Rényi model](#isolated-vertices-in-the-erdos-renyi-model)
    - [Isolated-vertex threshold in the Erdős-Rényi model](#isolated-vertex-threshold-in-the-erdos-renyi-model)
  - [Connectivity threshold in the Erdős-Rényi model](#connectivity-threshold-in-the-erdos-renyi-model)
    - [Connectivity of a fixed-density binomial random graph](#connectivity-of-a-fixed-density-binomial-random-graph)
    - [Critical-window connectivity probability of a binomial random graph](#critical-window-connectivity-probability-of-a-binomial-random-graph)
  - [Expected subgraph count in the Erdős-Rényi model](#expected-subgraph-count-in-the-erdos-renyi-model)
    - [Sparse clique-count concentration](#sparse-clique-count-concentration)
      - [Pendant extensions of sparse clique copies](#pendant-extensions-of-sparse-clique-copies)
    - [Vertex-disjoint sparse clique copies](#vertex-disjoint-sparse-clique-copies)

## Watts-Strogatz model

↑ **Parent:** [Random graph](random-graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Watts–Strogatz_model)

## Configuration model

↑ **Parent:** [Random graph](random-graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Configuration_model)

For a prescribed [degree sequence](graph-theory.md#degree-sequence) with even sum $M=\sum_i d_i$, attach $d_i$ labelled [half-edges](#half-edge-of-a-graph) to [vertex](graph.md#vertex-graph-theory) $i$ and choose a uniform [perfect matching](matching-graph-theory.md#perfect-matching) of the $M$ half-edges. Each pair becomes an [edge](graph-theory.md#edge-of-a-graph), giving a [multigraph](graph.md#multigraph) that may have [self-loops](graph.md#loop-graph-theory) or parallel edges. The number of pairings is $M!/[2^{M/2}(M/2)!]$. Every [simple graph](graph.md#simple-graph) with that degree sequence has exactly $\prod_i d_i!$ pairing representations, so conditioning on simplicity produces the uniform simple-graph model.

### Bounded-degree pairing avoidance estimate

↑ **Parent:** [Configuration model](#configuration-model)

For bounded [vertex degrees](graph-theory.md#degree-graph-theory), total degree $M\to\infty$, and a forbidden graph $G_0$ of bounded [maximum degree](graph-theory.md#maximum-degree), put $\lambda=M^{-1}\sum_i d_i(d_i-1)$ and $\mu=M^{-1}\sum_{ij\in E(G_0)}d_i d_j$. Count prescribed loop pairs, double-edge pairs, and forbidden-edge pairs in the [configuration model](#configuration-model). Their means are respectively $\lambda/2+o(1)$, $\lambda^2/4+o(1)$, and $\mu+o(1)$. A fixed collection of $t$ disjoint prescribed pairs occurs with probability $[(M-1)(M-3)\cdots(M-2t+1)]^{-1}$. Bounded degrees make intersecting bad configurations contribute $O(M^{-1})$ to each fixed [factorial moment](continuous-time-markov-chain.md#factorial-moment). Thus the total bad-pattern count has factorial moments $(\lambda/2+\lambda^2/4+\mu)^j+o(1)$. The [Bonferroni inequalities](combinatorics.md#bonferroni-inequalities) and uniformly bounded means give the displayed zero-pattern probability, without requiring the parameters to converge.

### Half-edge of a graph

↑ **Parent:** [Configuration model](#configuration-model)

A half-edge records an incidence of an [edge](graph-theory.md#edge-of-a-graph) at a [vertex](graph.md#vertex-graph-theory). Two half-edges form each edge, including two incidences at the same vertex for a [self-loop](graph.md#loop-graph-theory). In the [configuration model](#configuration-model) these incidences are individually labelled before random pairing.

## Preferential attachment

↑ **Parent:** [Random graph](random-graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Preferential_attachment)

In preferential attachment, new [edges](graph-theory.md#edge-of-a-graph) favour existing [vertices](graph.md#vertex-graph-theory) in proportion to a prescribed attractiveness, often their current [degree of a vertex](graph-theory.md#degree-graph-theory). A complete model must specify initial conditions, [self-loop](graph.md#loop-graph-theory) conventions and the normalization at each attachment. These details matter for the [vertex degree](graph-theory.md#degree-graph-theory) distribution of the earliest [vertices](graph.md#vertex-graph-theory).

<h3 id="barabasi-albert-model">Barabási-Albert model</h3>

↑ **Parent:** [Preferential attachment](#preferential-attachment)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Barabási–Albert_model)

### Linearized chord diagram model

↑ **Parent:** [Preferential attachment](#preferential-attachment)

Start with one [self-loop](graph.md#loop-graph-theory), and at step $t$ add one [vertex](graph.md#vertex-graph-theory) and one [edge](graph-theory.md#edge-of-a-graph). An old [vertex](graph.md#vertex-graph-theory) $i$ is chosen with [probability](probability-theory.md#probability) $d_i(t-1)/(2t-1)$, and the new [vertex](graph.md#vertex-graph-theory) is chosen with [probability](probability-theory.md#probability) $1/(2t-1)$, producing a [self-loop](graph.md#loop-graph-theory). [Self-loops](graph.md#loop-graph-theory) contribute two to the [degree of a vertex](graph-theory.md#degree-graph-theory). There are $n$ [edges](graph-theory.md#edge-of-a-graph) and total [vertex degree](graph-theory.md#degree-graph-theory) $2n$ at time $n$. This exact normalization is distinct from treating the total [vertex degree](graph-theory.md#degree-graph-theory) as the number of [edges](graph-theory.md#edge-of-a-graph).

#### First-vertex degree in the LCD model

↑ **Parent:** [Linearized chord diagram model](#linearized-chord-diagram-model)

In a [uniform linearized chord diagram](#uniform-linearized-chord-diagram), $\Pr(\sqrt nR_1\ge x)=(1-x^2/n)^n\to e^{-x^2}$. Conditional on the right endpoints, $d_1(n)=2+\sum_{i=2}^n\mathbf1_{\{L_i\le R_1\}}$, with [independent](random-variable.md#independent-random-variables) success [probabilities](probability-theory.md#probability) $R_1/R_i$. A [Chernoff bound](probability-inequality.md#chernoff-bound) gives $R_i=(1+o(1))\sqrt{i/n}$ uniformly for $i\ge n^{1/10}$. The early indicators are $o(\sqrt n)$, and the remaining conditional [mean](expected-value.md) is $(2+o(1))nR_1$. Their conditional [variance](variance.md) is $O_{\mathbb P}(\sqrt n)$. Hence $d_1(n)/\sqrt n-2\sqrt nR_1\to0$ in [probability](probability-theory.md#probability), proving the displayed tail limit. A [self-loop](graph.md#loop-graph-theory)'s contribution is included in the constant two.

#### Uniform linearized chord diagram

↑ **Parent:** [Linearized chord diagram model](#linearized-chord-diagram-model)

Pair $2n$ linearly ordered endpoints uniformly. Each pair is a chord; its larger endpoint ends a [vertex](graph.md#vertex-graph-theory) block, with all endpoints after the previous right endpoint merged into that [vertex](graph.md#vertex-graph-theory). Orient the chord from its right-endpoint block to its left-endpoint block. Removing the last endpoint and its mate leaves a uniform smaller pairing. Reinserting the mate into one of $2n-1$ equally likely gaps chooses an existing block proportionally to its endpoint count, or the final gap creates a [self-loop](graph.md#loop-graph-theory). This proves equivalence with the [linearized chord diagram model](#linearized-chord-diagram-model).

An equivalent continuous representation draws $n$ [independent](random-variable.md#independent-random-variables) pairs of [independent](random-variable.md#independent-random-variables) uniform points on $[0,1]$, orders the pairs by their maxima $R_1<\cdots<R_n$, and calls their minima $L_i$. The $R_i^2$ are [uniform order statistics](probability-theory.md#uniform-order-statistic); conditional on all the $R_i$, the $L_i$ are [independent](random-variable.md#independent-random-variables) uniform points on $[0,R_i]$.

## Random k-out graph

↑ **Parent:** [Random graph](random-graph.md)

Each [vertex](graph.md#vertex-graph-theory) independently chooses $k$ distinct other [vertices](graph.md#vertex-graph-theory) uniformly, and an undirected [edge](graph-theory.md#edge-of-a-graph) exists when either endpoint chooses the other. This has dependent undirected [edges](graph-theory.md#edge-of-a-graph) and is not a [binomial random graph](graph-theory.md#binomial-random-graph). Coupling the choices as the first $k$ entries of [independent](random-variable.md#independent-random-variables) random permutations makes the [graphs](graph.md) increasing in $k$.

### Connectivity of random k-out graphs

↑ **Parent:** [Random k-out graph](#random-k-out-graph)

For $k=2$, a disconnected [graph](graph.md) has a component of size $3\le s\le n/2$. The [probability](probability-theory.md#probability) that a fixed $s$-set has no crossing [edge](graph-theory.md#edge-of-a-graph) is at most $(s/n)^{2s}(1-s/n)^{2(n-s)}$. The [union bound](probability-inequality.md#boole-s-inequality) and $\binom ns\le(n/s)^s[n/(n-s)]^{n-s}$ bound the failure [probability](probability-theory.md#probability) by $\sum_{s=3}^{\lfloor n/2\rfloor}(s/n)^s=o(1)$. Split this sum at $\sqrt n$. The [random k-out graph](#random-k-out-graph) coupling extends the result to every fixed $k\ge2$.

## Rado graph

↑ **Parent:** [Random graph](random-graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rado_graph)

The Rado graph is the unique countably infinite [graph](graph.md) with the two-uniform [hypergraph extension property](hypergraph.md#hypergraph-extension-property). Equivalently, for any disjoint finite vertex sets $U,W$, some new vertex is adjacent to every member of $U$ and no member of $W$. The [back-and-forth method](model-theory.md#back-and-forth-method) proves uniqueness. Independent edge sampling on the [natural numbers](arithmetic.md#natural-number) with any fixed $p\in(0,1)$ produces this graph [almost surely](convergence-of-random-variables.md#almost-sure-convergence). It contains both edges and nonedges and therefore is not a [complete graph](graph-theory.md#complete-graph). Its first-order axioms constitute the [theory of the random graph](model-theory.md#theory-of-the-random-graph).

## Achlioptas process

↑ **Parent:** [Random graph](random-graph.md)

At each step offer a fixed number of independent uniform candidate [edges](graph-theory.md#edge-of-a-graph) on a fixed vertex set, and let a rule select one. The standard two-choice model offers two candidates. The rule may depend on the entire previously exposed history. Repeated already present [edges](graph-theory.md#edge-of-a-graph) make no change in the independent-candidate version; another usual version offers only absent [edges](graph-theory.md#edge-of-a-graph). The [forced merging of large components](#forced-merging-of-large-components) and [persistence of unsampled graph components](#persistence-of-unsampled-graph-components) apply to both over a linear number of steps. Fixed choice is essential in the [continuity of fixed-choice percolation](#continuity-of-fixed-choice-percolation) argument.

### Continuity of fixed-choice percolation

↑ **Parent:** [Achlioptas process](#achlioptas-process)

A fixed-choice [Achlioptas process](#achlioptas-process) cannot have its [largest component of a graph](graph.md#largest-component-of-a-graph) jump from $o(n)$ to a fixed positive fraction of $n$ within $o(n)$ steps, [with high probability](probabilistic-combinatorics.md#with-high-probability). The proof combines [forced merging of large components](#forced-merging-of-large-components) and [persistence of unsampled graph components](#persistence-of-unsampled-graph-components). An assumed jump forces positive vertex mass in each band $[k,Dk)$ slightly before the jump: insufficient smaller components can feed the final large component, while enough components above $Dk$ would merge too early. Persistence carries a fixed positive amount of each band to a common time. Taking sufficiently many disjoint bands with $k=1,D,D^2,\ldots$ then counts more than $n$ [vertices](graph.md#vertex-graph-theory). The number of offered candidates is fixed throughout this argument. Riordan and Warnke establish this obstruction and broader continuity results in [their original research paper](https://arxiv.org/abs/1102.5306).

### Persistence of unsampled graph components

↑ **Parent:** [Achlioptas process](#achlioptas-process)

Fix positive $\alpha$, $D\geq2$ and $B>0$. Suppose a size band $[k,Dk)$ of an [Achlioptas process](#achlioptas-process) contains at least $\alpha n$ [vertices](graph.md#vertex-graph-theory) at time $m$. For every fixed $k$, at least $\beta n$ of those [vertices](graph.md#vertex-graph-theory) remain in unchanged [graph components](graph.md#component-graph-theory) throughout the next $T=\lceil Bn/k\rceil$ steps, [with high probability](probabilistic-combinatorics.md#with-high-probability), where one may take $\beta=\alpha e^{-16BD}/4$. This is a deliberately nonoptimal positive constant.

For independent uniform candidate [edges](graph-theory.md#edge-of-a-graph), an initial [graph component](graph.md#component-graph-theory) with $w<Dk$ [vertices](graph.md#vertex-graph-theory) is untouched if none of the $2T$ candidate [edges](graph-theory.md#edge-of-a-graph) meets it. A uniform [edge](graph-theory.md#edge-of-a-graph) hits it with [probability](probability-theory.md#probability) at most $3w/n$. For sufficiently large $n$, $(1-3w/n)^{2T}\geq e^{-16BD}$, so the [expected value](expected-value.md) of the untouched vertex mass $Y$ is at least $\alpha e^{-16BD}n$. Replacing one row of two candidate [edges](graph-theory.md#edge-of-a-graph) can change $Y$ by at most $8Dk$, because only the initial [graph components](graph.md#component-graph-theory) hit by an old or new endpoint can change status. The [McDiarmid inequality](probability-inequality.md#mcdiarmid-s-inequality) therefore makes $Y\geq\alpha e^{-16BD}n/2$ except on an event of [probability](probability-theory.md#probability) $e^{-c n/k}$, for a positive constant $c$ depending only on $\alpha,B,D$. An untouched [graph component](graph.md#component-graph-theory) stays unchanged whichever offered [edge](graph-theory.md#edge-of-a-graph) is selected.

For candidates restricted to absent [edges](graph-theory.md#edge-of-a-graph), generate each by an independent uniform proposal stream and reject already present [edges](graph-theory.md#edge-of-a-graph). During any interval of $O(n)$ steps with $O(n)$ present [edges](graph-theory.md#edge-of-a-graph), each proposal has rejection [probability](probability-theory.md#probability) $O(1/n)$ conditional on the past. The number of rejections is at most $O(\log n)$ except on an event of [probability](probability-theory.md#probability) smaller than any inverse power of $n$: if there were $r$ rejections among $2T+r$ proposals, a [union bound](probability-inequality.md#boole-s-inequality) over their positions bounds this by $\binom{2T+r}r(C/n)^r$. The first $2T$ proposals are independent and give the previous untouched-mass estimate. Extra proposals can touch at most $2r$ additional initial [graph components](graph.md#component-graph-theory), losing only $O(Dk\log n)=o(n)$ [vertices](graph.md#vertex-graph-theory) for fixed $k$. This leaves the stated $\beta n$ bound. A [union bound](probability-inequality.md#boole-s-inequality) makes these estimates simultaneous over starting times $m\leq3n$. They hold through the entire interval, so deterministic or random stopping times within it are allowed.

### Forced merging of large components

↑ **Parent:** [Achlioptas process](#achlioptas-process)

For the two-choice [Achlioptas process](#achlioptas-process), fix $a>0$ and $K\geq1$. Conditional on any current [graph](graph.md) with $N_{\geq K}\geq an$, put $W$ equal to the [vertices](graph.md#vertex-graph-theory) in its large [graph components](graph.md#component-graph-theory). There are at most $n/K$ such initial [graph components](graph.md#component-graph-theory). If after $s$ more steps no [graph component](graph.md#component-graph-theory) contains $an/3$ [vertices](graph.md#vertex-graph-theory) of $W$, greedily assign final [graph components](graph.md#component-graph-theory) to two groups so that each meets at least $|W|/3\geq an/3$ [vertices](graph.md#vertex-graph-theory) of $W$. This induces a [set partition](combinatorics.md#set-partition) of the initial large [graph components](graph.md#component-graph-theory), of which there are at most $2^{n/K}$ possibilities.

For any fixed such split $W=A\cup B$, a uniform candidate [edge](graph-theory.md#edge-of-a-graph) joins $A$ to $B$ with [probability](probability-theory.md#probability) at least $2a^2/9$. If both candidates do so, the selected [edge](graph-theory.md#edge-of-a-graph) cannot avoid the crossing. Thus the [probability](probability-theory.md#probability) that the split survives all $s$ steps is at most $(1-a^4/81)^s$. The deliberately weaker constant also covers distinct candidate sampling for sufficiently large $n$. In the absent-edge version, as long as the split has survived, every $A$--$B$ [edge](graph-theory.md#edge-of-a-graph) is absent, so conditioning on absence can only increase this crossing [probability](probability-theory.md#probability). A [union bound](probability-inequality.md#boole-s-inequality) with $s=\lceil A(a)n/K\rceil$ and $A(a)=81(\log2+2)/a^4$ bounds failure by $e^{-2n/K}$. For fixed $K$, a further [union bound](probability-inequality.md#boole-s-inequality) makes the conclusion simultaneous over all starting steps $m\leq3n$. This proof is independent of how the rule chooses between the two candidates.

### Component-band vertex count

↑ **Parent:** [Achlioptas process](#achlioptas-process)

This is the total number of [vertices](graph.md#vertex-graph-theory) in [graph components](graph.md#component-graph-theory) with orders in the specified half-open interval. It differs from the number of those [graph components](graph.md#component-graph-theory). Write $N_{\geq k}$ for the total above the lower endpoint. Then $N_{[k,\ell)}=N_{\geq k}-N_{\geq\ell}$. Disjoint size bands count disjoint sets of [vertices](graph.md#vertex-graph-theory) at a common time, even though their mass may move between bands as an [Achlioptas process](#achlioptas-process) adds [edges](graph-theory.md#edge-of-a-graph).

## Simultaneous giant for fixed random-edge choice

↑ **Parent:** [Random graph](random-graph.md)

Offer $k$ independent uniform [edges](graph-theory.md#edge-of-a-graph) of the [complete graph](graph-theory.md#complete-graph) per row and permit any one to be selected from each row. If a chosen [graph](graph.md) has no [graph component](graph.md#component-graph-theory) of order at least $2n/3$, the [balanced component cut](graph.md#balanced-component-cut) provides an empty cut whose sides both have at least $n/3$ [vertices](graph.md#vertex-graph-theory). Each candidate [edge](graph-theory.md#edge-of-a-graph) crosses that cut with [probability](probability-theory.md#probability) at least $4/9$, so a row can avoid crossing with [probability](probability-theory.md#probability) at most $1-(4/9)^k$. The [union bound](probability-inequality.md#boole-s-inequality) over at most $2^n$ cuts gives failure probability at most $2^n[1-(4/9)^k]^{cn}$. Any fixed integer $c$ with $c[-\log(1-(4/9)^k)]>\log2$ suffices. The guarantee is simultaneous even for choices made after seeing every offered [edge](graph-theory.md#edge-of-a-graph).

## Giant component

↑ **Parent:** [Random graph](random-graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Giant_component)

A giant component in a sequence of [random graphs](random-graph.md) on $n$ [vertices](graph.md#vertex-graph-theory) has order proportional to $n$. Its existence can change at a [threshold function for a monotone graph property](#threshold-function-for-a-monotone-graph-property). A [giant component](#giant-component) need not contain every [vertex](graph.md#vertex-graph-theory), and its uniqueness requires proof for the model in question.

### Barely-supercritical largest-component expectation

↑ **Parent:** [Giant component](#giant-component)

Suppose $\varepsilon=o(1)$ and $\varepsilon\geq n^{-1/6}$. The [breadth-first exploration of a binomial random graph](#breadth-first-exploration-of-a-binomial-random-graph) has deterministic drift $F(t)=\varepsilon t-t^2/(2n)+O(\varepsilon^3n+\varepsilon)$ up to $3\varepsilon n$ steps. Its weighted [martingale](martingale.md) has [variance](variance.md) $O(\varepsilon n)$. For $h=\sqrt\varepsilon+(n\varepsilon^3)^{-1/8}$, the [Doob L2 maximal inequality](martingale.md#doob-l2-maximal-inequality) makes its maximum smaller than $h\varepsilon^2n/6$ [with high probability](probabilistic-combinatorics.md#with-high-probability). Then $A_t>0$ throughout $[h\varepsilon n,(2-h)\varepsilon n]$, giving a [graph component](graph.md#component-graph-theory) of order $(2-o(1))\varepsilon n$.

For the upper expectation bound, let $K=\lceil\varepsilon^{-3}\rceil$. The dominating [binomial branching process](galton-watson-process.md#binomial-branching-process) has [branching survival probability](galton-watson-process.md#survival-probability-of-a-branching-process) $(2+o(1))\varepsilon$ by the [binomial branching survival correction](galton-watson-process.md#binomial-branching-survival-correction). Its [branching process conditioned on extinction](galton-watson-process.md#branching-process-conditioned-on-extinction) has mean $1-\varepsilon+O(\varepsilon^2+\varepsilon/n)$ and total-progeny [expected value](expected-value.md) $O(1/\varepsilon)$. Therefore $\mathbb EN_{\geq K}\leq n\rho+O(n/(\varepsilon K))$. Since $L_1\leq K+N_{\geq K}$ and $K=o(\varepsilon n)$, this yields the matching upper bound. Controlling rare large components is necessary to conclude an [expected value](expected-value.md) asymptotic from a typical-size statement.

### Logarithmic-regime giant component

↑ **Parent:** [Giant component](#giant-component)

Fix $k\geq1$, $\gamma_0>1/(k+1)$, and $\gamma_0\leq\gamma\leq1-\omega(n)/\log n$ with $\omega(n)\to\infty$. A [binomial random graph](graph-theory.md#binomial-random-graph) has one [giant component](#giant-component) of the displayed order and all other [graph components](graph.md#component-graph-theory) are [tree components](graph.md#tree-component) of orders at most $k$, [with high probability](probabilistic-combinatorics.md#with-high-probability). The [expected value](expected-value.md) and [variance](variance.md) of the [isolated vertex](#isolated-vertex) count concentrate it around $n^{1-\gamma}\to\infty$. A [Cayley formula](tree-graph-theory.md#cayley-s-formula) upper bound for connected sets excludes component sizes $k+1$ through a small fixed fraction of $n$; the empty-[graph cut](graph.md#graph-cut) bound excludes the remaining sizes up to $n/2$. An extra-[edge](graph-theory.md#edge-of-a-graph) count excludes cyclic small [graph components](graph.md#component-graph-theory). The [expected value](expected-value.md) of the number of [vertices](graph.md#vertex-graph-theory) in small nonisolated [tree components](graph.md#tree-component) is $O(n d e^{-2d})=o(n e^{-d})$, where $d=np$. The [Markov inequality](probability-inequality.md#markov-s-inequality) completes the count of [vertices](graph.md#vertex-graph-theory) outside the unique large [graph component](graph.md#component-graph-theory).

## Isolated vertex

↑ **Parent:** [Random graph](random-graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isolated_vertex)

An isolated vertex has degree zero.

<h2 id="erdos-renyi-model">Erdős-Rényi model</h2>

↑ **Parent:** [Random graph](random-graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Erdős–Rényi_model)

In the $G(n,p)$ model, each of the $\binom n2$ possible edges is included independently with probability $p$.

### Breadth-first exploration of a binomial random graph

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

During [breadth-first search](tree-graph-theory.md#breadth-first-search) of $G(n,p)$ let $U_t$ count unseen [vertices](graph.md#vertex-graph-theory), $A_t$ active [vertices](graph.md#vertex-graph-theory), and $t$ explored [vertices](graph.md#vertex-graph-theory). When $A_{t-1}=0$ start a new unseen root, recorded by $b_t=1$; otherwise $b_t=0$. The newly discovered count is conditionally $\operatorname{Bin}(U_{t-1}-b_t,p)$. Subtract its conditional mean to obtain a [martingale difference](martingale.md#martingale-difference) $D_t$. With $q=1-p$, $U_0=n$ and $A_0=0$, iteration gives

$$
A_t=n-t-nq^t+\sum_{j\leq t}q^{t-j+1}b_j+q^t\sum_{j\leq t}q^{-j}D_j.
$$

The last sum is a [martingale](martingale.md). Positive $A_t$ over an interval means that the [graph component](graph.md#component-graph-theory) under exploration does not finish there. Independently adding phantom children couples each component exploration below a [binomial branching process](galton-watson-process.md#binomial-branching-process) with offspring law $\operatorname{Bin}(n,p)$.

### Uniform random graph process

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

Start with the empty [graph](graph.md) and reveal the [edges](graph-theory.md#edge-of-a-graph) of the [complete graph](graph-theory.md#complete-graph) in a uniformly random order. After $m$ steps its edge set is a uniform $m$-element subset. Independent uniform edge labels couple this process with all [binomial random graphs](graph-theory.md#binomial-random-graph): $G(n,p)=G_{n,M(p)}$, where $M(p)$ has a [binomial distribution](discrete-probability-distribution.md#binomial-distribution) with parameters $\binom n2,p$. For a [monotone graph property](#monotone-graph-property), concentration of $M(p)$ transfers a threshold estimate between edge probability and edge count.

#### Connectivity hitting time equals disappearance of isolated vertices

↑ **Parent:** [Uniform random graph process](#uniform-random-graph-process)

Couple the process with independent uniform edge labels, and expose $p_-=(\log n-\frac14\log\log n)/n$. A spanning-tree [union bound](probability-inequality.md#boole-s-inequality) excludes components of orders $2$ through $n/\log n$, and a cut bound excludes orders up to $n/2$. The graph has one large component and at most $\log n$ isolated vertices, with at least one isolated vertex. Before $p_+=(\log n+\frac14\log\log n)/n$, the probability of any new edge between those isolated vertices is $O((\log n)^2\log\log n/n)=o(1)$. All have joined the large component by $p_+$ by the [isolated-vertex threshold in the Erdős-Rényi model](#isolated-vertex-threshold-in-the-erdos-renyi-model). Throughout this window the only obstruction to connectivity is an isolated vertex, establishing the equality of hitting times.

#### Marked-set connectivity threshold

↑ **Parent:** [Uniform random graph process](#uniform-random-graph-process)

For a fixed set $L$ of $\lfloor\sqrt n\rfloor$ [vertices](graph.md#vertex-graph-theory), let $\tau_L$ be the first step at which they all belong to one [graph component](graph.md#component-graph-theory). In the [uniform random graph process](#uniform-random-graph-process), $\tau_L$ lies between $n(\log n-\omega)/4$ and $n(\log n+\omega)/4$ [with high probability](probabilistic-combinatorics.md#with-high-probability) for every $\omega\to\infty$. Below that scale the marked [isolated vertex](#isolated-vertex) count has divergent [expected value](expected-value.md) and small relative [variance](variance.md). Above it the [logarithmic-regime giant component](#logarithmic-regime-giant-component) misses $o(\sqrt n)$ [vertices](graph.md#vertex-graph-theory); [exchangeability](probability-distribution.md#exchangeable-random-variables) and a [union bound](probability-inequality.md#boole-s-inequality) show that none are marked. The label coupling then transfers the two assertions to the process.

<h3 id="tree-component-expectation-in-the-erdos-renyi-model">Tree-component expectation in the Erdős-Rényi model</h3>

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

For $X_j$ the number of [tree components](graph.md#tree-component) of order $j$ in a [binomial random graph](graph-theory.md#binomial-random-graph), choose their [vertices](graph.md#vertex-graph-theory), choose one of $j^{j-2}$ labelled [trees](tree-graph-theory.md) by the [Cayley formula](tree-graph-theory.md#cayley-s-formula), require its $j-1$ [edges](graph-theory.md#edge-of-a-graph), and exclude both the remaining internal [edges](graph-theory.md#edge-of-a-graph) and all crossing [edges](graph-theory.md#edge-of-a-graph). For $j=1$ interpret $j^{j-2}=1$, recovering the [isolated vertex](#isolated-vertex) count. If $p=\lambda/n$ for fixed positive $\lambda$ and $j=O(\log n)$, the [Stirling formula](real-analysis.md#stirling-formula) gives $\mathbb EX_j\sim n(\lambda e^{1-\lambda})^j/(\lambda\sqrt{2\pi}\,j^{5/2})$. Distinct overlapping vertex sets cannot both be [graph components](graph.md#component-graph-theory); for disjoint sets their joint occurrence gains the factor $(1-p)^{-j^2}$ relative to the product, because their between-set [edges](graph-theory.md#edge-of-a-graph) must be absent only once.

#### Fixed-order tree-component window

↑ **Parent:** [Tree-component expectation in the Erdős-Rényi model](#tree-component-expectation-in-the-erdos-renyi-model)

For fixed $k\geq2$ and $\omega\to\infty$, the expected number of [tree components](graph.md#tree-component) of order $k$ is asymptotic to $k^{k-2}n^kp^{k-1}e^{-knp}/k!$ throughout the displayed window. It tends to infinity: split $np$ at $1$ and $(\log n)/(2k)$ to obtain lower bounds of orders $\omega^{k-1}$, $\sqrt n$, and $e^\omega$. Distinct overlapping vertex sets cannot both be components; disjoint sets have joint-to-product probability ratio $(1-p)^{-k^2}=1+o(1)$. Thus the relative variance vanishes, proving a component of order $k$ exists [with high probability](probabilistic-combinatorics.md#with-high-probability).

### Monotone graph property

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

A graph property is increasing and monotone when adding edges cannot destroy it.

#### Threshold function for a monotone graph property

↑ **Parent:** [Monotone graph property](#monotone-graph-property)

A function $p^*(n)$ is a threshold when the property holds with probability tending to zero for $p/p^*\to0$ and with probability tending to one for $p/p^*\to\infty$.

#### Monotone coupling of binomial random graphs

↑ **Parent:** [Monotone graph property](#monotone-graph-property)

Assign an independent uniform label $U_e$ to every possible edge and include $e$ in $G(n,p)$ exactly when $U_e\leq p$. This couples all edge probabilities so that $p\leq q$ implies $G(n,p)\subseteq G(n,q)$.

### Sprinkling of a binomial random graph

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

Sprinkling exposes independent rounds $G(n,p_1),\ldots,G(n,p_k)$. Their union has distribution $G(n,p)$ where

$$
1-p=\prod_{i=1}^k(1-p_i).
$$

<h3 id="isolated-vertices-in-the-erdos-renyi-model">Isolated vertices in the Erdős-Rényi model</h3>

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

Let $N$ be the number of isolated vertices in $G(n,p)$. Indicator variables give

$$
\mathbb EN=n(1-p)^{n-1}
$$

and, because a specified pair is simultaneously isolated precisely when the $2n-3$ incident edges are absent,

$$
\mathbb E(N^2)=n(1-p)^{n-1}
+n(n-1)(1-p)^{2n-3}.
$$

<h4 id="isolated-vertex-threshold-in-the-erdos-renyi-model">Isolated-vertex threshold in the Erdős-Rényi model</h4>

↑ **Parent:** [Isolated vertices in the Erdős-Rényi model](#isolated-vertices-in-the-erdos-renyi-model)

For $p=c\log n/n$, the number $N$ of isolated vertices satisfies

$$
\mathbb P(N=0)\longrightarrow
\begin{cases}
1,&c>1,\\
0,&c<1.
\end{cases}
$$

The upper side follows from the first-moment bound. On the lower side, $\mathbb EN\to\infty$ and $\operatorname{var}(N)/(\mathbb EN)^2\to0$, so the second-moment method applies.

<h3 id="connectivity-threshold-in-the-erdos-renyi-model">Connectivity threshold in the Erdős-Rényi model</h3>

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

For every fixed $\varepsilon>0$,

$$
p\geq(1+\varepsilon)\frac{\log n}{n}
\Longrightarrow\mathbb P(G(n,p)\text{ is connected})\to1,
$$

whereas the probability tends to zero when $p\leq(1-\varepsilon)\log n/n$. Above the threshold a union bound excludes every component of size at most $n/2$; below it isolated vertices remain with high probability.

#### Connectivity of a fixed-density binomial random graph

↑ **Parent:** [Connectivity threshold in the Erdős-Rényi model](#connectivity-threshold-in-the-erdos-renyi-model)

A disconnected [binomial random graph](graph-theory.md#binomial-random-graph) has a [connected component of a graph](graph.md#component-graph-theory) with at most half its [vertices](graph.md#vertex-graph-theory). The [union bound](probability-inequality.md#boole-s-inequality) over its possible [vertex sets](graph.md#vertex-set) gives

$$
\Pr(G(n,p)\text{ disconnected})
\leq\sum_{s=1}^{\lfloor n/2\rfloor}\binom ns(1-p)^{s(n-s)}
\leq\sum_{s=1}^{\lfloor n/2\rfloor}\bigl(n(1-p)^{n/2}\bigr)^s.
$$

The final [geometric series](sequence-and-series.md#geometric-series) bound tends to zero for fixed $p>0$.

#### Critical-window connectivity probability of a binomial random graph

↑ **Parent:** [Connectivity threshold in the Erdős-Rényi model](#connectivity-threshold-in-the-erdos-renyi-model)

For fixed real $c$, the number of [isolated vertices](#isolated-vertex) in a [binomial random graph](graph-theory.md#binomial-random-graph) with $p=(\log n+c)/n$ converges to a [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) of mean $e^{-c}$. Its fixed [factorial moments](continuous-time-markov-chain.md#factorial-moment) tend to $(e^{-c})^k$. A [union bound](probability-inequality.md#boole-s-inequality) for small [connected components](geometry-and-topology.md#connected-component), together with exclusion of intermediate components, shows that [isolated vertices](#isolated-vertex) are asymptotically the only obstruction to connectivity. Thus the displayed [limit](calculus.md#limit-of-a-function) is the zero-mass of that [Poisson distribution](discrete-probability-distribution.md#poisson-distribution).

<h3 id="expected-subgraph-count-in-the-erdos-renyi-model">Expected subgraph count in the Erdős-Rényi model</h3>

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

If a fixed graph $H$ has $v$ vertices, $e$ edges, and $N_H(n)$ unlabelled copies in $K_n$, then the number $X_H$ of its copies in $G(n,p)$ satisfies

$$
\mathbb E X_H=N_H(n)p^e.
$$

This follows by writing $X_H$ as a sum of [indicator random variables](expected-value.md#indicator-random-variable).

#### Sparse clique-count concentration

↑ **Parent:** [Expected subgraph count in the Erdős-Rényi model](#expected-subgraph-count-in-the-erdos-renyi-model)

For $p=n^{-2/3}\log n$, the number $X$ of copies of $K_4$ satisfies

$$
\mathbb EX=\binom n4p^6\sim\frac{(\log n)^6}{24}
$$

and $\operatorname{var}(X)=o((\mathbb EX)^2)$. Two distinct copies have dependent indicators only when they share at least two vertices; pairs sharing two or three vertices contribute respectively $O(n^6p^{11})$ and $O(n^5p^9)$ to the variance.

##### Pendant extensions of sparse clique copies

↑ **Parent:** [Sparse clique-count concentration](#sparse-clique-count-concentration)

If $H$ is formed by attaching one pendant [edge](graph-theory.md#edge-of-a-graph) to a fixed [clique](graph-theory.md#clique-graph-theory), each copy has a unique clique core. Its number of extensions is the number of ambient [edges](graph-theory.md#edge-of-a-graph) from that core to outside [vertices](graph.md#vertex-graph-theory). At a scale where the core count is tight and its expected extension count diverges sufficiently rapidly, a [Chernoff bound](probability-inequality.md#chernoff-bound) uniformly over all possible cores shows that the total count, divided by the extension [mean](expected-value.md), has the same limiting law as the core count. Non-induced copies are intended; extra ambient [edges](graph-theory.md#edge-of-a-graph) are not forbidden.

#### Vertex-disjoint sparse clique copies

↑ **Parent:** [Expected subgraph count in the Erdős-Rényi model](#expected-subgraph-count-in-the-erdos-renyi-model)

For $p=n^{-2/3}\log n$, the expected number of pairs of $K_4$ copies sharing a vertex is

$$
O(n^7p^{12}+n^6p^{11}+n^5p^9)=o(1).
$$

Thus, with probability tending to one, all the $K_4$ copies are vertex-disjoint. Together with [sparse clique-count concentration](#sparse-clique-count-concentration), this gives arbitrarily many vertex-disjoint copies with probability tending to one.

## ↑ Ancestors (5)

1. [Graph theory](graph-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (8)

- [Giant component](#giant-component)
- [Largest component of a graph](graph.md#largest-component-of-a-graph)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2024/paper-1.md#d6/a/solution)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2.md#6/a/solution)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-12.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13.md#3/iii/solution)
- [Small-world network](graph-theory.md#small-world-network)
