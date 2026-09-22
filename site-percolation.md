# Site percolation

↑ **Parent:** [Percolation theory](probability-theory.md#percolation-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Site_percolation)

In site percolation, vertices are declared open or closed and one studies connected components of the induced open subgraph.

**Table of contents**

- [Critical probability for site percolation on the triangular lattice](#critical-probability-for-site-percolation-on-the-triangular-lattice)
- [Domain Markov property of a percolation exploration](#domain-markov-property-of-a-percolation-exploration)
- [Dependent percolation](#dependent-percolation)
  - [One-independent bond percolation](#one-independent-bond-percolation)
    - [Separated-block percolation renormalization](#separated-block-percolation-renormalization)
    - [Peierls circuit bound for one-independent percolation](#peierls-circuit-bound-for-one-independent-percolation)
  - [Monochromatic line-graph percolation counterexample](#monochromatic-line-graph-percolation-counterexample)
  - [Random-cluster model](#random-cluster-model)
    - [Bernoulli bounds for the random-cluster model](#bernoulli-bounds-for-the-random-cluster-model)
    - [Cluster weight in the random-cluster model](#cluster-weight-in-the-random-cluster-model)
    - [Random-cluster critical probability](#random-cluster-critical-probability)
      - [Monotonicity of random-cluster critical probability in cluster weight](#monotonicity-of-random-cluster-critical-probability-in-cluster-weight)
    - [Random-cluster weight monotonicity](#random-cluster-weight-monotonicity)
    - [Self-dual parameter of the random-cluster model](#self-dual-parameter-of-the-random-cluster-model)
      - [Symmetric cluster weight at the self-dual parameter](#symmetric-cluster-weight-at-the-self-dual-parameter)
    - [Random-cluster single-edge conditional probability](#random-cluster-single-edge-conditional-probability)
    - [Random-cluster boundary condition](#random-cluster-boundary-condition)
      - [Boundary monotonicity of the random-cluster measure](#boundary-monotonicity-of-the-random-cluster-measure)
      - [Wired random-cluster boundary condition](#wired-random-cluster-boundary-condition)
        - [Infinite-volume wired random-cluster measure](#infinite-volume-wired-random-cluster-measure)
          - [Random-cluster inverse correlation length](#random-cluster-inverse-correlation-length)
            - [Reflection comparison of random-cluster connections](#reflection-comparison-of-random-cluster-connections)
      - [Free random-cluster boundary condition](#free-random-cluster-boundary-condition)
    - [Positive association of the random-cluster model](#positive-association-of-the-random-cluster-model)
    - [Uniform connected-subgraph limit of the random-cluster model](#uniform-connected-subgraph-limit-of-the-random-cluster-model)
    - [Uniform spanning-tree limit of the random-cluster model](#uniform-spanning-tree-limit-of-the-random-cluster-model)
    - [Edwards-Sokal coupling](#edwards-sokal-coupling)
      - [Spin-connectivity identity for the Potts model](#spin-connectivity-identity-for-the-potts-model)
    - [Heat-bath Markov chain](#heat-bath-markov-chain)
  - [Level-set percolation](#level-set-percolation)
    - [Critical threshold for level-set percolation](#critical-threshold-for-level-set-percolation)
  - [Finite-range dependent random field](#finite-range-dependent-random-field)

## Critical probability for site percolation on the triangular lattice

↑ **Parent:** [Site percolation](site-percolation.md)

For independent site percolation on the triangular lattice, the critical probability is $p_c=1/2$. Self-duality, crossing estimates, and exclusion of an infinite critical cluster identify the threshold.

## Domain Markov property of a percolation exploration

↑ **Parent:** [Site percolation](site-percolation.md)

Conditioned on the sites revealed by an exploration interface, every unrevealed site retains its independent Bernoulli law. The explored boundary supplies boundary conditions for subsequent crossing events.

## Dependent percolation

↑ **Parent:** [Site percolation](site-percolation.md)

Dependent percolation allows the open states of different vertices or edges to be statistically dependent.

### One-independent bond percolation

↑ **Parent:** [Dependent percolation](#dependent-percolation)

A [bond percolation](bond-percolation.md) law is one-independent if the bond states in any two sets with disjoint endpoint sets are independent as collections. In particular, states of bonds in a [matching in a graph](graph-theory.md#matching-graph-theory) are mutually independent. The law need not be invariant under translations or positively associated.

#### Separated-block percolation renormalization

↑ **Parent:** [One-independent bond percolation](#one-independent-bond-percolation)

Place side-$2n$ [square lattice](graph.md#square-lattice) boxes around the points $3nv$, $v\in\mathbb Z^2$. The width-$2n$ rectangle joining adjacent boxes has length $5n$. Declare a coarse bond open when its long rectangle is crossed and each endpoint box is crossed in the transverse direction. Nonincident coarse bonds use disjoint fine-bond sets, while incident good bonds give connected open paths inside their common endpoint box. When fixed-aspect crossing probabilities tend to one, these coarse bond probabilities tend to one. The [Peierls circuit bound for one-independent percolation](#peierls-circuit-bound-for-one-independent-percolation) then yields an infinite fine-lattice open cluster.

#### Peierls circuit bound for one-independent percolation

↑ **Parent:** [One-independent bond percolation](#one-independent-bond-percolation)

If each bond has closed probability at most $q$ in [one-independent bond percolation](#one-independent-bond-percolation) on the [square lattice](graph.md#square-lattice), a set of $\ell$ bonds contains a [matching in a graph](graph-theory.md#matching-graph-theory) of size at least $\ell/4$: divide horizontal bonds by the parity of their left endpoint and vertical bonds by the parity of their lower endpoint. Each of the four classes is a matching. Mutual independence in the largest class proves the circuit bound. There are at most $4\ell3^\ell$ dual circuits of length $\ell$ surrounding the origin. For sufficiently small $q$, the sum of these circuit probabilities is less than one, so the origin has a positive chance of belonging to an [infinite percolation cluster](bond-percolation.md#infinite-percolation-cluster).

### Monochromatic line-graph percolation counterexample

↑ **Parent:** [Dependent percolation](#dependent-percolation)

Color the vertices of a periodic [graph](graph.md) independently red or blue with equal [probabilities](probability-theory.md#probability), and declare a vertex of its [line graph](graph-theory.md#line-graph) open exactly when the corresponding edge has equal-colored endpoints. The resulting [site percolation](site-percolation.md) has marginal $1/2$ and is a [finite-range dependent random field](#finite-range-dependent-random-field): sets at line-graph distance greater than one use disjoint color inputs. Red and blue open clusters cannot join. If the original graph has an infinite red component and an infinite blue component, its [line graph](graph-theory.md#line-graph) consequently has at least two [infinite percolation clusters](bond-percolation.md#infinite-percolation-cluster). One explicit [amenable graph](graph.md#amenable-graph) with that property is obtained by replacing each square-lattice vertex by a [complete graph](graph-theory.md#complete-graph) on ten vertices, joining neighboring blocks completely. Blocks containing both colors have independent probability $511/512$; a [Peierls argument](probability-theory.md#peierls-argument) proves that they percolate, and their infinite cluster carries both a red and a blue component. Thus finite-range dependence, even with all site marginals nondegenerate, does not substitute for finite energy in percolation uniqueness.

### Random-cluster model

↑ **Parent:** [Dependent percolation](#dependent-percolation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Random-cluster_model)

On a finite graph, the random-cluster model assigns an edge configuration $\omega$ probability proportional to

$$
p^{o(\omega)}(1-p)^{c(\omega)}q^{k(\omega)},
$$

where $o,c,k$ count open edges, closed edges, and open connected components.

#### Bernoulli bounds for the random-cluster model

↑ **Parent:** [Random-cluster model](#random-cluster-model)

For $q\geq1$, the [random-cluster measure](#random-cluster-model) lies between the two [Bernoulli](discrete-probability-distribution.md#bernoulli-distribution) product measures displayed above. The upper [Holley condition](probability-and-statistics.md#holley-condition) ratio is $q^{k(\omega\wedge\eta)-k(\eta)}\geq1$. The lower ratio is $q^{k(\omega\vee\eta)-k(\omega)+|\eta\setminus\omega|}\geq1$, because adding an edge reduces the component count by at most one. The comparisons persist under wired limits and give $p_c(1)\leq p_c(q)\leq qp_c(1)/(1+(q-1)p_c(1))$.

#### Cluster weight in the random-cluster model

↑ **Parent:** [Random-cluster model](#random-cluster-model)

The multiplicative factor $q$ assigned to each [connected component of a graph](graph.md#component-graph-theory) in a finite [random-cluster measure](#random-cluster-model). At fixed [edge](graph-theory.md#edge-of-a-graph) [probability](probability-theory.md#probability), the weight of a configuration with $k$ components includes $q^k$. For $q=1$ this reduces to independent [bond percolation](bond-percolation.md); increasing $q$ at fixed $p$, for $q\ge1$, suppresses [increasing events](probability-inequality.md#increasing-event) by [random-cluster weight monotonicity](#random-cluster-weight-monotonicity).

#### Random-cluster critical probability

↑ **Parent:** [Random-cluster model](#random-cluster-model)

The threshold for the origin to have an [infinite percolation cluster](bond-percolation.md#infinite-percolation-cluster) under a consistently chosen infinite-volume [random-cluster measure](#random-cluster-model), conventionally the wired measure: $p_c(q)=\inf\{p:\theta^{\mathrm w}(p,q)>0\}$. The definition alone makes no assertion about percolation exactly at the threshold.

##### Monotonicity of random-cluster critical probability in cluster weight

↑ **Parent:** [Random-cluster critical probability](#random-cluster-critical-probability)

The finite-volume [random-cluster weight monotonicity](#random-cluster-weight-monotonicity) passes to consistently wired or free infinite-volume measures for finite increasing connection events. Decreasing these events to origin-to-infinity connectivity yields $\theta(p,q_1)\ge\theta(p,q_2)$ for $q_1\le q_2$. The corresponding supercritical parameter sets are nested, and hence $p_c(q_1)\le p_c(q_2)$.

#### Random-cluster weight monotonicity

↑ **Parent:** [Random-cluster model](#random-cluster-model)

For fixed $p\in(0,1)$ and $1\le q_1\le q_2$, the [random-cluster measure](#random-cluster-model) at $q_1$ [stochastically dominates](probability-and-statistics.md#stochastic-domination-of-probability-measures) that at $q_2$. In [Holley's condition](probability-and-statistics.md#holley-condition), Bernoulli factors cancel. Put $a=k(S)-k(S\cup T)$ and $b=k(S\cap T)-k(T)$; [supermodularity of graph component count](graph.md#supermodularity-of-graph-component-count) gives $b\ge a\ge0$, and the weight ratio is $(q_2/q_1)^a q_2^{b-a}\ge1$. The comparison also holds with the same boundary wiring in both measures.

#### Self-dual parameter of the random-cluster model

↑ **Parent:** [Random-cluster model](#random-cluster-model)

Planar random-cluster duality relates edge odds by $[p/(1-p)][p^*/(1-p^*)]=q$. The fixed point $p=p^*$ has odds $\sqrt q$, giving the displayed parameter. A self-dual parameter does not by itself establish a critical threshold on an arbitrary [planar graph](graph-theory.md#planar-graph). At this parameter the [symmetric cluster weight at the self-dual parameter](#symmetric-cluster-weight-at-the-self-dual-parameter) makes the primal-dual cluster counts explicit.

##### Symmetric cluster weight at the self-dual parameter

↑ **Parent:** [Self-dual parameter of the random-cluster model](#self-dual-parameter-of-the-random-cluster-model)

The [planar cluster-count identity](graph-theory.md#planar-cluster-count-identity) rewrites $o(\omega)+2k(\omega)$ as $|V|-1+k(\omega)+k(\bar\omega^*)$. At the [self-dual parameter of the random-cluster model](#self-dual-parameter-of-the-random-cluster-model), $p/(1-p)=\sqrt q$, so its weight is $(\sqrt q)^{o(\omega)+2k(\omega)}$ up to a configuration-independent factor. Absorbing $(\sqrt q)^{|V|-1}$ into normalization proves the symmetric weight, with the unbounded dual face counted.

#### Random-cluster single-edge conditional probability

↑ **Parent:** [Random-cluster model](#random-cluster-model)

For an edge with endpoints already connected without that edge, including any boundary wiring, the conditional open [probability](probability-theory.md#probability) is $p$. Otherwise opening the edge merges two components, so the [conditional probability](probability-theory.md#conditional-probability) is $p/(p+q(1-p))$. For $q\geq1$, this [conditional probability](probability-theory.md#conditional-probability) increases when more other edges are open or more boundary vertices are identified. This is the local mechanism of [boundary monotonicity of the random-cluster measure](#boundary-monotonicity-of-the-random-cluster-measure).

#### Random-cluster boundary condition

↑ **Parent:** [Random-cluster model](#random-cluster-model)

A boundary condition for a finite-box [random-cluster measure](#random-cluster-model) is a partition of the boundary vertices. All vertices in one block are identified before counting open components; the identifications carry no Bernoulli edge factors. The weight is $p^{o(\omega)}(1-p)^{|E|-o(\omega)}q^{k_\xi(\omega)}$. A coarser partition makes more identifications. General partitions need not have a planar realization.

##### Boundary monotonicity of the random-cluster measure

↑ **Parent:** [Random-cluster boundary condition](#random-cluster-boundary-condition)

Here $\xi\preceq\zeta$ means each block of $\xi$ lies in a block of $\zeta$, and the measure order is [stochastic domination of probability measures](probability-and-statistics.md#stochastic-domination-of-probability-measures). The [random-cluster single-edge conditional probability](#random-cluster-single-edge-conditional-probability) is increasing in both exterior open edges and wiring for $q\geq1$. Couple two [heat-bath Markov chains](#heat-bath-markov-chain) by identical update edges and uniform random variables, starting from ordered states. Order persists, and convergence of the finite chains to their stationary laws proves the displayed inequality. At $q=1$, the law does not depend on the boundary partition.

##### Wired random-cluster boundary condition

↑ **Parent:** [Random-cluster boundary condition](#random-cluster-boundary-condition)

All boundary vertices are identified into one vertex for component counting. This is the most wired [random-cluster boundary condition](#random-cluster-boundary-condition) on a fixed boundary, and maximizes increasing-event [probabilities](probability-theory.md#probability) when $q\geq1$ by [boundary monotonicity of the random-cluster measure](#boundary-monotonicity-of-the-random-cluster-measure).

###### Infinite-volume wired random-cluster measure

↑ **Parent:** [Wired random-cluster boundary condition](#wired-random-cluster-boundary-condition)

For $q\ge1$, finite [random-cluster measures](#random-cluster-model) with all boundary [graph vertices](graph.md#vertex-graph-theory) identified have a weak infinite-volume [limit of a sequence](real-analysis.md#limit-of-a-sequence). On a regular [lattice](mathematical-logic.md#lattice) it is invariant under translations and [lattice](mathematical-logic.md#lattice) reflections and has [positive association of the random-cluster model](#positive-association-of-the-random-cluster-model). Its conditional single-edge open [probability](probability-theory.md#probability) lies between $p/(p+q(1-p))$ and $p$. Connection events can be approximated by increasing finite-volume path events, so their positive-association inequalities pass to the [limit of a sequence](real-analysis.md#limit-of-a-sequence).

###### Random-cluster inverse correlation length

↑ **Parent:** [Infinite-volume wired random-cluster measure](#infinite-volume-wired-random-cluster-measure)

[Positive association of random variables](probability-theory.md#positive-association-of-random-variables) and [translation invariance](physics.md#translation-invariance) give $C_{m+n}\ge C_mC_n$ for axis connection [probabilities](probability-theory.md#probability). The [Fekete lemma](real-analysis.md#fekete-s-lemma) applied to $-\log C_n$ proves the displayed [limit of a sequence](real-analysis.md#limit-of-a-sequence) and the bound $C_n\le e^{-n\alpha}$. The lower single-edge conditional bound gives $C_n\ge[p/(p+q(1-p))]^n$, so the decay rate is finite and nonnegative. It may be zero.

###### Reflection comparison of random-cluster connections

↑ **Parent:** [Random-cluster inverse correlation length](#random-cluster-inverse-correlation-length)

Choose a [graph vertex](graph.md#vertex-graph-theory) $x=(n,x_2,\ldots,x_d)$ on the boundary of a [lattice](mathematical-logic.md#lattice) box. Translation and reflection invariance identify the [probabilities](probability-theory.md#probability) of $0\leftrightarrow x$ and $x\leftrightarrow2ne_1$. Their intersection implies $0\leftrightarrow2ne_1$, so [positive association of random variables](probability-theory.md#positive-association-of-random-variables) gives $C_{2n}\ge\phi(0\leftrightarrow x)^2$. A [union bound](probability-inequality.md#boole-s-inequality) and [lattice](mathematical-logic.md#lattice) symmetries choose such an $x$ with [probability](probability-theory.md#probability) at least the box-boundary connection [probability](probability-theory.md#probability) divided by the number of boundary [graph vertices](graph.md#vertex-graph-theory). This polynomial factor disappears in the exponential rate, identifying boundary and axial inverse correlation lengths.

##### Free random-cluster boundary condition

↑ **Parent:** [Random-cluster boundary condition](#random-cluster-boundary-condition)

The boundary partition has singleton blocks, so no different boundary vertices are identified. Open component counting is the ordinary counting in the finite graph, including isolated vertices. This is the least wired [random-cluster boundary condition](#random-cluster-boundary-condition).

#### Positive association of the random-cluster model

↑ **Parent:** [Random-cluster model](#random-cluster-model)

For $0\leq p\leq1$ and $q\geq1$, the [FKG inequality](probability-inequality.md#fkg-inequality) implies that increasing functions of a random-cluster configuration have nonnegative covariance. The conclusion can fail for $0<q<1$.

#### Uniform connected-subgraph limit of the random-cluster model

↑ **Parent:** [Random-cluster model](#random-cluster-model)

On a finite connected graph, fixing $p=1/2$ and sending $q\downarrow0$ makes the random-cluster model converge to the uniform law on connected spanning subgraphs: the factor $q^{k(\omega)}$ selects the minimum possible component count $k=1$, while all surviving configurations have equal remaining weight.

#### Uniform spanning-tree limit of the random-cluster model

↑ **Parent:** [Random-cluster model](#random-cluster-model)

If $p,q\downarrow0$ with $q/p\to0$, the random-cluster model on a finite connected graph converges to the [uniform spanning tree](combinatorics.md#uniform-spanning-tree). Relative to a tree, an acyclic configuration with $k>1$ components pays a factor $(q/p)^{k-1}$, while every additional cycle pays a factor asymptotic to $p$.

#### Edwards-Sokal coupling

↑ **Parent:** [Random-cluster model](#random-cluster-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Edwards-Sokal_coupling)

The Edwards-Sokal coupling assigns one common random spin to every random-cluster component. For $q=2$ it couples the random-cluster model to the [Ising model](statistical-physics.md#ising-model).

##### Spin-connectivity identity for the Potts model

↑ **Parent:** [Edwards-Sokal coupling](#edwards-sokal-coupling)

Given a [random-cluster](#random-cluster-model) configuration, its components receive independent uniform colors under the [Edwards-Sokal coupling](#edwards-sokal-coupling). Two vertices have equal [Potts](statistical-physics.md#potts-model) spins with probability $1$ if connected and $1/q$ otherwise. Averaging proves the identity. With a wired component fixed to color $1$, the same argument gives normalized [spontaneous magnetization](statistical-physics.md#spontaneous-magnetization) $(q\pi^1(\sigma_0=1)-1)/(q-1)=\phi^{\rm w}(0\leftrightarrow\infty)$ in infinite volume. Thus its onset is the wired [random-cluster critical probability](#random-cluster-critical-probability), transformed to $\beta_c=-\log(1-p_c)$ in this convention.

#### Heat-bath Markov chain

↑ **Parent:** [Random-cluster model](#random-cluster-model)

A heat-bath Markov chain repeatedly chooses one coordinate and redraws it from its conditional distribution given all other coordinates. The target distribution is reversible and stationary for these updates.

### Level-set percolation

↑ **Parent:** [Dependent percolation](#dependent-percolation)

For a random field $(Y_x)$, level-set percolation studies the random vertex set $\{x:Y_x\geq a\}$ as the threshold $a$ varies.

#### Critical threshold for level-set percolation

↑ **Parent:** [Level-set percolation](#level-set-percolation)

The critical threshold is the boundary between levels at which an unbounded superlevel component can occur and levels at which every superlevel component is almost surely finite.

### Finite-range dependent random field

↑ **Parent:** [Dependent percolation](#dependent-percolation)

A random field is finite-range dependent if collections indexed by sets farther apart than a fixed distance are independent. Sparse subsets of long paths then restore enough independence for path-counting arguments.

## ↑ Ancestors (6)

1. [Percolation theory](probability-theory.md#percolation-theory)
2. [Probability theory](probability-theory.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (26)

- [Conformal invariance of planar percolation](probability-theory.md#conformal-invariance-of-planar-percolation)
- [Directed percolation](probability-theory.md#directed-percolation)
- [Encounter box in percolation](bond-percolation.md#encounter-box-in-percolation)
- [Monochromatic line-graph percolation counterexample](#monochromatic-line-graph-percolation-counterexample)
- [Parallel-bond ray with different site and bond thresholds](probability-theory.md#parallel-bond-ray-with-different-site-and-bond-thresholds)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-39.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-26.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-204.md#2/a/solution)
- [Percolation cluster](bond-percolation.md#percolation-cluster)
- [Percolation uniqueness on an amenable quasi-transitive graph](bond-percolation.md#percolation-uniqueness-on-an-amenable-quasi-transitive-graph)
- [Percolation universality hypothesis](critical-phenomenon.md#percolation-universality-hypothesis)
- [Right continuity of percolation probability](probability-theory.md#right-continuity-of-percolation-probability)
- [Supercritical continuity of percolation probability](probability-theory.md#supercritical-continuity-of-percolation-probability)
- [Survival and susceptibility thresholds for directed percolation](probability-theory.md#survival-and-susceptibility-thresholds-for-directed-percolation)
- [Triangular lattice](graph.md#triangular-lattice)
- [Uniqueness of the infinite percolation cluster](bond-percolation.md#uniqueness-of-the-infinite-percolation-cluster)
