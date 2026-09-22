# Percolation theory

↑ **Parent:** [Probability theory](probability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Percolation_theory)

Percolation theory asks how many local connections must be available before a large connected structure appears. Start with a [graph](graph.md), randomly retain some [edges](graph-theory.md#edge-of-a-graph) or [vertices](graph.md#vertex-graph-theory), and study the resulting [percolation clusters](bond-percolation.md#percolation-cluster). In independent [bond percolation](bond-percolation.md), every [edge](graph-theory.md#edge-of-a-graph) is open with [probability](probability-theory.md#probability) $p$, independently of the others. In independent [site percolation](site-percolation.md), the random decisions concern [vertices](graph.md#vertex-graph-theory) instead. A [percolation cluster](bond-percolation.md#percolation-cluster) is a [connected component of a graph](graph.md#component-graph-theory) formed by the available connections; an [open path](bond-percolation.md#open-path-in-bond-percolation) joins two [vertices](graph.md#vertex-graph-theory) exactly when they belong to the same [percolation cluster](bond-percolation.md#percolation-cluster).

The attraction is that a local rule can produce a global change. One open [edge](graph-theory.md#edge-of-a-graph) says little about travel across a large [graph](graph.md). Many alternative [graph paths](graph-theory.md#path-in-a-graph) can nevertheless make distant connections likely. The model separates the geometry of possible connections from the [probability distribution](probability-distribution.md) of which connections are usable. This was the central perspective of Broadbent and Hammersley's 1957 paper, which discussed porous solids and disease transmission as interpretations of the same mathematical structure: [Percolation processes I: Crystals and mazes, introduction](https://courses.physics.ucsd.edu/2019/Spring/physics235/Broadbent_Hammersley.pdf). Independent [bond percolation](bond-percolation.md) supplies a simplified model of those systems; the physical interpretation still requires justification of its [independence](random-variable.md#independent-random-variables) assumptions.

For a completely calculable example, consider the four [edges](graph-theory.md#edge-of-a-graph) around a square and ask whether opposite corners $A$ and $C$ are connected. There are two [graph paths](graph-theory.md#path-in-a-graph), each using two [edges](graph-theory.md#edge-of-a-graph). Each [open path](bond-percolation.md#open-path-in-bond-percolation) has [probability](probability-theory.md#probability) $p^2$. Their [events](probability-space.md#event) are [independent events](probability-theory.md#independent-events) because the paths share no [edges](graph-theory.md#edge-of-a-graph), even though they share endpoints. The [inclusion-exclusion principle](combinatorics.md#inclusion-exclusion-principle) therefore gives

$$
\boxed{\mathbb P_p(A\leftrightarrow C)=2p^2-p^4.}
$$

At $p=1/2$, the connection [probability](probability-theory.md#probability) is $7/16$, larger than the $1/4$ for either chosen [graph path](graph-theory.md#path-in-a-graph). Counting all sixteen equally likely [edge](graph-theory.md#edge-of-a-graph) configurations gives the same answer: two configurations with exactly two open [edges](graph-theory.md#edge-of-a-graph), four with three, and one with four connect $A$ to $C$. Connectivity benefits from alternative routes; adding their [probabilities](probability-theory.md#probability) without subtracting their overlap would count the all-open configuration twice.

<a id="image-two-alternative-paths-increase-the-probability-of-connecting-opposite-corners"></a>
![](percolation-square-connectivity.png)

**[Figure 1](#image-two-alternative-paths-increase-the-probability-of-connecting-opposite-corners). Two alternative paths increase the probability of connecting opposite corners**.

This finite calculation is already useful for studying redundant connections. The deeper question is what happens as the [graph](graph.md) becomes arbitrarily large: does connectivity remain confined to finite [percolation clusters](bond-percolation.md#percolation-cluster), or can an [infinite percolation cluster](bond-percolation.md#infinite-percolation-cluster) appear? The [percolation probability](#percolation-probability) and [percolation critical probability](#percolation-critical-probability) make that question precise. A finite picture can illustrate the geometry, but cannot establish the existence of an [infinite percolation cluster](bond-percolation.md#infinite-percolation-cluster).

**Table of contents**

- [Directed percolation](#directed-percolation)
  - [Oriented site percolation](#oriented-site-percolation)
  - [Oriented bond percolation](#oriented-bond-percolation)
  - [Parallel-bond ray with different site and bond thresholds](#parallel-bond-ray-with-different-site-and-bond-thresholds)
  - [Incoming-edge coupling of site and bond percolation](#incoming-edge-coupling-of-site-and-bond-percolation)
  - [Survival and susceptibility thresholds for directed percolation](#survival-and-susceptibility-thresholds-for-directed-percolation)
- [Conformal invariance of planar percolation](#conformal-invariance-of-planar-percolation)
- [Lace expansion](#lace-expansion)
- [Bond percolation](bond-percolation.md)
  - [Rectangle crossing in bond percolation](bond-percolation.md#rectangle-crossing-in-bond-percolation)
    - [Finite-torus crossing amplification](bond-percolation.md#finite-torus-crossing-amplification)
  - [Open path in bond percolation](bond-percolation.md#open-path-in-bond-percolation)
  - [Uniform random orientation out-cluster comparison](bond-percolation.md#uniform-random-orientation-out-cluster-comparison)
  - [Percolation triangle condition](bond-percolation.md#percolation-triangle-condition)
  - [Percolation two-point connection probability](bond-percolation.md#percolation-two-point-connection-probability)
    - [Reflection lower bound for two-point percolation](bond-percolation.md#reflection-lower-bound-for-two-point-percolation)
  - [Connection decay rate in a percolation strip](bond-percolation.md#connection-decay-rate-in-a-percolation-strip)
    - [Strip approximation to the planar connection decay rate](bond-percolation.md#strip-approximation-to-the-planar-connection-decay-rate)
    - [Closed-cut bound for percolation in a strip](bond-percolation.md#closed-cut-bound-for-percolation-in-a-strip)
  - [Translation ergodicity of Bernoulli percolation](bond-percolation.md#translation-ergodicity-of-bernoulli-percolation)
  - [Percolation cluster](bond-percolation.md#percolation-cluster)
    - [Maximum cluster radius under exponential one-arm decay](bond-percolation.md#maximum-cluster-radius-under-exponential-one-arm-decay)
    - [Infinite percolation cluster](bond-percolation.md#infinite-percolation-cluster)
    - [Uniqueness of the infinite percolation cluster](bond-percolation.md#uniqueness-of-the-infinite-percolation-cluster)
      - [Percolation uniqueness on an amenable quasi-transitive graph](bond-percolation.md#percolation-uniqueness-on-an-amenable-quasi-transitive-graph)
      - [Boundary counting proof of percolation uniqueness](bond-percolation.md#boundary-counting-proof-of-percolation-uniqueness)
        - [Encounter box in percolation](bond-percolation.md#encounter-box-in-percolation)
      - [Trifurcation vertex in percolation](bond-percolation.md#trifurcation-vertex-in-percolation)
        - [Trifurcation boundary-counting lemma](bond-percolation.md#trifurcation-boundary-counting-lemma)
          - [Forest proof of trifurcation boundary counting](bond-percolation.md#forest-proof-of-trifurcation-boundary-counting)
  - [Percolation susceptibility](bond-percolation.md#percolation-susceptibility)
    - [Tree-graph moment bound for a percolation cluster](bond-percolation.md#tree-graph-moment-bound-for-a-percolation-cluster)
    - [Exponential one-arm decay from finite susceptibility](bond-percolation.md#exponential-one-arm-decay-from-finite-susceptibility)
  - [Russo-Seymour-Welsh theorem](bond-percolation.md#russo-seymour-welsh-theorem)
    - [Uniform RSW crossing estimate](bond-percolation.md#uniform-rsw-crossing-estimate)
    - [RSW reflection extension lemma](bond-percolation.md#rsw-reflection-extension-lemma)
      - [Reflected attachment estimate for percolation](bond-percolation.md#reflected-attachment-estimate-for-percolation)
    - [One-arm probability](bond-percolation.md#one-arm-probability)
      - [Weighted BK boundary-splitting estimate](bond-percolation.md#weighted-bk-boundary-splitting-estimate)
      - [Polynomial critical one-arm upper bound](bond-percolation.md#polynomial-critical-one-arm-upper-bound)
      - [Independent annular barriers for percolation](bond-percolation.md#independent-annular-barriers-for-percolation)
      - [BK boundary-splitting estimate](bond-percolation.md#bk-boundary-splitting-estimate)
      - [Percolation one-arm decay rate](bond-percolation.md#percolation-one-arm-decay-rate)
        - [Almost-subadditive percolation decay rate](bond-percolation.md#almost-subadditive-percolation-decay-rate)
      - [One-arm extension estimate](bond-percolation.md#one-arm-extension-estimate)
        - [RSW gluing lemma for two one-arm events](bond-percolation.md#rsw-gluing-lemma-for-two-one-arm-events)
  - [Van den Berg-Kesten inequality](bond-percolation.md#van-den-berg-kesten-inequality)
    - [Coordinate-splitting proof of the BK inequality](bond-percolation.md#coordinate-splitting-proof-of-the-bk-inequality)
    - [Square-lattice one-arm lower bound from disjoint occurrence](bond-percolation.md#square-lattice-one-arm-lower-bound-from-disjoint-occurrence)
    - [Disjoint occurrence of increasing events](bond-percolation.md#disjoint-occurrence-of-increasing-events)
- [Percolation probability](#percolation-probability)
  - [Boundary-side amplification for planar percolation](#boundary-side-amplification-for-planar-percolation)
  - [Near-critical percolation power upper bound](#near-critical-percolation-power-upper-bound)
  - [Right continuity of percolation probability](#right-continuity-of-percolation-probability)
    - [Supercritical continuity of percolation probability](#supercritical-continuity-of-percolation-probability)
  - [Percolation critical probability](#percolation-critical-probability)
    - [Sharpness of the percolation transition](#sharpness-of-the-percolation-transition)
    - [Connective-constant lower bound for percolation](#connective-constant-lower-bound-for-percolation)
    - [Harris-Kesten theorem](#harris-kesten-theorem)
      - [Harris theorem for square-lattice bond percolation](#harris-theorem-for-square-lattice-bond-percolation)
      - [Alternating arms argument at the self-dual percolation parameter](#alternating-arms-argument-at-the-self-dual-percolation-parameter)
        - [Three-fold symmetric primal-dual noncoexistence](#three-fold-symmetric-primal-dual-noncoexistence)
        - [Alternating exterior-arm separation lemma](#alternating-exterior-arm-separation-lemma)
- [Monotone coupling of Bernoulli percolation](#monotone-coupling-of-bernoulli-percolation)
  - [Finite-box comparison for percolation parameters](#finite-box-comparison-for-percolation-parameters)
  - [Coupled onset parameter for origin percolation](#coupled-onset-parameter-for-origin-percolation)
  - [Sprinkling coupling for Bernoulli percolation](#sprinkling-coupling-for-bernoulli-percolation)
- [Site percolation](site-percolation.md)
  - [Critical probability for site percolation on the triangular lattice](site-percolation.md#critical-probability-for-site-percolation-on-the-triangular-lattice)
  - [Domain Markov property of a percolation exploration](site-percolation.md#domain-markov-property-of-a-percolation-exploration)
  - [Dependent percolation](site-percolation.md#dependent-percolation)
    - [One-independent bond percolation](site-percolation.md#one-independent-bond-percolation)
      - [Separated-block percolation renormalization](site-percolation.md#separated-block-percolation-renormalization)
      - [Peierls circuit bound for one-independent percolation](site-percolation.md#peierls-circuit-bound-for-one-independent-percolation)
    - [Monochromatic line-graph percolation counterexample](site-percolation.md#monochromatic-line-graph-percolation-counterexample)
    - [Random-cluster model](site-percolation.md#random-cluster-model)
      - [Bernoulli bounds for the random-cluster model](site-percolation.md#bernoulli-bounds-for-the-random-cluster-model)
      - [Cluster weight in the random-cluster model](site-percolation.md#cluster-weight-in-the-random-cluster-model)
      - [Random-cluster critical probability](site-percolation.md#random-cluster-critical-probability)
        - [Monotonicity of random-cluster critical probability in cluster weight](site-percolation.md#monotonicity-of-random-cluster-critical-probability-in-cluster-weight)
      - [Random-cluster weight monotonicity](site-percolation.md#random-cluster-weight-monotonicity)
      - [Self-dual parameter of the random-cluster model](site-percolation.md#self-dual-parameter-of-the-random-cluster-model)
        - [Symmetric cluster weight at the self-dual parameter](site-percolation.md#symmetric-cluster-weight-at-the-self-dual-parameter)
      - [Random-cluster single-edge conditional probability](site-percolation.md#random-cluster-single-edge-conditional-probability)
      - [Random-cluster boundary condition](site-percolation.md#random-cluster-boundary-condition)
        - [Boundary monotonicity of the random-cluster measure](site-percolation.md#boundary-monotonicity-of-the-random-cluster-measure)
        - [Wired random-cluster boundary condition](site-percolation.md#wired-random-cluster-boundary-condition)
          - [Infinite-volume wired random-cluster measure](site-percolation.md#infinite-volume-wired-random-cluster-measure)
            - [Random-cluster inverse correlation length](site-percolation.md#random-cluster-inverse-correlation-length)
              - [Reflection comparison of random-cluster connections](site-percolation.md#reflection-comparison-of-random-cluster-connections)
        - [Free random-cluster boundary condition](site-percolation.md#free-random-cluster-boundary-condition)
      - [Positive association of the random-cluster model](site-percolation.md#positive-association-of-the-random-cluster-model)
      - [Uniform connected-subgraph limit of the random-cluster model](site-percolation.md#uniform-connected-subgraph-limit-of-the-random-cluster-model)
      - [Uniform spanning-tree limit of the random-cluster model](site-percolation.md#uniform-spanning-tree-limit-of-the-random-cluster-model)
      - [Edwards-Sokal coupling](site-percolation.md#edwards-sokal-coupling)
        - [Spin-connectivity identity for the Potts model](site-percolation.md#spin-connectivity-identity-for-the-potts-model)
      - [Heat-bath Markov chain](site-percolation.md#heat-bath-markov-chain)
    - [Level-set percolation](site-percolation.md#level-set-percolation)
      - [Critical threshold for level-set percolation](site-percolation.md#critical-threshold-for-level-set-percolation)
    - [Finite-range dependent random field](site-percolation.md#finite-range-dependent-random-field)
- [Peierls argument](#peierls-argument)
  - [Connective-constant Peierls bound](#connective-constant-peierls-bound)
- [Finite-energy property (percolation)](#finite-energy-property-percolation)
  - [Finite-energy property of Bernoulli percolation](#finite-energy-property-of-bernoulli-percolation)
    - [Finite modification of Bernoulli percolation](#finite-modification-of-bernoulli-percolation)
- [Exponential decay of subcritical percolation](#exponential-decay-of-subcritical-percolation)
  - [Finite-set criterion for percolation sharpness](#finite-set-criterion-for-percolation-sharpness)
  - [Exponential tail of subcritical cluster size](#exponential-tail-of-subcritical-cluster-size)
- [One-arm event](#one-arm-event)
- [OSSS inequality](#osss-inequality)
  - [OSSS exploration of a one-arm event](#osss-exploration-of-a-one-arm-event)

## Directed percolation

↑ **Parent:** [Percolation theory](percolation-theory.md)

In [bond percolation](bond-percolation.md) on a [directed graph](graph-theory.md#directed-graph), independently open each [directed edge](graph-theory.md#directed-edge) with [probability](probability-theory.md#probability) $p$. The out-cluster of $x$ consists of vertices reachable by open [directed paths](graph-theory.md#directed-path). In [site percolation](site-percolation.md), independently open vertices and require every vertex of the [directed path](graph-theory.md#directed-path), including $x$, to be open. The same definitions allow a [multigraph](graph.md#multigraph). The orientation matters: an infinite underlying [connected graph](graph.md#connected-graph) need not contain an infinite out-cluster from a specified root.

### Oriented site percolation

↑ **Parent:** [Directed percolation](#directed-percolation)

Independently open vertices of a [directed graph](graph-theory.md#directed-graph) with common [probability](probability-theory.md#probability) $p$, and require every vertex of an infinite directed path to be open, including its root. Conditioning the root to be open changes the survival probability by a factor $p$ and does not change the critical probability. This model gives an independent comparison process in the [independent oriented-percolation comparison for the contact process](stochastic-process.md#independent-oriented-percolation-comparison-for-the-contact-process).

### Oriented bond percolation

↑ **Parent:** [Directed percolation](#directed-percolation)

Independently open the bonds of a [directed graph](graph-theory.md#directed-graph) with a common [probability](probability-theory.md#probability) $p$, and ask whether an infinite open directed path starts at a specified root. On the oriented [square lattice](graph.md#square-lattice), edges run from $(x,n)$ to $(x\pm1,n+1)$ with $x+n$ even. The critical probability is the infimum of parameters with positive survival probability. The [incoming-edge coupling of site and bond percolation](#incoming-edge-coupling-of-site-and-bond-percolation) compares this threshold with that of [oriented site percolation](#oriented-site-percolation).

### Parallel-bond ray with different site and bond thresholds

↑ **Parent:** [Directed percolation](#directed-percolation)

Take a [directed graph](graph-theory.md#directed-graph) with vertices $v_0,v_1,\ldots$ and $n+1$ parallel bonds from $v_n$ to $v_{n+1}$. This is a [locally finite graph](graph-theory.md#locally-finite-graph), although the incoming degrees are unbounded. For [bond percolation](bond-percolation.md), $\theta_b(p)=\prod_{n\ge0}(1-(1-p)^{n+1})>0$ whenever $p>0$: the failure [probabilities](probability-theory.md#probability) are summable, so the [infinite product](sequence-and-series.md#infinite-product) is positive. For [site percolation](site-percolation.md), survival requires every vertex of the ray to be open, which has [probability](probability-theory.md#probability) zero for $p<1$. Thus the [survival and susceptibility thresholds for directed percolation](#survival-and-susceptibility-thresholds-for-directed-percolation) satisfy $p_H^b=0$ and $p_H^s=1$.

### Incoming-edge coupling of site and bond percolation

↑ **Parent:** [Directed percolation](#directed-percolation)

Suppose every vertex of a [directed graph](graph-theory.md#directed-graph) has at most $\Delta$ incoming bonds. In [bond percolation](bond-percolation.md) with parameter $q$, open a site whenever at least one incoming bond is open. Incoming bond sets have different heads and hence are disjoint, so these site indicators are [independent random variables](random-variable.md#independent-random-variables). Supplement their [probabilities](probability-theory.md#probability) to $r=1-(1-q)^\Delta$. Every vertex reached by a nontrivial open [directed path](graph-theory.md#directed-path) is now open. Conditioning the root to be open gives $\theta_s(r)\ge r\theta_b(q)$, since a simple [directed path](graph-theory.md#directed-path) from the root never uses a bond entering the root. Thus $p_H^s\le1-(1-p_H^b)^\Delta$.

### Survival and susceptibility thresholds for directed percolation

↑ **Parent:** [Directed percolation](#directed-percolation)

For the out-cluster $C_x$ in [directed percolation](#directed-percolation), define $p_H=\inf\{p:\mathbb P_p(|C_x|=\infty)>0\}$ and $p_T=\inf\{p:\mathbb E_p|C_x|=\infty\}$, with value $1$ when the relevant set is empty below $1$. The first is a survival threshold; the second is a [percolation susceptibility](bond-percolation.md#percolation-susceptibility) threshold. Both depend on the root in a general [directed graph](graph-theory.md#directed-graph). Exploring a [site percolation](site-percolation.md) cluster and using each fresh vertex coin for its first tested incoming bond gives a [coupling of probability distributions](probability-and-statistics.md#coupling) with [bond percolation](bond-percolation.md) such that $\theta_s(p)\le p\theta_b(p)$ and $\chi_s(p)\le p\chi_b(p)$. Consequently $p_H^b\le p_H^s$ and $p_T^b\le p_T^s$.

## Conformal invariance of planar percolation

↑ **Parent:** [Percolation theory](percolation-theory.md)

For critical [site percolation](site-percolation.md) on the [triangular lattice](graph.md#triangular-lattice), scaling-limit crossing probabilities transform naturally under conformal maps between planar domains. This rigorously established property supports descriptions of interfaces by [SLE](schramm-loewner-evolution.md) and calculations of planar [percolation critical exponents](critical-phenomenon.md#percolation-critical-exponents). Transferring it to a different lattice or to [bond percolation](bond-percolation.md) requires a separate universality argument.

## Lace expansion

↑ **Parent:** [Percolation theory](percolation-theory.md)

An iterative expansion of long-range connectivity functions that separates an approximately random-walk contribution from corrections caused by loops and intersections. In suitable high-dimensional [percolation](percolation-theory.md) models it controls these corrections and proves [mean-field percolation exponents](critical-phenomenon.md#mean-field-percolation-exponents). It also applies to other models, including [self-avoiding walks](combinatorics.md#self-avoiding-walk); its use always requires model-specific estimates.

## Bond percolation

↑ **Parent:** [Percolation theory](percolation-theory.md)

[This section is present in another page, follow this link to view it.](bond-percolation.md)

## Percolation probability

↑ **Parent:** [Percolation theory](percolation-theory.md)

For independent [bond percolation](bond-percolation.md) on an infinite [graph](graph.md) with a specified root $o$, let $C_o$ be its [percolation cluster](bond-percolation.md#percolation-cluster). The percolation probability is

$$
\theta(p)=\mathbb P_p(|C_o|=\infty).
$$

It concerns the root, rather than the existence of an [infinite percolation cluster](bond-percolation.md#infinite-percolation-cluster) somewhere else. Even above the [percolation critical probability](#percolation-critical-probability) of the [square lattice](graph.md#square-lattice), an isolated root has [probability](probability-theory.md#probability) $(1-p)^4$, because its four incident [edges](graph-theory.md#edge-of-a-graph) can all be closed. Thus $\theta(p)\leq1-(1-p)^4<1$ when $p<1$. Positive percolation probability does not mean every [vertex](graph.md#vertex-graph-theory) is connected to infinity.

On the [square lattice](graph.md#square-lattice), the [events](probability-space.md#event) that $o$ is joined by an [open path](bond-percolation.md#open-path-in-bond-percolation) to the boundary of $[-n,n]^2$ decrease as $n$ increases. Their [probabilities](probability-theory.md#probability) converge to $\theta(p)$ by [continuity from above of a measure](measure.md#continuity-from-above-of-a-measure). This relates an infinite question to finite observations, without equating any one finite boundary connection with survival forever. The [monotone coupling of Bernoulli percolation](#monotone-coupling-of-bernoulli-percolation) shows that $\theta$ is a [monotone function](calculus.md#monotonic-function) of $p$.

### Boundary-side amplification for planar percolation

↑ **Parent:** [Percolation probability](#percolation-probability)

If an [infinite percolation cluster](bond-percolation.md#infinite-percolation-cluster) exists almost surely, the [probability](probability-theory.md#probability) that a large square box intersects one tends to one. The four rotationally symmetric exterior-side arm events are increasing. By the [Harris-FKG inequality](probability-inequality.md#harris-fkg-inequality), their common [probability](probability-theory.md#probability) is at least $1-(1-P(D_N))^{1/4}$, where $D_N$ is their union. Thus a pair of specified opposite sides both has an infinite exterior arm with [probability](probability-theory.md#probability) at least $1-2(1-P(D_N))^{1/4}$, tending to one. The rays start at a boundary [graph vertex](graph.md#vertex-graph-theory) and immediately leave the [graph vertex](graph.md#vertex-graph-theory) box.

### Near-critical percolation power upper bound

↑ **Parent:** [Percolation probability](#percolation-probability)

Suppose a planar [bond percolation](bond-percolation.md) model has critical [one-arm probability](bond-percolation.md#one-arm-probability) at most $Cn^{-\alpha}$ with $\alpha>0$, and a finite-radius connection event depends on $O(n^2)$ [edges](graph-theory.md#edge-of-a-graph). The [finite-box comparison for percolation parameters](#finite-box-comparison-for-percolation-parameters) gives $\theta(p_c+\varepsilon)\leq Cn^{-\alpha}+C'\varepsilon n^2$. Balancing at $n\asymp\varepsilon^{-1/(\alpha+2)}$ gives $\theta(p_c+\varepsilon)\leq A\varepsilon^{\alpha/(\alpha+2)}$. For the [square lattice](graph.md#square-lattice) use $p_c=1/2$ and the [polynomial critical one-arm upper bound](bond-percolation.md#polynomial-critical-one-arm-upper-bound).

### Right continuity of percolation probability

↑ **Parent:** [Percolation probability](#percolation-probability)

For independent [site percolation](site-percolation.md) or [bond percolation](bond-percolation.md) on a rooted [locally finite graph](graph-theory.md#locally-finite-graph), $\theta(p)$ is right continuous on $[0,1)$. Finite-radius connection events have polynomial [probabilities](probability-theory.md#probability) in $p$ and decrease to infinite connection. Thus $\theta$ is their infimum by [continuity from above of a measure](measure.md#continuity-from-above-of-a-measure). This infimum of [continuous functions](calculus.md#continuous-function) is upper semicontinuous; parameter monotonicity from the [monotone coupling of Bernoulli percolation](#monotone-coupling-of-bernoulli-percolation) then gives right continuity.

#### Supercritical continuity of percolation probability

↑ **Parent:** [Right continuity of percolation probability](#right-continuity-of-percolation-probability)

Independent [site percolation](site-percolation.md) and [bond percolation](bond-percolation.md) on the [cubic lattice](graph.md#cubic-lattice) have continuous [percolation probability](#percolation-probability) on $(p_c,1]$. Fix $p>p_c$ and an intermediate $q\in(p_c,p)$. By [uniqueness of the infinite percolation cluster](bond-percolation.md#uniqueness-of-the-infinite-percolation-cluster), every origin in the infinite $p$-cluster has a finite $p$-open [graph path](graph-theory.md#path-in-a-graph) to the infinite $q$-cluster. In the uniform-label [monotone coupling of Bernoulli percolation](#monotone-coupling-of-bernoulli-percolation), the finitely many labels on this [graph path](graph-theory.md#path-in-a-graph) are strictly below fixed $p$ [almost surely](convergence-of-random-variables.md#almost-sure-convergence), so it persists at some parameter below $p$. The [coupled onset parameter for origin percolation](#coupled-onset-parameter-for-origin-percolation) has no attained atom there, giving left continuity, including at $1$. Combine this with [right continuity of percolation probability](#right-continuity-of-percolation-probability).

### Percolation critical probability

↑ **Parent:** [Percolation probability](#percolation-probability)

For the rooted infinite model defining [percolation probability](#percolation-probability), the percolation critical probability is

$$
p_c=\inf\{p:\theta(p)>0\}.
$$

Below $p_c$, the root has [probability](probability-theory.md#probability) zero of belonging to an [infinite percolation cluster](bond-percolation.md#infinite-percolation-cluster). Above $p_c$, that [probability](probability-theory.md#probability) is positive, by the definition and the [monotone coupling of Bernoulli percolation](#monotone-coupling-of-bernoulli-percolation). The definition alone does not determine behavior at $p_c$, or the numerical value of $p_c$: these require results specific to the [graph](graph.md) and the model.

A finite [graph](graph.md) with $M$ [edges](graph-theory.md#edge-of-a-graph) has $2^M$ open/closed configurations. The [probability](probability-theory.md#probability) of any connectivity [event](probability-space.md#event) is a finite sum of terms $p^k(1-p)^{M-k}$, hence a [polynomial](polynomial.md) in $p$. The square's $2p^2-p^4$ is an example. These finite [probabilities](probability-theory.md#probability) vary smoothly, although an infinite-system limit can distinguish a whole interval with $\theta(p)=0$ from one with $\theta(p)>0$. A steep finite connection curve and a mathematically proved [percolation critical probability](#percolation-critical-probability) are different kinds of information.

#### Sharpness of the percolation transition

↑ **Parent:** [Percolation critical probability](#percolation-critical-probability)

Independent [bond percolation](bond-percolation.md) on the [cubic lattice](graph.md#cubic-lattice) has exponential connection decay at every $p<p_c$ and positive [percolation probability](#percolation-probability) at every $p>p_c$. The [finite-set criterion for percolation sharpness](#finite-set-criterion-for-percolation-sharpness) gives decay below its auxiliary threshold. The [Margulis–Russo formula](analysis-of-boolean-functions.md#margulis-russo-formula) and exploration from a finite box boundary give $g_n'(p)\geq(1-g_n(p))\inf_{S\ni0}\varphi_p(S)/(p(1-p))$, with the infimum over interior finite sets. Above the auxiliary threshold the infimum is at least one; integrating gives positive [percolation probability](#percolation-probability) and identifies the two thresholds. This theorem does not identify the value of $p_c$ for a particular lattice.

#### Connective-constant lower bound for percolation

↑ **Parent:** [Percolation critical probability](#percolation-critical-probability)

For independent [bond percolation](bond-percolation.md) on a transitive locally finite lattice, let $c_n$ count rooted [self-avoiding walks](combinatorics.md#self-avoiding-walk) and let $\mu=\lim c_n^{1/n}$ be the [connective constant](combinatorics.md#connective-constant). An infinite open [percolation cluster](bond-percolation.md#percolation-cluster) supplies an open walk of every length. The [union bound](probability-inequality.md#boole-s-inequality) gives $\theta(p)\leq c_np^n$, which tends to zero when $p\mu<1$. Thus $p_c\geq1/\mu$.

#### Harris-Kesten theorem

↑ **Parent:** [Percolation critical probability](#percolation-critical-probability)

The [percolation critical probability](#percolation-critical-probability) of independent [bond percolation](bond-percolation.md) on the infinite [square lattice](graph.md#square-lattice) is exactly

$$
\boxed{p_c(\mathbb Z^2)=\frac12.}
$$

In this model, $\theta(p)=0$ for $p\leq1/2$ and $\theta(p)>0$ for $p>1/2$. The particular [graph](graph.md), independent [edge](graph-theory.md#edge-of-a-graph) decisions, and distinction between [bond percolation](bond-percolation.md) and [site percolation](site-percolation.md) matter: this value is not a universal threshold for arbitrary random networks. The equality of open and closed [edge](graph-theory.md#edge-of-a-graph) [probabilities](probability-theory.md#probability) at $1/2$ suggests a relation to [dual bond percolation](planar-graph.md#dual-bond-percolation), but that symmetry alone is not a proof of long-distance connectivity.

Harris established the lower bound, including absence of an [infinite percolation cluster](bond-percolation.md#infinite-percolation-cluster) at $p=1/2$, in 1960. Kesten completed the equality in 1980. His original paper states the threshold result as Theorem 1 and the positive/zero [percolation probability](#percolation-probability) alternatives as Theorem 2: [Harry Kesten, The critical probability of bond percolation on the square lattice equals 1/2](https://math.bme.hu/~balint/oktatas/perkolacio/percolation_papers/kesten_1.pdf). These are claims about the infinite [square lattice](graph.md#square-lattice), rather than deductions from a simulated finite sample.

##### Harris theorem for square-lattice bond percolation

↑ **Parent:** [Harris-Kesten theorem](#harris-kesten-theorem)

Uniform fixed-aspect [rectangle crossing in bond percolation](bond-percolation.md#rectangle-crossing-in-bond-percolation) bounds at the self-dual parameter yield a positive lower bound for closed dual circuits in geometrically spaced disjoint annuli. The [independent annular barriers for percolation](bond-percolation.md#independent-annular-barriers-for-percolation) imply that an origin-to-infinity open [graph path](graph-theory.md#path-in-a-graph) has probability zero. Parameter monotonicity gives zero [percolation probability](#percolation-probability) for every $p\leq1/2$.

##### Alternating arms argument at the self-dual percolation parameter

↑ **Parent:** [Harris-Kesten theorem](#harris-kesten-theorem)

At parameter $1/2$, primal and [dual bond percolation](planar-graph.md#dual-bond-percolation) on the [square lattice](graph.md#square-lattice) have the same [probability distribution](probability-distribution.md). Suppose an [infinite percolation cluster](bond-percolation.md#infinite-percolation-cluster) exists. Large boxes meet it with [probability](probability-theory.md#probability) tending to one. The [square-root trick for positively associated events](probability-inequality.md#square-root-trick-for-positively-associated-events) and quarter-turn symmetry imply that each side has an infinite exterior open arm with [probability](probability-theory.md#probability) tending to one. The same holds for dual arms. A [union bound](probability-inequality.md#boole-s-inequality) then gives positive [probability](probability-theory.md#probability) of primal top and bottom arms together with dual left and right arms.

Use a primal box $[-r,r]^2$ and a dual box with sides at $\pm(r+1/2)$. Open only primal [edges](graph-theory.md#edge-of-a-graph) whose endpoints both lie in the primal box, preserving all outward and exterior arm [edges](graph-theory.md#edge-of-a-graph). The two primal arms are joined inside. Planarity prevents the two alternating dual arms from joining: a proposed dual connection together with the inner boundary arc separates one primal infinite arm from infinity. Thus the modified configuration has two infinite dual clusters. Its positive [probability](probability-theory.md#probability) by [finite modification of Bernoulli percolation](#finite-modification-of-bernoulli-percolation) contradicts [uniqueness of the infinite percolation cluster](bond-percolation.md#uniqueness-of-the-infinite-percolation-cluster). Consequently the [percolation probability](#percolation-probability) at $1/2$ is zero. This is often called Zhang's argument.

###### Three-fold symmetric primal-dual noncoexistence

↑ **Parent:** [Alternating arms argument at the self-dual percolation parameter](#alternating-arms-argument-at-the-self-dual-percolation-parameter)

For independent [bond percolation](bond-percolation.md) on a periodic plane lattice with three-fold rotation symmetry, the primal model at $p$ and the [dual bond percolation](planar-graph.md#dual-bond-percolation) model at $1-p$ cannot both percolate. To adapt [Zhang's argument](#alternating-arms-argument-at-the-self-dual-percolation-parameter), divide a large boundary circle into six arcs, repeating the division in each $120$-degree sector. Vary the division point until the failure probabilities $a,b$ of the two alternating primal arc types are comparable within a factor $(1-p)^{-2}$. Moving past a single crossing edge changes a failure probability by at most a factor $(1-p)^{-1}$, by the [FKG inequality](probability-inequality.md#fkg-inequality). If the probability of no primal exterior arm is at most $\varepsilon$, then $a^3b^3\le\varepsilon$ and both failures are at most $(1-p)^{-1}\varepsilon^{1/6}$. For the dual model, at least one arc type has failure at most $\varepsilon^{1/6}$; its three rotations have the same bound. Four alternating primal/dual arms now occur with positive probability, contradicting the [alternating exterior-arm separation lemma](#alternating-exterior-arm-separation-lemma) and uniqueness after a finite modification. This extends the four-fold argument to the [martini lattice](planar-graph.md#martini-lattice).

###### Alternating exterior-arm separation lemma

↑ **Parent:** [Alternating arms argument at the self-dual percolation parameter](#alternating-arms-argument-at-the-self-dual-percolation-parameter)

Four infinite exterior arms entering a square in alternating primal-open and dual-open order force the two primal arms to be disjoint outside the square. If they met, their finite connecting crosscut together with a boundary arc would enclose one dual arm, preventing its escape to infinity. Connecting the two primal arms through the square creates a proper doubly infinite [open path](bond-percolation.md#open-path-in-bond-percolation), separating the two remaining dual infinite tails. [finite-energy property of Bernoulli percolation](#finite-energy-property-of-bernoulli-percolation) can then turn this configuration into two infinite dual clusters, contradicting uniqueness. Care is needed to preserve the exterior dual tails even if the finite modification destroys their original boundary attachments.

## Monotone coupling of Bernoulli percolation

↑ **Parent:** [Percolation theory](percolation-theory.md)

Assign each [edge](graph-theory.md#edge-of-a-graph) $e$ an [independent](random-variable.md#independent-random-variables) [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) label $U_e$ on $[0,1]$. At parameter $p$, declare $e$ open exactly when $U_e\leq p$. Each open/closed decision then has the required [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution), and different [edge](graph-theory.md#edge-of-a-graph) decisions are [independent](random-variable.md#independent-random-variables). The same construction applies to [site percolation](site-percolation.md) with labels on [vertices](graph.md#vertex-graph-theory).

Keep those labels fixed when increasing $p$. For $p\leq q$, every $p$-open [edge](graph-theory.md#edge-of-a-graph) is also $q$-open, so every $p$-open [graph path](graph-theory.md#path-in-a-graph) survives and each [percolation cluster](bond-percolation.md#percolation-cluster) can only gain [vertices](graph.md#vertex-graph-theory). This [coupling of probability distributions](probability-and-statistics.md#coupling) compares complete configurations on one [probability space](probability-space.md), rather than comparing two unrelated pictures. Any [increasing event](probability-inequality.md#increasing-event), such as an [open path](bond-percolation.md#open-path-in-bond-percolation) between specified [vertices](graph.md#vertex-graph-theory), consequently has a nondecreasing [probability](probability-theory.md#probability).

<a id="image-one-set-of-random-edge-labels-gives-nested-root-clusters-as-the-opening-probability-increases"></a>
![](percolation-monotone-grid.png)

**[Figure 2](#image-one-set-of-random-edge-labels-gives-nested-root-clusters-as-the-opening-probability-increases). One set of random edge labels gives nested root clusters as the opening probability increases**.

The three panels use one seeded collection of labels on a finite $17\times17$ [square lattice](graph.md#square-lattice) box. Colored [edges](graph-theory.md#edge-of-a-graph) and dots show the central root's [percolation cluster](bond-percolation.md#percolation-cluster); gray [edges](graph-theory.md#edge-of-a-graph) are open but disconnected from it. A [percolation cluster](bond-percolation.md#percolation-cluster) can grow by many [vertices](graph.md#vertex-graph-theory) when one newly opened [edge](graph-theory.md#edge-of-a-graph) joins it to another large [percolation cluster](bond-percolation.md#percolation-cluster). The panels illustrate a nested construction, not an estimate of $\theta(p)$ or a proof of the [Harris-Kesten theorem](#harris-kesten-theorem).

### Finite-box comparison for percolation parameters

↑ **Parent:** [Monotone coupling of Bernoulli percolation](#monotone-coupling-of-bernoulli-percolation)

If an [increasing event](probability-inequality.md#increasing-event) $A$ depends on $m$ sites or [edges](graph-theory.md#edge-of-a-graph), the uniform-label [monotone coupling of Bernoulli percolation](#monotone-coupling-of-bernoulli-percolation) and the [union bound](probability-inequality.md#boole-s-inequality) give $0\leq\mathbb P_q(A)-\mathbb P_p(A)\leq m(q-p)$ for $p\leq q$. A change of the event requires a coordinate with label in $(p,q]$. For [bond percolation](bond-percolation.md) from the origin to the boundary of $[-n,n]^2$, first-hit [graph paths](graph-theory.md#path-in-a-graph) use the $4n(2n+1)$ internal [edges](graph-theory.md#edge-of-a-graph), so the same count bounds the parameter sensitivity.

### Coupled onset parameter for origin percolation

↑ **Parent:** [Monotone coupling of Bernoulli percolation](#monotone-coupling-of-bernoulli-percolation)

In the uniform-label [monotone coupling of Bernoulli percolation](#monotone-coupling-of-bernoulli-percolation), let $I_p$ mean that the origin belongs to an [infinite percolation cluster](bond-percolation.md#infinite-percolation-cluster), and let $M=\inf\{p:I_p\}$. The occurrence parameters form an upper interval. Therefore $\{M<p\}=\bigcup_{r<p,\ r\in\mathbb Q}I_r$ and $\theta(p-)=\mathbb P(M<p)$. Since $\{M<p\}\subseteq I_p\subseteq\{M\leq p\}$, the jump is $\theta(p)-\theta(p-)=\mathbb P(I_p\cap\{M=p\})$. Occurrence at the infimum is not presumed.

### Sprinkling coupling for Bernoulli percolation

↑ **Parent:** [Monotone coupling of Bernoulli percolation](#monotone-coupling-of-bernoulli-percolation)

For $p<q$, first sample Bernoulli percolation at parameter $p$, then independently open each remaining closed coordinate with probability $(q-p)/(1-p)$. Every coordinate is then open with probability $q$, so the union has the parameter-$q$ law. This coupling separates existing $p$-clusters from the additional sprinkled connections between them.

## Site percolation

↑ **Parent:** [Percolation theory](percolation-theory.md)

[This section is present in another page, follow this link to view it.](site-percolation.md)

## Peierls argument

↑ **Parent:** [Percolation theory](percolation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Peierls_argument)

A Peierls argument bounds a rare large defect by encoding it as a contour, estimating the number of contours of each size, and summing their exponentially small probabilities.

### Connective-constant Peierls bound

↑ **Parent:** [Peierls argument](#peierls-argument)

Independent [bond percolation](bond-percolation.md) on the [square lattice](graph.md#square-lattice) satisfies $p_c\leq1-\mu^{-1}$, where $\mu$ is its [connective constant](combinatorics.md#connective-constant). If $(1-p)\mu<1$, closed dual [graph cycles](graph-theory.md#cycle-in-a-graph) have a summable large-length tail: their counts are bounded by a polynomial factor times the count of [self-avoiding walks](combinatorics.md#self-avoiding-walk). Conditioning a sufficiently large finite box to be open excludes short enclosing [graph cycles](graph-theory.md#cycle-in-a-graph) without changing the law of the remaining [edges](graph-theory.md#edge-of-a-graph). With positive conditional [probability](probability-theory.md#probability) no enclosing closed dual [graph cycle](graph-theory.md#cycle-in-a-graph) remains, so the origin belongs to an [infinite percolation cluster](bond-percolation.md#infinite-percolation-cluster).

## Finite-energy property (percolation)

↑ **Parent:** [Percolation theory](percolation-theory.md)

A [percolation](percolation-theory.md) measure has the finite-energy property if, conditional on all exterior states, every prescribed state of any finite collection of sites or edges has positive [probability](probability-theory.md#probability) almost surely. This permits finite local modifications within events of positive probability. It is a hypothesis on the measure and does not follow merely from invariance under graph symmetries.

### Finite-energy property of Bernoulli percolation

↑ **Parent:** [Finite-energy property (percolation)](#finite-energy-property-percolation)

For $0<p<1$, prescribing any finite collection of Bernoulli percolation sites or edges has positive conditional probability given all states outside that collection.

#### Finite modification of Bernoulli percolation

↑ **Parent:** [Finite-energy property of Bernoulli percolation](#finite-energy-property-of-bernoulli-percolation)

For $0<p<1$, every prescribed state pattern on a finite [edge](graph-theory.md#edge-of-a-graph) [set](set.md) has positive conditional [probability](probability-theory.md#probability) given all exterior states: [independence](random-variable.md#independent-random-variables) makes it $p^a(1-p)^b$ for $a$ prescribed open and $b$ prescribed closed [edges](graph-theory.md#edge-of-a-graph). Thus a positive-probability exterior event remains possible after any finite local surgery. This is the [finite-energy property of Bernoulli percolation](#finite-energy-property-of-bernoulli-percolation), and applies equally to [dual bond percolation](planar-graph.md#dual-bond-percolation).

## Exponential decay of subcritical percolation

↑ **Parent:** [Percolation theory](percolation-theory.md)

Below the percolation threshold, the probability that a fixed vertex has an open path to graph distance $n$ is at most $Ce^{-cn}$ for positive constants $C,c$.

### Finite-set criterion for percolation sharpness

↑ **Parent:** [Exponential decay of subcritical percolation](#exponential-decay-of-subcritical-percolation)

For a finite vertex set $S$ containing the origin, this quantity is the expected number of potentially open exit edges reached from the origin within $S$. If $\varphi_p(S)<1$, the [BK inequality](bond-percolation.md#van-den-berg-kesten-inequality) applied to the first exit of a long open [self-avoiding walk](combinatorics.md#self-avoiding-walk) gives a contraction at the scale of $S$ and hence exponential connection decay. The threshold $\widetilde p_c=\sup\{p:\varphi_p(S)<1\text{ for some finite }S\ni0\}$ equals the [percolation critical probability](#percolation-critical-probability) by the pivotal-edge differential inequality in [sharpness of the percolation transition](#sharpness-of-the-percolation-transition).

### Exponential tail of subcritical cluster size

↑ **Parent:** [Exponential decay of subcritical percolation](#exponential-decay-of-subcritical-percolation)

For independent [bond percolation](bond-percolation.md) on $\mathbb Z^d$ below the [percolation critical probability](#percolation-critical-probability), there are $K,c>0$ such that $\mathbb P_p(|C(x)|\geq n)\leq Ke^{-cn}$, uniformly in $x$. This concerns the number of vertices in a [percolation cluster](bond-percolation.md#percolation-cluster), a stronger conclusion than decay of its radius alone.

## One-arm event

↑ **Parent:** [Percolation theory](percolation-theory.md)

The one-arm event $A_R$ is the event that a specified root is joined through open vertices or edges to graph distance $R$.

## OSSS inequality

↑ **Parent:** [Percolation theory](percolation-theory.md)

For a Boolean function of independent coordinates and a randomized [decision tree](theoretical-computer-science.md#decision-tree) that determines it, the OSSS inequality bounds its variance by a sum of coordinate influences weighted by their revealment probabilities.

### OSSS exploration of a one-arm event

↑ **Parent:** [OSSS inequality](#osss-inequality)

Choosing an intermediate radius uniformly and exploring the open cluster meeting that sphere gives a decision tree for a [one-arm event](#one-arm-event). Translation and a union bound control each revealment by a constant times the average of the one-arm probabilities over the possible radii.

## ↑ Ancestors (5)

1. [Probability theory](probability-theory.md)
2. [Probability and statistics](probability-and-statistics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Bond percolation](bond-percolation.md)
