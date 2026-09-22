# Matching (graph theory)

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matching_(graph_theory))

A [matching in a graph](matching-graph-theory.md) is a [set](set.md) $M$ of [edges](graph-theory.md#edge-of-a-graph) of an [undirected graph](graph-theory.md#undirected-graph) with no shared endpoints: each [vertex](graph.md#vertex-graph-theory) has capacity for at most one selected [edge](graph-theory.md#edge-of-a-graph). It describes simultaneous compatible pairs, such as jobs assigned to distinct available workers, or tasks each occupying two resources that cannot be shared. The empty [set](set.md) is a valid [matching in a graph](matching-graph-theory.md).[Matching, Covering and Packing, opening paragraph, printed p. 1: independent edges and matchings](mathematics-bibliography.md#graph-theory-by-reinhard-diestel)

For a finite [simple graph](graph.md#simple-graph) $G=(V,E)$, write $x_e=1$ when $e$ is selected and $x_e=0$ otherwise. The vertex capacity constraint is exactly

$$
x_e\in\{0,1\}\quad(e\in E),\qquad
\sum_{e\in E:\,v\in e}x_e\leq1\quad(v\in V).
$$

These are constraints on a discrete selection, not a requirement that every [vertex](graph.md#vertex-graph-theory) be used. A [matching in a graph](matching-graph-theory.md) with [matching saturation](#matching-saturation) of all [vertices](graph.md#vertex-graph-theory) is a [perfect matching](#perfect-matching); an [unmatched vertex in a matching](#unmatched-vertex-in-a-matching) uses none of its capacity.

The objective must be specified separately. A [maximum cardinality matching](#maximum-cardinality-matching) selects as many [edges](graph-theory.md#edge-of-a-graph) as possible; a [maximum-weight matching](#maximum-weight-matching) selects the greatest total benefit; a [minimum-weight perfect matching](#minimum-weight-perfect-matching) minimizes cost while requiring every [vertex](graph.md#vertex-graph-theory) to be paired. A [maximal matching](#maximal-matching) only says that no additional [edge](graph-theory.md#edge-of-a-graph) fits alongside the current choices. The four-[vertex](graph.md#vertex-graph-theory) [path graph](graph-theory.md#path-graph) below separates these notions: choosing the middle [edge](graph-theory.md#edge-of-a-graph) blocks both outer [edges](graph-theory.md#edge-of-a-graph), yet replacing it by those two [edges](graph-theory.md#edge-of-a-graph) pairs more [vertices](graph.md#vertex-graph-theory).

This model is useful because conflicts are local at [vertices](graph.md#vertex-graph-theory), while the quality of a selection can depend on coordinated changes along a whole [augmenting path in a matching](#augmenting-path-in-a-matching). A [greedy matching](#greedy-matching) gives a quick feasible selection; [Berge's theorem](#berge-s-theorem) explains when searching for such changes has reached a [maximum cardinality matching](#maximum-cardinality-matching). Repeating the pairing problem over time leads instead to [proper edge colouring](graph-coloring.md#proper-edge-coloring), where each time slot is a [matching in a graph](matching-graph-theory.md).

**Table of contents**

- [Unmatched vertex in a matching](#unmatched-vertex-in-a-matching)
- [Matching saturation](#matching-saturation)
- [Stable matching in a bipartite graph](#stable-matching-in-a-bipartite-graph)
  - [Mutual-worst edge in stable matchings](#mutual-worst-edge-in-stable-matchings)
  - [Gale-Shapley algorithm](#gale-shapley-algorithm)
    - [Proposer-optimal stable matching](#proposer-optimal-stable-matching)
      - [Receiver-pessimal stable matching](#receiver-pessimal-stable-matching)
  - [Blocking pair in stable matching](#blocking-pair-in-stable-matching)
- [Near-perfect matching](#near-perfect-matching)
- [Matching generating function](#matching-generating-function)
  - [Annealing ratios for a matching generating function](#annealing-ratios-for-a-matching-generating-function)
- [Alternating path in a matching](#alternating-path-in-a-matching)
- [Augmenting path in a matching](#augmenting-path-in-a-matching)
  - [Berge's theorem](#berge-s-theorem)
  - [Short augmenting paths in a dense bipartite graph](#short-augmenting-paths-in-a-dense-bipartite-graph)
- [Perfect matching](#perfect-matching)
  - [Flexible vertex in a balanced bipartite graph](#flexible-vertex-in-a-balanced-bipartite-graph)
  - [Minimum-weight perfect matching](#minimum-weight-perfect-matching)
  - [One-factorization](#one-factorization)
- [Maximal matching](#maximal-matching)
  - [Greedy matching](#greedy-matching)
- [Matching number](#matching-number)
- [Maximum cardinality matching](#maximum-cardinality-matching)
- [Maximum-weight matching](#maximum-weight-matching)
- [Hall's marriage theorem](#hall-s-marriage-theorem)
  - [Hall condition](#hall-condition)
    - [Hall obstruction](#hall-obstruction)
  - [Hall allocation model](#hall-allocation-model)
  - [System of distinct representatives](#system-of-distinct-representatives)
  - [Hall theorem proof outline](#hall-theorem-proof-outline)
  - [Random bipartite matching from empty-rectangle exclusion](#random-bipartite-matching-from-empty-rectangle-exclusion)
  - [Hall matching of maximal separated sets](#hall-matching-of-maximal-separated-sets)
  - [Degree-weighted Hall condition](#degree-weighted-hall-condition)
  - [Measurable Hall theorem](#measurable-hall-theorem)
  - [Hall induction through a tight set](#hall-induction-through-a-tight-set)
  - [Regular bipartite graph has a perfect matching](#regular-bipartite-graph-has-a-perfect-matching)
- [Regular-graph matching bound from unmatched vertices](#regular-graph-matching-bound-from-unmatched-vertices)
  - [Disjoint union of triangles as a sharp matching example](#disjoint-union-of-triangles-as-a-sharp-matching-example)

## Unmatched vertex in a matching

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)

A [vertex](graph.md#vertex-graph-theory) is an [unmatched vertex in a matching](#unmatched-vertex-in-a-matching) $M$ if no [edge](graph-theory.md#edge-of-a-graph) of $M$ is incident to it. It is also called free or exposed, always relative to the specified [matching in a graph](matching-graph-theory.md): changing $M$ can change which [vertices](graph.md#vertex-graph-theory) are free. The endpoints of an [augmenting path in a matching](#augmenting-path-in-a-matching) must be distinct [unmatched vertices in a matching](#unmatched-vertex-in-a-matching) before the change.

## Matching saturation

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)

A [matching in a graph](matching-graph-theory.md) saturates a specified [vertex set](graph.md#vertex-set) $X$ when every [vertex](graph.md#vertex-graph-theory) of $X$ is incident to one selected [edge](graph-theory.md#edge-of-a-graph). Exactly one selected [edge](graph-theory.md#edge-of-a-graph) meets each such [vertex](graph.md#vertex-graph-theory), since matching [edges](graph-theory.md#edge-of-a-graph) have disjoint endpoints. [Vertices](graph.md#vertex-graph-theory) outside $X$ may remain unmatched. A [perfect matching](#perfect-matching) saturates the entire [vertex set](graph.md#vertex-set); [Hall's marriage theorem](#hall-s-marriage-theorem) tests [matching saturation](#matching-saturation) of a specified side in a finite [bipartite graph](bipartite-graph.md).

## Stable matching in a bipartite graph

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)

A [stable matching in a bipartite graph](#stable-matching-in-a-bipartite-graph) pairs two groups so that no acceptable unpaired pair would both rather be together. Give a finite [bipartite graph](bipartite-graph.md) $G=(L\cup R,E)$ a [strict preference](set-theory.md#strict-preference) ordering at each [vertex](graph.md#vertex-graph-theory) over its [neighbours of a vertex](graph-theory.md#neighbour-of-a-vertex). An [edge](graph-theory.md#edge-of-a-graph) means that both endpoints regard the pair as acceptable; every acceptable partner ranks above being unmatched. Lists may be incomplete, and $L$ and $R$ may have unequal [cardinalities](cardinal-number.md#cardinality). A [matching in a graph](matching-graph-theory.md) $M\subseteq E$ is stable when it has no [blocking pair in stable matching](#blocking-pair-in-stable-matching).

Write $M(v)$ for the partner of a [vertex](graph.md#vertex-graph-theory) $v$, or $\bot$ if $v$ is an [unmatched vertex in a matching](#unmatched-vertex-in-a-matching). An unused [edge](graph-theory.md#edge-of-a-graph) $(\ell,r)$ is a [blocking pair in stable matching](#blocking-pair-in-stable-matching) precisely when

$$
r\succ_\ell M(\ell)\quad\text{and}\quad \ell\succ_r M(r),
$$

where $\succ_v$ denotes the [strict preference](set-theory.md#strict-preference) at $v$ and $\bot$ ranks below every [neighbour of a vertex](graph-theory.md#neighbour-of-a-vertex). Both inequalities matter: wanting a different partner alone cannot upset a [stable matching](#stable-matching-in-a-bipartite-graph). A [stable matching](#stable-matching-in-a-bipartite-graph) need not be a [perfect matching](#perfect-matching); the [Gale-Shapley algorithm](#gale-shapley-algorithm) still finds one with incomplete lists and unequal sides.

Here is an original example on the [complete bipartite graph](bipartite-graph.md#complete-bipartite-graph) $K_{3,3}$, with $L=\{A,B,C\}$ and $R=\{X,Y,Z\}$. Read each row from best to worst:

$$
\begin{array}{c|ccc|c|ccc}
\text{left}&1&2&3&\text{right}&1&2&3\\\hline
A&X&Y&Z&X&C&A&B\\
B&X&Y&Z&Y&A&B&C\\
C&Y&Z&X&Z&A&B&C
\end{array}
$$

There are two [stable matchings](#stable-matching-in-a-bipartite-graph),

$$
M_L=\{(A,X),(B,Y),(C,Z)\},\qquad
M_R=\{(A,Y),(B,Z),(C,X)\}.
$$

For $M_L$, the only unpaired partners preferred by left [vertices](graph.md#vertex-graph-theory) are $B$ wanting $X$ and $C$ wanting $Y$. But $X$ prefers its partner $A$ to $B$, and $Y$ prefers its partner $B$ to $C$. Hence neither is a [blocking pair in stable matching](#blocking-pair-in-stable-matching). For $M_R$, the left [vertices](graph.md#vertex-graph-theory) want $A$ with $X$, $B$ with $X$ or $Y$, and $C$ with $Y$ or $Z$. In every case the right [vertex](graph.md#vertex-graph-theory) prefers its current partner: $X$ has $C$, $Y$ has $A$, and $Z$ has $B$.

By contrast, $N=\{(A,X),(B,Z),(C,Y)\}$ is a [perfect matching](#perfect-matching) with a [blocking pair in stable matching](#blocking-pair-in-stable-matching) $(B,Y)$: $B$ prefers $Y$ to $Z$, while $Y$ prefers $B$ to $C$. The abandoned partners need not agree to the change; stability tests the incentives of the two endpoints of the unused [edge](graph-theory.md#edge-of-a-graph).

<a id="image-one-blocking-pair-in-stable-matching-and-two-stable-matchings-for-the-same-strict-preference-lists"></a>
![](stable-matching-blocking-pair-comparison.png)

**[Figure 1](#image-one-blocking-pair-in-stable-matching-and-two-stable-matchings-for-the-same-strict-preference-lists). One blocking pair in stable matching and two stable matchings for the same strict preference lists**.

There are $3!=6$ [permutations](combinatorics.md#permutation) of right partners. The following table lists every [blocking pair in stable matching](#blocking-pair-in-stable-matching) for each [perfect matching](#perfect-matching); the middle column gives the partners of $A,B,C$ in that order:

$$
\begin{array}{c|c|l}
& (M(A),M(B),M(C))&\text{blocking pairs}\\\hline
M_L&(X,Y,Z)&\text{none}\\
N&(X,Z,Y)&(B,Y)\\
&(Y,X,Z)&(A,X)\\
M_R&(Y,Z,X)&\text{none}\\
&(Z,X,Y)&(A,X),\ (A,Y)\\
&(Z,Y,X)&(A,Y)
\end{array}
$$

This exhausts the [stable matchings](#stable-matching-in-a-bipartite-graph): any nonperfect [matching in a graph](matching-graph-theory.md) here leaves an unmatched [vertex](graph.md#vertex-graph-theory) on each side, and those two form a [blocking pair in stable matching](#blocking-pair-in-stable-matching) because every cross-pair is acceptable. Notice that every left [vertex](graph.md#vertex-graph-theory) prefers $M_L$ and every right [vertex](graph.md#vertex-graph-theory) prefers $M_R$. Stability can accommodate opposing interests without selecting a single universally preferred outcome.

A [stable matching](#stable-matching-in-a-bipartite-graph) addresses the possibility of mutually beneficial departures. Its definition contains no numerical total social benefit or [maximum-weight matching](#maximum-weight-matching) objective. For example, assigning benefit $100$ to each [edge](graph-theory.md#edge-of-a-graph) of $N$ and zero to every other [edge](graph-theory.md#edge-of-a-graph) makes $N$ the unique [maximum-weight matching](#maximum-weight-matching), yet $(B,Y)$ still blocks it under the displayed [preference relations](set-theory.md#preference-relation). Such external benefits need not represent participants' rankings.

### Mutual-worst edge in stable matchings

↑ **Parent:** [Stable matching in a bipartite graph](#stable-matching-in-a-bipartite-graph)

If the endpoints of an [edge](graph-theory.md#edge-of-a-graph) rank one another last and one [stable matching in a bipartite graph](#stable-matching-in-a-bipartite-graph) contains that edge, every stable matching contains it. In the symmetric difference of two stable matchings, preference comparisons propagate along alternating paths: if a vertex prefers its new partner, that partner must prefer its old partner to avoid blocking the old matching. An alternating path cannot end unmatched on the preferred side, so the component is an alternating cycle, on which the two parts prefer opposite matchings. A mutual-worst edge absent from the new matching would make both its endpoints prefer the new matching, contradicting this propagation.

### Gale-Shapley algorithm

↑ **Parent:** [Stable matching in a bipartite graph](#stable-matching-in-a-bipartite-graph)

The [Gale-Shapley algorithm](#gale-shapley-algorithm) constructs a [stable matching](#stable-matching-in-a-bipartite-graph) by letting one side propose and the other hold its best offer so far. The word "deferred" is essential: a held proposal is tentative and can be replaced. [David Gale](mathematics.md#david-gale) and [Lloyd Shapley](mathematics.md#lloyd-shapley) presented this construction in their 1962 paper, [College Admissions and the Stability of Marriage](https://iqua.ece.toronto.edu/baochun/ece1771f/papers/Gale-Shapley-1962.pdf), §3, printed pp. 12–13; §4 extends it to college quotas and unacceptable pairs.

For the one-partner [bipartite graph](bipartite-graph.md) model, designate $L$ as proposers and $R$ as receivers:
- Start with the empty [matching in a graph](matching-graph-theory.md). Each proposer keeps a pointer to its first untried acceptable partner.
- Choose an [unmatched vertex in a matching](#unmatched-vertex-in-a-matching) $\ell\in L$ whose list is not exhausted. It proposes to its highest-ranked untried [neighbour of a vertex](graph-theory.md#neighbour-of-a-vertex) $r$ and advances its pointer permanently.
- If $r$ holds nobody, it holds $\ell$. Otherwise $r$ compares $\ell$ with its currently held proposer, keeps the one it prefers, and rejects the other. A displaced proposer becomes unmatched and may propose again later.
- Stop when every unmatched proposer has exhausted its list. The held pairs are the output [matching in a graph](matching-graph-theory.md).

Held proposers wait; only unmatched proposers act. A receiver can replace its held partner, whereas a proposer never tries the same [edge](graph-theory.md#edge-of-a-graph) twice. Isolated [vertices](graph.md#vertex-graph-theory) simply remain unmatched. These rules also describe incomplete acceptable lists and unequal sides without adding fictitious acceptable partners.

For the preference lists under [stable matching](#stable-matching-in-a-bipartite-graph), choose available proposers in [queue data structure](data-structure.md#fifo-queue) order, initially $A,B,C$, adding rejected proposers at the end. The proposals are $A\to X$, $B\to X$, $C\to Y$, $B\to Y$, $C\to Z$. At the fourth proposal, $Y$ replaces its held $C$ by $B$ because $B\succ_Y C$. This frees $C$ to try $Z$, producing $M_L$.

<a id="image-five-proposals-in-the-gale-shapley-algorithm-y-replaces-a-tentative-partner-before-the-final-stable-matching"></a>
![](stable-matching-deferred-acceptance-trace.png)

**[Figure 2](#image-five-proposals-in-the-gale-shapley-algorithm-y-replaces-a-tentative-partner-before-the-final-stable-matching). Five proposals in the Gale-Shapley algorithm: Y replaces a tentative partner before the final stable matching**.

Reverse the proposing side. Starting in the order $X,Y,Z$, the proposals are $X\to C$, $Y\to A$, $Z\to A$, $Z\to B$. Now $A$ rejects $Z$ because it already holds $Y$. The result is $M_R$. Thus the choice of proposing side can change the output even with [strict preferences](set-theory.md#strict-preference) and complete lists.

Why does the procedure work? Each [edge](graph-theory.md#edge-of-a-graph) receives at most one proposal, so at most $|E|$ proposals occur. At all times, the held [edges](graph-theory.md#edge-of-a-graph) form a [matching in a graph](matching-graph-theory.md), and each receiver holds its favourite proposer among all proposals received. A receiver's held partner can only improve according to its [strict preference](set-theory.md#strict-preference). If a proposer prefers $r$ to its final partner, or ends unmatched while $r$ is acceptable, it must already have proposed to $r$. A rejection means $r$ then held someone better, and its final partner is at least as good. Such an [edge](graph-theory.md#edge-of-a-graph) cannot be a [blocking pair in stable matching](#blocking-pair-in-stable-matching). This covers every possible [blocking pair in stable matching](#blocking-pair-in-stable-matching), proving stability at termination.

With a [queue data structure](data-structure.md#fifo-queue) of unmatched proposers, a next-choice pointer for each list, and constant-time receiver-rank lookups, each proposal takes constant work. Using [Big O notation](real-analysis.md#big-o-notation), the [time complexity](theoretical-computer-science.md#time-complexity) is $O(|E|+|V|)$ including initialization, provided list construction and rank preprocessing also take $O(|E|+|V|)$. Edge-indexed ranks with cross-referenced list entries, or expected constant-time hash lookups, allow sparse storage proportional to $|E|+|V|$. Repeatedly scanning a receiver's preference list to compare offers would lose this bound. For complete lists with $n$ [vertices](graph.md#vertex-graph-theory) per side, $|E|=n^2$ and the bound is $O(n^2)$. Initializing full $n\times n$ rank tables itself costs $\Theta(n^2)$ time and space, even when only a sparse [set](set.md) of pairs is acceptable.

The [Gale-Shapley algorithm](#gale-shapley-algorithm) does more than establish existence: with [strict preferences](set-theory.md#strict-preference), its output is a [proposer-optimal stable matching](#proposer-optimal-stable-matching).[§5, printed p. 14, Theorem 2: applicant optimality and the rejection induction](mathematics-bibliography.md#college-admissions-and-the-stability-of-marriage-by-david-gale-and-lloyd-shapley) It is also a [receiver-pessimal stable matching](#receiver-pessimal-stable-matching), as proved below. Both qualifications compare partners across [stable matchings](#stable-matching-in-a-bipartite-graph).

#### Proposer-optimal stable matching

↑ **Parent:** [Gale-Shapley algorithm](#gale-shapley-algorithm)

For fixed [strict preferences](set-theory.md#strict-preference), a [proposer-optimal stable matching](#proposer-optimal-stable-matching) gives each proposer its best partner obtainable in any [stable matching](#stable-matching-in-a-bipartite-graph), with unmatched ranked last. The [Gale-Shapley algorithm](#gale-shapley-algorithm) achieves all these individual optima simultaneously. In the worked example, $M_L$ gives $A,B,C$ partners ranked $1,2,2$, respectively; the alternative $M_R$ gives them ranks $2,3,3$.

Suppose a first rejection of a pair belonging to some [stable matching](#stable-matching-in-a-bipartite-graph) $S$ occurs when $r$ rejects $\ell$ for $\ell'$. Every partner $\ell'$ prefers to $r$ has already rejected it, so none can be its partner in $S$. If $S(r)=\ell$, then $\ell'$ prefers $r$ to $S(\ell')$, while $r$ prefers $\ell'$ to $\ell$: a [blocking pair in stable matching](#blocking-pair-in-stable-matching), a contradiction. Hence no rejected pair is stable, and each proposer receives its best stable partner. Under [strict preferences](set-theory.md#strict-preference) this also makes the outcome independent of proposal order.

##### Receiver-pessimal stable matching

↑ **Parent:** [Proposer-optimal stable matching](#proposer-optimal-stable-matching)

For fixed [strict preferences](set-theory.md#strict-preference), the same output of the [Gale-Shapley algorithm](#gale-shapley-algorithm) gives each receiver its worst partner obtainable in any [stable matching](#stable-matching-in-a-bipartite-graph), treating unmatched as last. "Worst" is restricted to stable possibilities: a receiver might still receive its favourite acceptable partner if every [stable matching](#stable-matching-in-a-bipartite-graph) assigns it that partner. Reversing the proposing side gives receivers their best stable partners instead.

For a short proof, let $M$ be a [proposer-optimal stable matching](#proposer-optimal-stable-matching) and $S$ any other [stable matching](#stable-matching-in-a-bipartite-graph). If a receiver $r$ preferred $M(r)=\ell$ to $S(r)$, then proposer optimality would make $\ell$ prefer $r=M(\ell)$ to $S(\ell)$, since the partners differ and [preferences](set-theory.md#preference-relation) are strict. The pair $(\ell,r)$ would block $S$. Therefore no receiver prefers its partner in $M$ to its partner in $S$. In the worked example, right-side ranks in $M_L$ are $2,2,3$ for $X,Y,Z$, whereas $M_R$ gives them $1,1,2$. Neither outcome is universally best for both sides.

### Blocking pair in stable matching

↑ **Parent:** [Stable matching in a bipartite graph](#stable-matching-in-a-bipartite-graph)

An acceptable unused [edge](graph-theory.md#edge-of-a-graph) whose endpoints both prefer each other to their partners in a [matching in a graph](matching-graph-theory.md), treating every acceptable partner as preferable to being unmatched. A [stable matching](#stable-matching-in-a-bipartite-graph) has no such [edge](graph-theory.md#edge-of-a-graph). In the worked example, $(B,Y)$ blocks $N$ even though $A$ already has its first choice.

## Near-perfect matching

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)

In a [graph](graph.md) with $2n$ [vertices](graph.md#vertex-graph-theory), a near-perfect [matching in a graph](matching-graph-theory.md) has $n-1$ [edges](graph-theory.md#edge-of-a-graph) and exactly two unmatched [vertices](graph.md#vertex-graph-theory).

## Matching generating function

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)

The coefficient $m_k$ counts [matchings in a graph](matching-graph-theory.md) with $k$ [edges](graph-theory.md#edge-of-a-graph). For a [bipartite graph](bipartite-graph.md) with $n$ [vertices](graph.md#vertex-graph-theory) on each side, $m_n$ counts [perfect matchings](#perfect-matching) and equals the [permanent of a matrix](linear-algebra.md#permanent-mathematics) of its bipartite adjacency [matrix](vector-space.md#matrix). Positive activity $\lambda$ makes $Z_G$ the normalizing constant of the [weighted matching Markov chain](markov-chain.md#weighted-matching-markov-chain).

### Annealing ratios for a matching generating function

↑ **Parent:** [Matching generating function](#matching-generating-function)

For $0<a\leq b$, expand the [expectation](expected-value.md) under the [weighted matching Markov chain](markov-chain.md#weighted-matching-markov-chain) stationary weights to obtain the displayed identity. If the largest [matching in a graph](matching-graph-theory.md) has $n$ [edges](graph-theory.md#edge-of-a-graph) and $b/a\leq1+1/n$, the observable lies in $[1,e]$. Its sample mean has controlled error by the [Hoeffding inequality](probability-inequality.md#hoeffding-inequality). A product of $J$ ratios, each estimated to relative accuracy $O(\varepsilon/J)$, approximates the full ratio to relative accuracy $O(\varepsilon)$.

## Alternating path in a matching

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)

An [alternating path in a matching](#alternating-path-in-a-matching) $M$ is a [graph path](graph-theory.md#path-in-a-graph) whose successive [edges](graph-theory.md#edge-of-a-graph) alternate between membership in $M$ and membership outside $M$. Here [graph paths](graph-theory.md#path-in-a-graph) have no repeated [vertices](graph.md#vertex-graph-theory). Alternation alone does not make a [graph path](graph-theory.md#path-in-a-graph) an [augmenting path in a matching](#augmenting-path-in-a-matching): its endpoints must both be [unmatched vertices in a matching](#unmatched-vertex-in-a-matching). For example, relative to $M=\{(2,3),(4,5)\}$ in the six-[vertex](graph.md#vertex-graph-theory) [path graph](graph-theory.md#path-graph), $2,3,4,5$ alternates but has matched endpoints; toggling just those three [edges](graph-theory.md#edge-of-a-graph) loses one selected [edge](graph-theory.md#edge-of-a-graph).

## Augmenting path in a matching

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)

An [augmenting path in a matching](#augmenting-path-in-a-matching) $M$ is a nonempty [alternating path in a matching](#alternating-path-in-a-matching) with distinct endpoints that are both [unmatched vertices in a matching](#unmatched-vertex-in-a-matching). Its first and last [edges](graph-theory.md#edge-of-a-graph) lie outside $M$. Thus it has $k+1$ unselected [edges](graph-theory.md#edge-of-a-graph) and $k$ selected [edges](graph-theory.md#edge-of-a-graph), for some $k\geq0$. Taking the [symmetric difference](set.md#symmetric-difference)

$$
M'=M\mathbin\triangle E(P)
=(M\setminus E(P))\cup(E(P)\setminus M)
$$

removes the selected [edges](graph-theory.md#edge-of-a-graph) on $P$ and inserts its unselected [edges](graph-theory.md#edge-of-a-graph). Each internal [vertex](graph.md#vertex-graph-theory) exchanges one selected [edge](graph-theory.md#edge-of-a-graph) for another; each endpoint gains its first selected [edge](graph-theory.md#edge-of-a-graph). All choices away from $P$ stay in place, so $M'$ is a [matching in a graph](matching-graph-theory.md) with $|M'|=|M|+1$.[Matching, Covering and Packing, §2.1, printed p. 2: alternating paths, augmenting paths and symmetric difference](mathematics-bibliography.md#graph-theory-by-reinhard-diestel)

For an explicit repair, let the [path graph](graph-theory.md#path-graph) $P_6$ have [vertices](graph.md#vertex-graph-theory) $1,2,3,4,5,6$ in that order and start with

$$
M=\{(2,3),(4,5)\},\qquad P=(1,2,3,4,5,6).
$$

The endpoints $1$ and $6$ are initially [unmatched vertices in a matching](#unmatched-vertex-in-a-matching). Along $P$ the [edges](graph-theory.md#edge-of-a-graph) are outside, inside, outside, inside, outside $M$. Remove $(2,3)$ and $(4,5)$, then add $(1,2),(3,4),(5,6)$ together:

$$
M'=M\mathbin\triangle E(P)=\{(1,2),(3,4),(5,6)\}.
$$

This raises the [cardinality](cardinal-number.md#cardinality) from two to three and gives a [perfect matching](#perfect-matching). Six [vertices](graph.md#vertex-graph-theory) allow at most three disjoint pairs, so it is also a [maximum cardinality matching](#maximum-cardinality-matching). The initial $M$ is already a [maximal matching](#maximal-matching): every unused [edge](graph-theory.md#edge-of-a-graph) touches a matched [vertex](graph.md#vertex-graph-theory). Augmentation succeeds because it can replace earlier choices instead of only adding to them.

<a id="image-the-augmenting-path-in-a-matching-on-p₆-replaces-two-selected-edges-by-three-using-symmetric-difference"></a>
![](matching-augmenting-path-symmetric-difference.png)

**[Figure 3](#image-the-augmenting-path-in-a-matching-on-p₆-replaces-two-selected-edges-by-three-using-symmetric-difference). The augmenting path in a matching on P₆ replaces two selected edges by three using symmetric difference**.

One unused [edge](graph-theory.md#edge-of-a-graph) joining two [unmatched vertices in a matching](#unmatched-vertex-in-a-matching) is the shortest possible [augmenting path in a matching](#augmenting-path-in-a-matching). Longer [augmenting paths in a matching](#augmenting-path-in-a-matching) reassign several partners, explaining why a stalled [greedy matching](#greedy-matching) need not be optimal. For edge benefits $w_e$, the change in total benefit is

$$
\sum_{e\in E(P)\setminus M}w_e-\sum_{e\in E(P)\cap M}w_e,
$$

which need not be positive even though the [cardinality](cardinal-number.md#cardinality) increases. A [maximum-weight matching](#maximum-weight-matching) therefore needs a different optimality test. In an assignment equality graph an [augmenting path in a matching](#augmenting-path-in-a-matching) moves toward a [perfect matching](#perfect-matching) while preserving zero [reduced costs](linear-programming.md#reduced-cost) on matched [edges](graph-theory.md#edge-of-a-graph); this is the setting used by the [Hungarian algorithm](linear-programming.md#hungarian-algorithm).

<h3 id="berge-s-theorem">Berge's theorem</h3>

↑ **Parent:** [Augmenting path in a matching](#augmenting-path-in-a-matching)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Berge's_theorem)

For a finite [simple graph](graph.md#simple-graph) $G$ and a [matching in a graph](matching-graph-theory.md) $M\subseteq E(G)$, $M$ is a [maximum cardinality matching](#maximum-cardinality-matching) if and only if $G$ has no [augmenting path in a matching](#augmenting-path-in-a-matching) relative to $M$. The [graph](graph.md) need not be a [bipartite graph](bipartite-graph.md), and the assertion concerns [cardinality](cardinal-number.md#cardinality), not edge benefits.[Claude Berge, Two theorems in graph theory, printed p. 842: finite unoriented graph and Problem 3; printed p. 843, Theorem 1: maximum matching and absence of an alternating chain between neutral points](mathematics-bibliography.md#two-theorems-in-graph-theory-by-claude-berge)

The criterion turns a global comparison with every competing [matching in a graph](matching-graph-theory.md) into a search for one repair. Starting from any [matching in a graph](matching-graph-theory.md), repeatedly find and toggle an [augmenting path in a matching](#augmenting-path-in-a-matching). Each step adds one selected [edge](graph-theory.md#edge-of-a-graph), so finiteness gives termination after at most $\lfloor |V(G)|/2\rfloor-|M|$ steps; absence of any further [augmenting path in a matching](#augmenting-path-in-a-matching) certifies maximum [cardinality](cardinal-number.md#cardinality). This is an optimality criterion, not by itself a bound on the work needed to find each [graph path](graph-theory.md#path-in-a-graph).

For a short proof outline, an [augmenting path in a matching](#augmenting-path-in-a-matching) immediately contradicts maximum [cardinality](cardinal-number.md#cardinality). Conversely, if another [matching in a graph](matching-graph-theory.md) $N$ has $|N|>|M|$, consider the [subgraph](graph-theory.md#subgraph) whose [set](set.md) of [edges](graph-theory.md#edge-of-a-graph) is $M\mathbin\triangle N$. Its [vertices](graph.md#vertex-graph-theory) have [degree of a vertex](graph-theory.md#degree-graph-theory) at most two; its nontrivial [connected components](geometry-and-topology.md#connected-component) are [graph paths](graph-theory.md#path-in-a-graph) and even [cycles in a graph](graph-theory.md#cycle-in-a-graph), alternating between the two [matchings in a graph](matching-graph-theory.md). A [cycle in a graph](graph-theory.md#cycle-in-a-graph) contributes equal numbers from each. Hence some [graph path](graph-theory.md#path-in-a-graph) contributes one more [edge](graph-theory.md#edge-of-a-graph) from $N$ than from $M$ and starts and ends with [edges](graph-theory.md#edge-of-a-graph) from $N$. Its endpoints are [unmatched vertices in a matching](#unmatched-vertex-in-a-matching) relative to $M$, yielding the required [augmenting path in a matching](#augmenting-path-in-a-matching).

### Short augmenting paths in a dense bipartite graph

↑ **Parent:** [Augmenting path in a matching](#augmenting-path-in-a-matching)

The two sides have $n$ [vertices](graph.md#vertex-graph-theory) each. Given a nonperfect [matching in a graph](matching-graph-theory.md), choose unmatched [vertices](graph.md#vertex-graph-theory) $u,v$ on opposite sides. An unmatched [neighbour](graph-theory.md#neighbour-of-a-vertex) of either supplies a one-edge [augmenting path in a matching](#augmenting-path-in-a-matching). Otherwise their [neighbours](graph-theory.md#neighbour-of-a-vertex) are matched; the matched left [vertices](graph.md#vertex-graph-theory) corresponding to $N(u)$ and the set $N(v)$ have total size greater than $n$, so they intersect. This supplies the alternating [path in a graph](graph-theory.md#path-in-a-graph) $u,b,a,v$ with $ab$ in the [matching in a graph](matching-graph-theory.md). Repeated augmentation produces a [perfect matching](#perfect-matching).

Choose such an augmentation deterministically. Its reverse is specified by at most four [vertices](graph.md#vertex-graph-theory), giving at most $2n^4$ preimages for a [matching in a graph](matching-graph-theory.md) of the next size. Thus the [matching generating function](#matching-generating-function) coefficients satisfy $m_k\leq2n^4m_{k+1}$.

## Perfect matching

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perfect_matching)

A [perfect matching](#perfect-matching) is a [matching in a graph](matching-graph-theory.md) that covers every [vertex](graph.md#vertex-graph-theory) exactly once. Its [edges](graph-theory.md#edge-of-a-graph) have no shared endpoints, and every [vertex](graph.md#vertex-graph-theory) is an endpoint of one selected [edge](graph-theory.md#edge-of-a-graph). It is useful when a collection must be divided into disjoint pairs with no element left over.

In a [bipartite graph](bipartite-graph.md) with equally many [vertices](graph.md#vertex-graph-theory) on its two sides, a [perfect matching](#perfect-matching) can assign every person one allowed job and every job one person. The example under [permanent of a matrix](linear-algebra.md#permanent-mathematics) has three people and three jobs, with exactly three valid assignments. The blue [edges](graph-theory.md#edge-of-a-graph) below show those three [perfect matchings](#perfect-matching); a crossing in the drawing is not an extra [vertex](graph.md#vertex-graph-theory).

<a id="image-three-perfect-matchings-pair-every-person-vertex-with-one-job-vertex-along-allowed-edges"></a>
![](permanent-perfect-matching-assignments.png)

**[Figure 4](#image-three-perfect-matchings-pair-every-person-vertex-with-one-job-vertex-along-allowed-edges). Three perfect matchings pair every person vertex with one job vertex along allowed edges**.

Every selected [edge](graph-theory.md#edge-of-a-graph) covers two [vertices](graph.md#vertex-graph-theory), so a [graph](graph.md) with an [odd integer](integer.md#odd-integer) number of [vertices](graph.md#vertex-graph-theory) has no [perfect matching](#perfect-matching). An [even integer](integer.md#even-number) number is necessary but does not guarantee existence: an [isolated vertex](random-graph.md#isolated-vertex) cannot be covered. A [perfect matching](#perfect-matching) also need not be unique. For example, the [complete bipartite graph](bipartite-graph.md#complete-bipartite-graph) $K_{2,2}$ has two [perfect matchings](#perfect-matching), corresponding to the two ways of assigning two people to two jobs.

Counting all [perfect matchings](#perfect-matching) is a different question from finding one. For a zero-one [biadjacency matrix](bipartite-graph.md#biadjacency-matrix) of a balanced [bipartite graph](bipartite-graph.md), the count is its [permanent of a matrix](linear-algebra.md#permanent-mathematics). The [nonzero determinant criterion for a perfect matching](graph-theory.md#perfect-matching-from-a-nonzero-determinant) supplies an existence test, but cancellation means that a zero [determinant](multilinear-algebra.md#determinant) does not rule one out.

### Flexible vertex in a balanced bipartite graph

↑ **Parent:** [Perfect matching](#perfect-matching)

A vertex on one side of a balanced [bipartite graph](bipartite-graph.md) is flexible if every incident edge lies in a [perfect matching](#perfect-matching). The strict [Hall marriage theorem](#hall-s-marriage-theorem) inequalities for nonempty proper subsets imply flexibility of every vertex: after forcing an edge, removal of its ends loses at most one neighbour from each remaining set. If a perfect matching exists without the strict condition, choose a minimal nonempty tight set. Its induced balanced graph has the strict condition internally, and each internal matching extends using the original matching outside that set. Thus at least one flexible vertex always exists.

### Minimum-weight perfect matching

↑ **Parent:** [Perfect matching](#perfect-matching)

A minimum-weight [perfect matching](#perfect-matching) pairs every vertex exactly once while minimizing total edge weight. General weighted [perfect matching](#perfect-matching) has polynomial-time algorithms. In the [Christofides algorithm](mathematical-optimization.md#christofides-algorithm), it corrects precisely the odd-degree vertices of a [minimum spanning tree](tree-graph-theory.md#minimum-spanning-tree). Alternating edges of a cyclic order on an even number of vertices give two [perfect matchings](#perfect-matching); the cheaper one costs at most half that cycle's cost.

### One-factorization

↑ **Parent:** [Perfect matching](#perfect-matching)

A one-factorization partitions every edge of a graph into [perfect matchings](#perfect-matching). Each matching uses every vertex exactly once. A [total of synthemes](combinatorics.md#total-of-synthemes) is precisely a one-factorization of the complete graph on six points.

## Maximal matching

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)

A [maximal matching](#maximal-matching) is a [matching in a graph](matching-graph-theory.md) to which no extra [edge](graph-theory.md#edge-of-a-graph) can be added while retaining all current selected [edges](graph-theory.md#edge-of-a-graph). Equivalently, no [edge](graph-theory.md#edge-of-a-graph) joins two [unmatched vertices in a matching](#unmatched-vertex-in-a-matching); those [vertices](graph.md#vertex-graph-theory) form an [independent set](graph-theory.md#independent-set-graph-theory). Every [maximum cardinality matching](#maximum-cardinality-matching) is a [maximal matching](#maximal-matching), but the converse fails.

Take the [path graph](graph-theory.md#path-graph) $P_4$ with [vertices](graph.md#vertex-graph-theory) $1,2,3,4$ and [edges](graph-theory.md#edge-of-a-graph) $(1,2),(2,3),(3,4)$. A [greedy algorithm](algorithm.md#greedy-algorithm) that first selects the middle [edge](graph-theory.md#edge-of-a-graph) produces $M=\{(2,3)\}$. Both remaining [edges](graph-theory.md#edge-of-a-graph) touch a matched [vertex](graph.md#vertex-graph-theory), so this size-one [matching in a graph](matching-graph-theory.md) is maximal. Yet $N=\{(1,2),(3,4)\}$ has two [edges](graph-theory.md#edge-of-a-graph). No [matching in a graph](matching-graph-theory.md) on four [vertices](graph.md#vertex-graph-theory) has more than two [edges](graph-theory.md#edge-of-a-graph), so $N$ is a [maximum cardinality matching](#maximum-cardinality-matching). The two remaining free [vertices](graph.md#vertex-graph-theory) of $M$, namely $1$ and $4$, are not adjacent; that does not prevent a longer [augmenting path in a matching](#augmenting-path-in-a-matching) from joining them.

<a id="image-choosing-the-middle-edge-of-p₄-gives-a-maximal-matching-of-size-one-the-outer-edges-give-a-maximum-cardinality-matching-of-size-two"></a>
![](matching-greedy-middle-edge-trap.png)

**[Figure 5](#image-choosing-the-middle-edge-of-p₄-gives-a-maximal-matching-of-size-one-the-outer-edges-give-a-maximum-cardinality-matching-of-size-two). Choosing the middle edge of P₄ gives a maximal matching of size one; the outer edges give a maximum cardinality matching of size two**.

Maximality is useful as a quick stopping rule and a modest guarantee. For any [maximal matching](#maximal-matching) $M$ and [maximum cardinality matching](#maximum-cardinality-matching) $N$ in a finite [simple graph](graph.md#simple-graph), every [edge](graph-theory.md#edge-of-a-graph) of $N$ touches an endpoint of an [edge](graph-theory.md#edge-of-a-graph) of $M$. Assign it to one such [edge](graph-theory.md#edge-of-a-graph) of $M$. Since $N$ has disjoint endpoints, each [edge](graph-theory.md#edge-of-a-graph) of $M$ receives at most two assignments, proving $|N|\leq2|M|$. The P₄ example reaches equality. Thus maximality guarantees at least half the largest [cardinality](cardinal-number.md#cardinality), but says nothing comparable about arbitrary edge benefits. Its selected endpoints also form a [vertex cover](graph-theory.md#vertex-cover), as explained under [vertex cover](graph-theory.md#vertex-cover).

### Greedy matching

↑ **Parent:** [Maximal matching](#maximal-matching)

A [greedy matching](#greedy-matching) starts with the empty [matching in a graph](matching-graph-theory.md), scans all [edges](graph-theory.md#edge-of-a-graph) in some order, and selects an [edge](graph-theory.md#edge-of-a-graph) exactly when both endpoints are [unmatched vertices in a matching](#unmatched-vertex-in-a-matching). For a finite [graph](graph.md), a complete scan returns a [maximal matching](#maximal-matching): a rejected [edge](graph-theory.md#edge-of-a-graph) had a matched endpoint, which stays matched thereafter. Stopping before all [edges](graph-theory.md#edge-of-a-graph) have been considered need not give maximality. Changing the order can change the result; on P₄, middle-first gives one pair, whereas outer-first gives two. A [greedy algorithm](algorithm.md#greedy-algorithm) of this form never revisits its choices, while an [augmenting path in a matching](#augmenting-path-in-a-matching) does.

## Matching number

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)

For a finite [graph](graph.md) $G$, the [matching number](#matching-number) is

$$
\nu(G)=\max\{|M|:M\text{ is a matching of }G\}.
$$

It is the [cardinality](cardinal-number.md#cardinality) of a [maximum cardinality matching](#maximum-cardinality-matching). The vertex capacity constraint gives $0\leq\nu(G)\leq\lfloor |V(G)|/2\rfloor$. The worked [path graph](graph-theory.md#path-graph) examples have $\nu(P_4)=2$ and $\nu(P_6)=3$. A [perfect matching](#perfect-matching) reaches $|V(G)|/2$; the empty [graph](graph.md) has [matching number](#matching-number) zero.

## Maximum cardinality matching

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximum_cardinality_matching)

A [maximum cardinality matching](#maximum-cardinality-matching) is a [matching in a graph](matching-graph-theory.md) with as many [edges](graph-theory.md#edge-of-a-graph) as any [matching in a graph](matching-graph-theory.md) of the same [graph](graph.md). It has [cardinality](cardinal-number.md#cardinality) $\nu(G)$, the [matching number](#matching-number), and need not be unique or be a [perfect matching](#perfect-matching). For example, any single [edge](graph-theory.md#edge-of-a-graph) of a [triangle in a graph](graph.md#triangle-in-a-graph) is a [maximum cardinality matching](#maximum-cardinality-matching), but leaves one [vertex](graph.md#vertex-graph-theory) unmatched. [Berge's theorem](#berge-s-theorem) characterizes these optima by the absence of an [augmenting path in a matching](#augmenting-path-in-a-matching).

## Maximum-weight matching

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)

Assign each [edge](graph-theory.md#edge-of-a-graph) $e$ a real benefit $w_e$. A [maximum-weight matching](#maximum-weight-matching) maximizes $\sum_{e\in M}w_e$ over all [matchings in a graph](matching-graph-theory.md) $M$; the empty [matching in a graph](matching-graph-theory.md) is allowed. Setting every $w_e=1$ recovers a [maximum cardinality matching](#maximum-cardinality-matching), but otherwise the objectives can disagree.

On the same [path graph](graph-theory.md#path-graph) $P_4$, give the middle [edge](graph-theory.md#edge-of-a-graph) benefit $3$ and each outer [edge](graph-theory.md#edge-of-a-graph) benefit $1$. The [matching in a graph](matching-graph-theory.md) $\{(2,3)\}$ has total benefit $3$, while the two-[edge](graph-theory.md#edge-of-a-graph) [matching in a graph](matching-graph-theory.md) $\{(1,2),(3,4)\}$ has total benefit $2$. Thus the smaller choice is the unique [maximum-weight matching](#maximum-weight-matching). If instead the requirement is to find a [maximum cardinality matching](#maximum-cardinality-matching) and then maximize benefit among those, the outer [edges](graph-theory.md#edge-of-a-graph) must be chosen. Requiring a [perfect matching](#perfect-matching) before optimizing cost is another distinct problem, covered by [minimum-weight perfect matching](#minimum-weight-perfect-matching). With negative benefits a [maximum-weight matching](#maximum-weight-matching) can even be empty, so it need not be a [maximal matching](#maximal-matching).

<h2 id="hall-s-marriage-theorem">Hall's marriage theorem</h2>

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hall's_marriage_theorem)

For a finite [bipartite graph](bipartite-graph.md) $G=(L\cup R,E)$ with disjoint left and right [vertex sets](graph.md#vertex-set), [Hall's marriage theorem](#hall-s-marriage-theorem) characterizes when distinct allowed partners can be chosen for every left [vertex](graph.md#vertex-graph-theory). A [matching in a graph](matching-graph-theory.md) with [matching saturation](#matching-saturation) of $L$ exists **if and only if** every [subset](set.md#subset) $S\subseteq L$ satisfies

$$
|N_G(S)|\geq |S|,\qquad N_G(S)=\{r\in R:\text{some }s\in S\text{ has }sr\in E\}.
$$

The [graph neighbourhood](graph-theory.md#graph-neighbourhood) counts distinct right [vertices](graph.md#vertex-graph-theory), rather than [edges](graph-theory.md#edge-of-a-graph) or repeated choices. This is the [Hall condition](#hall-condition). Its failure supplies a concrete [Hall obstruction](#hall-obstruction). Necessity follows because the chosen partners of $S$ are distinct members of $N_G(S)$; sufficiency is the surprising assertion that these collective counts rule out every obstacle.[Matching, Covering and Packing, 4th electronic edition 2010, corrected reprint 2012, §2.1, printed pp. 3–4, Theorem 2.1.2: matching of the specified part](mathematics-bibliography.md#graph-theory-by-reinhard-diestel)

The right side may be larger: [matching saturation](#matching-saturation) of $L$ leaves $|R|-|L|$ right [vertices](graph.md#vertex-graph-theory) unmatched. Only when $|L|=|R|$ does a [matching in a graph](matching-graph-theory.md) saturating $L$ automatically become a [perfect matching](#perfect-matching). For a specified [subset](set.md#subset) $X\subseteq L$, apply the same criterion only to $S\subseteq X$, using the [induced subgraph](graph-theory.md#induced-subgraph) on $X\cup R$. The remaining left [vertices](graph.md#vertex-graph-theory) need not be matched. The empty [set](set.md) gives $0\geq0$; if $X$ is empty, the empty [matching in a graph](matching-graph-theory.md) suffices.

Consider a [scheduling](mathematical-optimization.md#scheduling) model with three unit-duration jobs $a,b,c$ and four available slots $1,2,3,4$ on one machine. Each job needs exactly one slot, each slot accepts at most one job, and the allowed slots are

$$
N(a)=\{1,2\},\qquad N(b)=\{1\},\qquad N(c)=\{2,3,4\}.
$$

The [bipartite graph](bipartite-graph.md) below admits $M=\{a2,b1,c3\}$, a [matching in a graph](matching-graph-theory.md) saturating all jobs while leaving slot $4$ unused. It is not a [perfect matching](#perfect-matching) of the seven-[vertex](graph.md#vertex-graph-theory) [graph](graph.md). A greedy choice $a1$ initially blocks $b$, but the [augmenting path in a matching](#augmenting-path-in-a-matching) $b,1,a,2$ replaces $a1$ by $b1,a2$; subsequent assignment of $c3$ succeeds. A bad partial choice is not an impossibility certificate.

<a id="image-a-matching-in-a-graph-saturates-all-three-jobs-and-leaves-one-of-four-slots-unused"></a>
![](hall-matching-three-jobs-four-slots.png)

**[Figure 6](#image-a-matching-in-a-graph-saturates-all-three-jobs-and-leaves-one-of-four-slots-unused). A matching in a graph saturates all three jobs and leaves one of four slots unused**. Thick blue [edges](graph-theory.md#edge-of-a-graph) are $a2,b1,c3$; thin grey [edges](graph-theory.md#edge-of-a-graph) are other allowed assignments. Crossings are not [vertices](graph.md#vertex-graph-theory).

There are eight [subsets](set.md#subset) of $L=\{a,b,c\}$. Listing each [graph neighbourhood](graph-theory.md#graph-neighbourhood) makes the all-[subset](set.md#subset) requirement explicit:

| $S$ | $N(S)$ | $|S|$ | $|N(S)|$ |
| --- | --- | --- | --- |
| $\varnothing$ | $\varnothing$ | 0 | 0 |
| $\{a\}$ | $\{1,2\}$ | 1 | 2 |
| $\{b\}$ | $\{1\}$ | 1 | 1 |
| $\{c\}$ | $\{2,3,4\}$ | 1 | 3 |
| $\{a,b\}$ | $\{1,2\}$ | 2 | 2 |
| $\{a,c\}$ | $\{1,2,3,4\}$ | 2 | 4 |
| $\{b,c\}$ | $\{1,2,3,4\}$ | 2 | 4 |
| $\{a,b,c\}$ | $\{1,2,3,4\}$ | 3 | 4 |

There are exactly two [matchings in a graph](matching-graph-theory.md) saturating $L$: $\{a2,b1,c3\}$ and $\{a2,b1,c4\}$. Job $b$ forces slot $1$, then job $a$ forces slot $2$, leaving two choices for $c$.

### Hall condition

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

The [Hall condition](#hall-condition) requires enough distinct [neighbours](graph-theory.md#neighbour-of-a-vertex) for **every** [subset](set.md#subset) of the specified left [vertex set](graph.md#vertex-set) in a finite [bipartite graph](bipartite-graph.md). Checking the whole left [set](set.md) establishes only one inequality. Checking singleton [sets](set.md) establishes only that each left [vertex](graph.md#vertex-graph-theory) has positive [degree of a vertex](graph-theory.md#degree-graph-theory). Overlapping lists can pass both tests and still fail to admit [matching saturation](#matching-saturation) of the left side.

#### Hall obstruction

↑ **Parent:** [Hall condition](#hall-condition)

A [Hall obstruction](#hall-obstruction) is a left [subset](set.md#subset) $S$ with fewer distinct [neighbours](graph-theory.md#neighbour-of-a-vertex) than [vertices](graph.md#vertex-graph-theory). At most $|N(S)|$ members of $S$ can be matched, so at least $|S|-|N(S)|$ must remain unmatched. The [pigeonhole principle](combinatorics.md#pigeonhole-principle) proves failure without enumerating every proposed assignment.

For a stronger counterexample than an [isolated vertex](random-graph.md#isolated-vertex), take $L=\{a,b,c,d\}$ and $R=\{1,2,3,4\}$ with

$$
N(a)=N(b)=N(c)=\{1,2\},\qquad N(d)=\{3,4\}.
$$

Every [vertex](graph.md#vertex-graph-theory) has positive [degree of a vertex](graph-theory.md#degree-graph-theory), the sides have equal [cardinality](cardinal-number.md#cardinality), and $|N(L)|=|L|=4$. Every two-[vertex](graph.md#vertex-graph-theory) left [subset](set.md#subset) also passes the [Hall condition](#hall-condition). Nevertheless $S=\{a,b,c\}$ has only $N(S)=\{1,2\}$, so $2<3$ rules out [matching saturation](#matching-saturation) of $L$.

<a id="image-a-three-vertex-hall-obstruction-has-only-two-neighbours-despite-enough-slots-in-total"></a>
![](hall-obstruction-three-jobs-two-slots.png)

**[Figure 7](#image-a-three-vertex-hall-obstruction-has-only-two-neighbours-despite-enough-slots-in-total). A three-vertex Hall obstruction has only two neighbours, despite enough slots in total**. Red boundaries identify $S=\{a,b,c\}$ and $N(S)=\{1,2\}$. Thick blue [edges](graph-theory.md#edge-of-a-graph) give the maximum-size [matching in a graph](matching-graph-theory.md) $\{a1,b2,d3\}$; $c$ and slot $4$ are unmatched.

All sixteen left [subsets](set.md#subset) can be checked by writing $k=|S\cap\{a,b,c\}|$ and $\varepsilon=1$ if $d\in S$, otherwise $0$. Then

$$
|S|=k+\varepsilon,\qquad |N(S)|=2\mathbf1_{\{k>0\}}+2\varepsilon.
$$

Only $k=3,\varepsilon=0$ violates the [Hall condition](#hall-condition). Every [matching in a graph](matching-graph-theory.md) uses at most two [edges](graph-theory.md#edge-of-a-graph) incident to $\{a,b,c\}$ and at most one incident to $d$, so the [matching number](#matching-number) is three. There are exactly twelve size-three [matchings in a graph](matching-graph-theory.md): choose two of $a,b,c$ in three ways, assign them to $1,2$ in two ways, and choose $3$ or $4$ for $d$. Thus the obstruction identifies the bottleneck: adding availability only for $d$ cannot help; allowing $c$ to use slot $3$ permits $\{a1,b2,c3,d4\}$, a [perfect matching](#perfect-matching).

### Hall allocation model

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

In a unit-capacity [assignment problem](linear-programming.md#assignment-problem), left [vertices](graph.md#vertex-graph-theory) represent demands and right [vertices](graph.md#vertex-graph-theory) represent individually usable resources; an [edge](graph-theory.md#edge-of-a-graph) records compatibility. All constraints must be encoded by those allowed pairs and by using each resource at most once. [Hall's marriage theorem](#hall-s-marriage-theorem) decides feasibility. Costs belong to an additional [mathematical optimization](mathematical-optimization.md) problem; precedence between jobs or requirements for consecutive slots need additional modelling.

The authored [Notes on the design of a conference scheduler by David R. MacIver](mathematics-bibliography.md#notes-on-the-design-of-a-conference-scheduler-by-david-r-maciver) (Implementation, 7 August 2022) illustrates a [Hall obstruction](#hall-obstruction) with four talks confined to three slots. With one talk per slot, that [subset](set.md#subset) has size four and a [graph neighbourhood](graph-theory.md#graph-neighbourhood) of size three. An unused slot outside its [graph neighbourhood](graph-theory.md#graph-neighbourhood) does not remove the bottleneck. In the three-job example above, the same [scheduling](mathematical-optimization.md#scheduling) model instead has two complete assignments.

The allocation exercise in [Graph Theory by Reinhard Diestel](mathematics-bibliography.md#graph-theory-by-reinhard-diestel) (Matching, Covering and Packing, printed p. 20, Exercise 9) asks for disjoint [subsets](set.md#subset) $D_i\subseteq A_i$ of prescribed nonnegative [integer](integer.md) sizes $d_i$. Replace demand $i$ by $d_i$ left [vertices](graph.md#vertex-graph-theory) with allowed resource [set](set.md) $A_i$. [Hall's marriage theorem](#hall-s-marriage-theorem) gives exactly the condition

$$
\left|\bigcup_{i\in I}A_i\right|\geq\sum_{i\in I}d_i\qquad\text{for every index subset }I.
$$

For a numerical instance, let $A_1=\{1,2\}$, $A_2=\{2,3\}$, and $d_1=2,d_2=1$. The separate demands and their combined demand fit, and $D_1=\{1,2\},D_2=\{3\}$ works. Raising $d_2$ to two leaves both individual tests valid but demands four distinct resources from a [set union](set.md#set-union) of size three. This is the same collective obstruction with repeated demand [vertices](graph.md#vertex-graph-theory).

### System of distinct representatives

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

A [system of distinct representatives](#system-of-distinct-representatives) for a finite indexed family of finite [sets](set.md) $(A_i)_{i\in I}$ chooses one element $x_i\in A_i$ per index, with all choices distinct. Form a [bipartite graph](bipartite-graph.md) with left [vertex set](graph.md#vertex-set) $I$, right [vertex set](graph.md#vertex-set) $\bigcup_{i\in I}A_i$, and [edges](graph-theory.md#edge-of-a-graph) $ix$ whenever $x\in A_i$. [Matching saturation](#matching-saturation) of $I$ is precisely a [system of distinct representatives](#system-of-distinct-representatives). Hence [Hall's marriage theorem](#hall-s-marriage-theorem) says that such choices exist exactly when $|\bigcup_{i\in J}A_i|\geq|J|$ for every [subset](set.md#subset) $J\subseteq I$. Repeated equal [sets](set.md) still have separate indices and separate demands.

### Hall theorem proof outline

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

For sufficiency, take a [matching in a graph](matching-graph-theory.md) of maximum size and suppose a left [vertex](graph.md#vertex-graph-theory) $u$ is unmatched. Follow unused [edges](graph-theory.md#edge-of-a-graph) from left to right and matching [edges](graph-theory.md#edge-of-a-graph) back to the left. An unmatched reachable right [vertex](graph.md#vertex-graph-theory) yields an [augmenting path in a matching](#augmenting-path-in-a-matching), contradicting maximal size. Otherwise let $S,T$ be the reachable left and right [sets](set.md). Every member of $T$ is matched to a distinct member of $S\setminus\{u\}$, and every member of $S\setminus\{u\}$ is reached this way. Since $N(S)=T$, we obtain $|N(S)|=|S|-1$, contradicting the [Hall condition](#hall-condition). Finiteness ensures that a maximum-size [matching in a graph](matching-graph-theory.md) exists.

The alternative [Hall induction through a tight set](#hall-induction-through-a-tight-set) uses [mathematical induction](foundations-of-mathematics.md#mathematical-induction): a proper nonempty [subset](set.md#subset) with $|N(S)|=|S|$ splits off a balanced [induced subgraph](graph-theory.md#induced-subgraph); without such a tight [set](set.md), deleting one chosen [edge](graph-theory.md#edge-of-a-graph)'s endpoints preserves the [Hall condition](#hall-condition) on the smaller left side.

### Random bipartite matching from empty-rectangle exclusion

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

In the equal-part random [bipartite graph](bipartite-graph.md) with fixed edge probability $0<p<1$, rule out empty rectangles of side $\lceil\sqrt n\rceil$ and vertices with at least $n-\lceil\sqrt n\rceil$ nonneighbors. A union bound gives the displayed asymptotic estimate. Small vertex sets satisfy Hall's condition by the degree bound; intermediate sets do so because their omitted-neighbor rectangle would contain a forbidden square; large sets meet every vertex in the other part. Thus [Hall's marriage theorem](#hall-s-marriage-theorem) gives a perfect matching asymptotically almost surely. This does not mean probability one at any finite size.

### Hall matching of maximal separated sets

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

Two maximum-[cardinality](cardinal-number.md#cardinality) $\varepsilon$-separated subsets $A,B$ of a [compact metric space](topological-analysis.md#compact-metric-space) have a bijection that moves each point by less than $\varepsilon$. Join $a$ to $b$ when their distance is below $\varepsilon$. If $S\subseteq A$ had fewer than $|S|$ neighbours, replacing these neighbours in $B$ by $S$ would create a larger separated set. The [Hall marriage theorem](#hall-s-marriage-theorem) therefore supplies a [perfect matching](#perfect-matching). This allows empirical averages on a compact [isometry group](riemannian-geometry.md#isometry-group) to be made approximately invariant without assuming a prior [Haar measure](measure.md#haar-measure) construction.

### Degree-weighted Hall condition

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

In a finite bipartite graph, suppose every left vertex has positive degree and each edge joins vertices with $d(x)\geq d(y)$ from left to right. Then $|N(A)|\geq\sum_{x\in A}\sum_{y\sim x}1/d(y)\geq|A|$, so a matching covers the left side.

### Measurable Hall theorem

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

For finitely many [Lebesgue measurable sets](measure-theory.md#lebesgue-measurable-set) $A_i\subseteq[0,1]$ and nonnegative demands $b_i$, pairwise disjoint measurable [subsets](set.md#subset) $B_i\subseteq A_i$ with $\lambda(B_i)=b_i$ exist exactly when $\lambda(\bigcup_{i\in I}A_i)\geq\sum_{i\in I}b_i$ for every index [subset](set.md#subset) $I$. Necessity is additivity and monotonicity of [Lebesgue measure](measure-theory.md#lebesgue-measure). For sufficiency, partition the [set union](set.md#set-union) into membership cells $E_J$, send flow from a source through demand vertices $i$ to cells with $i\in J$, then to a sink. Source capacities are $b_i$, cell capacities are $\lambda(E_J)$, and intermediate capacities are $D=\sum_i b_i$. Every [cut of a flow network](flow-network.md#cut-of-a-flow-network) has capacity at least $D$ by the assumed inequalities. The [max-flow min-cut theorem](flow-network.md#max-flow-min-cut-theorem) provides the allocations, and [divisibility of Lebesgue measure](measure-theory.md#divisibility-of-lebesgue-measure) turns each cell allocation into disjoint pieces. If $D=0$, all $B_i$ can simply be empty.

### Hall induction through a tight set

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

For Hall's theorem, either every proper nonempty set has one excess neighbour and one deletes an arbitrary edge's endpoints, or a tight set $S$ with $|N(S)|=|S|$ splits the problem into the induced graph on $S\cup N(S)$ and its complement.

### Regular bipartite graph has a perfect matching

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

In a $k$-regular bipartite graph, edge counting gives equal vertex-class sizes and $k|S|\leq k|N(S)|$. Hall's theorem therefore supplies a perfect matching.

## Regular-graph matching bound from unmatched vertices

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)

If a $k$-regular graph on $n$ vertices has a maximum matching of size $m$, its unmatched vertices are independent. Counting their incident edges gives $k(n-2m)\leq2(k-1)m$, and hence $m\geq kn/(4k-2)$.

### Disjoint union of triangles as a sharp matching example

↑ **Parent:** [Regular-graph matching bound from unmatched vertices](#regular-graph-matching-bound-from-unmatched-vertices)

The disjoint union of $r$ triangles is $2$-regular on $3r$ vertices and has matching number $r$, attaining the regular-graph lower bound $n/3$.

## ↑ Ancestors (5)

1. [Graph theory](graph-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)
