# Paper 214

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_214.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_214.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 214](paper-214.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For [bond percolation](../../../bond-percolation.md), the [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) states that any two [increasing events](../../../probability-inequality.md#increasing-event) $A,B$ satisfy

$$
\mathbb P_p(A\cap B)\geq\mathbb P_p(A)\mathbb P_p(B).
$$

The same inequality holds for two [decreasing events](../../../probability-inequality.md#decreasing-event), either by reversing the coordinate order or by taking complements in the two-event identity. Intersections of [decreasing events](../../../probability-inequality.md#decreasing-event) are [decreasing events](../../../probability-inequality.md#decreasing-event), so induction gives

$$
\mathbb P_p\left(\bigcap_{j=1}^n A_j^c\right)\geq\prod_{j=1}^n\mathbb P_p(A_j^c).
$$

Write $a=\mathbb P_p(A_1)=\cdots=\mathbb P_p(A_n)$ and $u=\mathbb P_p(\bigcup_jA_j)$. Then $1-u\geq(1-a)^n$. Taking the nonnegative $n$-th root and rearranging yields the [square-root trick for positively associated events](../../../probability-inequality.md#square-root-trick-for-positively-associated-events):

$$
\boxed{\mathbb P_p(A_1)\geq1-\left(1-\mathbb P_p\left(\bigcup_{j=1}^n A_j\right)\right)^{1/n}.}
$$

No independence among the events is needed.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Put $I=\{x:|C(x)|=\infty\}$, the union of all infinite [percolation clusters](../../../bond-percolation.md#percolation-cluster). Since $p>p_c$, the [percolation probability](../../../probability-theory.md#percolation-probability) $\theta(p)$ is positive. The [translation ergodicity of Bernoulli percolation](../../../bond-percolation.md#translation-ergodicity-of-bernoulli-percolation) makes $\{I\ne\varnothing\}$ a zero-one event; it has positive probability because $\mathbb P_p(0\in I)=\theta(p)>0$, hence it occurs [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).

Let $D_m=\{B(m)\cap I\ne\varnothing\}$. These events increase to $\{I\ne\varnothing\}$, so [continuity from below of a measure](../../../measure-theory.md#continuity-from-below-of-a-measure) gives $\mathbb P_p(D_m)\to1$. On $D_m$, some vertex of $B(m)$ has an infinite open [path in a graph](../../../graph-theory.md#path-in-a-graph). For every $N\geq m$, the segment up to its first visit to $\partial B(N)$ lies entirely in $B(N)$. Thus even with this restriction on the connecting [path in a graph](../../../graph-theory.md#path-in-a-graph),

$$
\boxed{\inf_{n\geq1}\mathbb P_p\bigl(B(m)\longleftrightarrow\partial B(m+n)\text{ within }B(m+n)\bigr)\geq\mathbb P_p(D_m)\longrightarrow1.}
$$

This proves the requested uniformity and supplies the version needed for crossings later.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

For each of the $2d$ coordinate faces $F$ of $B(N)$, define the [increasing event](../../../probability-inequality.md#increasing-event) $A_F(m,N)$ that an open [path in a graph](../../../graph-theory.md#path-in-a-graph) lying in $B(N)$ joins $B(m)$ to $F$. Their union is exactly the event of connection from $B(m)$ to $\partial B(N)$ within $B(N)$. The [bond percolation](../../../bond-percolation.md) law and the centered boxes are invariant under coordinate permutations and sign changes, so all $2d$ events have the same probability.

Apply the [square-root trick for positively associated events](../../../probability-inequality.md#square-root-trick-for-positively-associated-events) from part (a), with $2d$ in place of the number of events. If $\delta_m=1-\mathbb P_p(D_m)$, part (b.i) gives, for every $N=m+n$,

$$
\boxed{\mathbb P_p(A_F(m,N))\geq1-\delta_m^{1/(2d)}\longrightarrow1,\qquad\text{uniformly in }n\geq1.}
$$

In particular this holds for the left and right faces, and it proves the stronger statement in which each connecting [path in a graph](../../../graph-theory.md#path-in-a-graph) stays inside the outer box.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

We use the [uniqueness of the infinite percolation cluster](../../../bond-percolation.md#uniqueness-of-the-infinite-percolation-cluster) on $\mathbb Z^d$: for $p>p_c$, there is [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) exactly one infinite [percolation cluster](../../../bond-percolation.md#percolation-cluster), denoted $I$. Fix $m$ and let $N>m$. Two observations account for the possible distinct endpoints of the face connections.

First, the probability that some finite [percolation cluster](../../../bond-percolation.md#percolation-cluster) meeting $B(m)$ reaches $\partial B(N)$ tends to zero as $N\to\infty$. There are only finitely many vertices in $B(m)$, and each of their finite [percolation clusters](../../../bond-percolation.md#percolation-cluster) has finite radius; apply the [union bound](../../../probability-inequality.md#boole-s-inequality) and [continuity from above of a measure](../../../measure-theory.md#continuity-from-above-of-a-measure).

Second, all vertices of $I\cap B(m)$ are joined to one another inside $B(N)$ with probability tending to one. On each configuration, this is a finite set of vertices of one connected [percolation cluster](../../../bond-percolation.md#percolation-cluster). Choose a finite open [path in a graph](../../../graph-theory.md#path-in-a-graph) from one such vertex to each of the others; the union of these finitely many paths is contained in some finite box. The assertion is vacuous if the set is empty.

By part (b.ii), each of the two face-connection events within $B(N)$ fails with probability at most $\delta_m^{1/(2d)}$. Outside the two exceptional events just described, their endpoints in $B(m)$ belong to $I$ and can be joined inside $B(N)$. Concatenating the left-face path, that joining path, and the right-face path produces a crossing of $B(N)$. Consequently

$$
\limsup_{N\to\infty}\mathbb P_p(\mathrm{LR}(N)^c)\leq2\delta_m^{1/(2d)}.
$$

Now let $m\to\infty$. Since $\delta_m\to0$,

$$
\boxed{\lim_{N\to\infty}\mathbb P_p(\mathrm{LR}(N))=1.}
$$

The order of limits matters: $m$ is fixed while the finitely many relevant [percolation clusters](../../../bond-percolation.md#percolation-cluster) are connected inside increasingly large boxes.

## 2

↑ **Parent:** [Paper 214](paper-214.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write $N_m=|B(m)|$ and $\theta=\theta(p)>0$. By translation invariance and [linearity of expectation](../../../probability-theory.md#linearity-of-expectation),

$$
\mathbb E_pR(m)=\sum_{x\in B(m)}\mathbb P_p(x\text{ belongs to the infinite cluster})=\theta N_m.
$$

Let $r=\mathbb P_p(R(m)\geq\theta N_m/2)$. Since $0\leq R(m)\leq N_m$, splitting the [expectation](../../../probability-theory.md#expected-value) at the threshold gives

$$
\theta N_m\leq\frac{\theta N_m}{2}(1-r)+N_mr.
$$

Rearranging produces the slightly stronger estimate

$$
\boxed{\mathbb P_p\left(R(m)\geq\frac{\theta(p)|B(m)|}{2}\right)\geq\frac{\theta(p)}{2-\theta(p)}\geq\frac{\theta(p)}2.}
$$

Only the mean and boundedness of the [random variable](../../../random-variable.md) are used; independence of the vertex-membership events is unnecessary.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $m\geq1$, let $S_m$ be the set of vertices of $B(m)$ connected to $\partial B(m)$ by an open [path in a graph](../../../graph-theory.md#path-in-a-graph) using only edges of $B(m)$. Every infinite-cluster vertex of $B(m)$ belongs to $S_m$, by stopping an infinite open [path in a graph](../../../graph-theory.md#path-in-a-graph) at its first boundary visit. Hence the [increasing event](../../../probability-inequality.md#increasing-event)

$$
E_m=\{|S_m|\geq\theta(p)(2m+1)^2/2\}
$$

has probability at least $\theta(p)/2$ by part (a). Importantly, $E_m$ depends only on the edges with both endpoints in $B(m)$.

Open all $8m$ perimeter edges joining successive vertices of $\partial B(m)$. They form a [cycle in a graph](../../../graph-theory.md#cycle-in-a-graph), and opening them joins every vertex of $S_m$ into one [percolation cluster](../../../bond-percolation.md#percolation-cluster), containing the specified perimeter vertex $v_m=(m,0)$. The [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) bounds the probability of this event together with $E_m$ below by $p^{8m}\theta(p)/2$.

Close all $8m+4$ edges in the [edge boundary](../../../combinatorics.md#edge-boundary-in-a-graph) of $B(m)$. These edges are distinct from the internal edges already considered, so their states are independent of those events. The resulting [percolation cluster](../../../bond-percolation.md#percolation-cluster) of $v_m$ is finite, contained in $B(m)$, and has at least $|S_m|$ vertices. Therefore, by translating $v_m$ to the origin,

$$
\mathbb P_p\bigl(\theta(p)(2m+1)^2/2\leq|C|<\infty\bigr)\geq\frac{\theta(p)}2p^{8m}(1-p)^{8m+4}.
$$

For $n\geq1$, choose $m=\lceil\sqrt{n/(2\theta(p))}\rceil$. Then the threshold is at least $n$, and $m\leq(1+(2\theta(p))^{-1/2})\sqrt n$. Put $A=-\log p$ and $B=-\log(1-p)$; both are positive. The preceding lower bound is at least $e^{-c_1\sqrt n}$ with, for example,

$$
\boxed{c_1=8(A+B)\left(1+\frac1{\sqrt{2\theta(p)}}\right)+4B+\log\frac2{\theta(p)},\qquad
\mathbb P_p(n\leq|C|<\infty)\geq e^{-c_1\sqrt n}.}
$$

The construction modifies only order-$m$ boundary edges while trapping order-$m^2$ vertices, which explains the [stretched exponential](../../../analysis.md#stretched-exponential-function) scale. Here $\mathbb N$ is interpreted as the positive integers; the proposed lower bound at $n=0$ would be false because $\theta(p)>0$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Declare an edge of the [planar dual graph](../../../graph-theory.md#planar-dual-graph) open exactly when its crossed primal edge is closed. This [dual bond percolation](../../../graph-theory.md#dual-bond-percolation) has parameter $q=1-p<1/2=p_c$, using the [Harris-Kesten theorem](../../../probability-theory.md#harris-kesten-theorem). We use the standard [exponential tail of subcritical cluster size](../../../probability-theory.md#exponential-tail-of-subcritical-cluster-size): for some $K,a>0$, uniformly in the dual vertex $v$,

$$
\mathbb P_q(|C^*(v)|\geq k)\leq Ke^{-ak},\qquad k\geq1.
$$

This is decay of the number of vertices in the [percolation cluster](../../../bond-percolation.md#percolation-cluster), not merely its radius.

On $\{|C|=n\}$, the geometric fact allowed in the paper supplies a simple dual [cycle in a graph](../../../graph-theory.md#cycle-in-a-graph) surrounding $C$, with length $\ell\geq\alpha\sqrt n$. Every crossed edge is in the [edge boundary](../../../combinatorics.md#edge-boundary-in-a-graph) of $C$ and is therefore closed, so the dual cycle is open. Its $\ell$ distinct vertices lie in one dual [percolation cluster](../../../bond-percolation.md#percolation-cluster) of size at least $\ell$.

A dual [cycle in a graph](../../../graph-theory.md#cycle-in-a-graph) of length $\ell$ surrounding the origin has all its vertices within sup-norm distance $\ell+1$ of the origin: its coordinate spans are at most $\ell$, and the origin lies between each pair of extreme coordinates. There are at most $K_0(\ell+1)^2$ possible dual vertices there. The [union bound](../../../probability-inequality.md#boole-s-inequality) over lengths and possible vertices yields

$$
\mathbb P_p(|C|=n)\leq KK_0\sum_{\ell\geq\lceil\alpha\sqrt n\rceil}(\ell+1)^2e^{-a\ell}\leq K_1e^{-b\sqrt n}
$$

for some $K_1,b>0$, since a polynomial factor can be absorbed into a slower [exponential decay](../../../analysis.md#exponential-decay).

To remove the constant prefactor for all $n\geq1$, first choose $n_0$ so that the bound is at most $e^{-(b/2)\sqrt n}$ for $n\geq n_0$. For the remaining finitely many $n$, use $\mathbb P_p(|C|=n)\leq1-\theta(p)<1$ and choose

$$
\boxed{c_2=\min\left\{\frac b2,\frac{-\log(1-\theta(p))}{\sqrt{n_0}}\right\}>0,\qquad
\mathbb P_p(|C|=n)\leq e^{-c_2\sqrt n}.}
$$

For $1\leq n<n_0$, the chosen $c_2$ ensures $e^{-c_2\sqrt n}\geq1-\theta(p)$.

## 3

↑ **Parent:** [Paper 214](paper-214.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Thomson principle](../../../markov-process.md#thomson-principle) states that the [effective resistance](../../../markov-process.md#effective-resistance) is the minimum [energy of a flow](../../../graph-theory.md#energy-of-a-flow) among all [unit flows](../../../graph-theory.md#unit-flow) from $a$ to $b$:

$$
R_{\mathrm{eff}}(a,b)=\min_{\operatorname{div}\vartheta=\mathbf1_a-\mathbf1_b}\sum_{e\in E}r_e\vartheta(e)^2.
$$

The [flow](../../../graph-theory.md#flow) is antisymmetric on oriented edges, and the sum counts each unoriented edge once. The [Rayleigh monotonicity principle](../../../markov-process.md#rayleigh-monotonicity-principle) states that increasing edge resistances, including deleting edges by setting their resistance to infinity, cannot decrease the [effective resistance](../../../markov-process.md#effective-resistance). Decreasing resistances or identifying vertices cannot increase it.

Take a shortest [path in a graph](../../../graph-theory.md#path-in-a-graph) from $a$ to $b$, of length $d=d_G(a,b)$, and send one unit of [flow](../../../graph-theory.md#flow) along it, with zero [flow](../../../graph-theory.md#flow) on all other edges. Its [energy of a flow](../../../graph-theory.md#energy-of-a-flow) is $d$ because each edge resistance is one. The [Thomson principle](../../../markov-process.md#thomson-principle) gives

$$
\boxed{R_{\mathrm{eff}}(a,b)\leq d_G(a,b).}
$$

Alternatively, delete all edges outside that path and use the [Rayleigh monotonicity principle](../../../markov-process.md#rayleigh-monotonicity-principle); the remaining edges are in series, with total resistance $d$. When $a=b$, both quantities are zero.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Choose a [spanning tree](../../../combinatorics.md#spanning-tree) $T$ of $G$, rooted at $a$. A [depth-first traversal of a tree](../../../combinatorics.md#depth-first-traversal-of-a-tree) gives a deterministic closed walk

$$
v_0=a,v_1,\ldots,v_{2(n-1)}=a
$$

that traverses each edge of $T$ once in each direction and visits every vertex. Define [stopping times](../../../martingale.md#stopping-time) $S_0=0$ and

$$
S_{j+1}=\inf\{t\geq S_j:X_t=v_{j+1}\}.
$$

The [simple random walk](../../../markov-process.md#simple-random-walk) is at $v_j$ at time $S_j$. All these [hitting times](../../../markov-process.md#first-passage-time) have finite mean on the finite connected [graph](../../../graph.md). By the [Strong Markov property](../../../markov-process.md#strong-markov-property),

$$
\mathbb E_a S_{2(n-1)}=\sum_{j=0}^{2(n-1)-1}\mathbb E_{v_j}\tau_{v_{j+1}}.
$$

The [cover time](../../../probability-and-statistics.md#cover-time) is no larger than $S_{2(n-1)}$. Grouping the summands by the two traversals of each tree edge and applying the [commute time identity](../../../markov-process.md#commute-time-identity) gives

$$
\mathbb E_a\tau_{\mathrm{cov}}\leq\sum_{\{u,v\}\in T}\bigl(\mathbb E_u\tau_v+\mathbb E_v\tau_u\bigr)=2|E|\sum_{\{u,v\}\in T}R_{\mathrm{eff}}^G(u,v).
$$

The [effective resistances](../../../markov-process.md#effective-resistance) are measured in the original [graph](../../../graph.md), where each tree-edge pair is adjacent. Part (a) therefore bounds every summand by one, so

$$
\boxed{\mathbb E_a\tau_{\mathrm{cov}}\leq2(n-1)|E|.}
$$

For the one-vertex [graph](../../../graph.md), the [cover time](../../../probability-and-statistics.md#cover-time) is zero and the same bound is immediate.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $d=d_G(a,b)>0$, and for $i=1,\ldots,d$ put

$$
U_i=\{x:d_G(a,x)<i\},\qquad \Pi_i=\partial_eU_i.
$$

Each [edge cutset](../../../graph-theory.md#edge-cutset) $\Pi_i$ separates $a$ from $b$. Adjacent vertices have [graph distances](../../../graph-theory.md#distance-graph-theory) from $a$ differing by at most one. Hence an edge can cross at most one of these level boundaries, so the [edge cutsets](../../../graph-theory.md#edge-cutset) are pairwise edge-disjoint. Write $k_i=|\Pi_i|\geq1$; then $\sum_i k_i\leq|E|$.

The [Nash-Williams inequality](../../../markov-process.md#nash-williams-inequality) for unit conductances gives

$$
R_{\mathrm{eff}}(a,b)\geq\sum_{i=1}^d\frac1{k_i}\geq\frac{d^2}{\sum_i k_i}\geq\frac{d^2}{|E|},
$$

where the middle inequality is the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). One can also derive the first inequality directly: every [unit flow](../../../graph-theory.md#unit-flow) has signed net flux one through each $\Pi_i$, so its [energy of a flow](../../../graph-theory.md#energy-of-a-flow) on that cut is at least $1/k_i$; sum over the disjoint cuts and use the [Thomson principle](../../../markov-process.md#thomson-principle).

Combining with the [commute time identity](../../../markov-process.md#commute-time-identity) yields

$$
\boxed{\mathbb E_a\tau_b+\mathbb E_b\tau_a=2|E|R_{\mathrm{eff}}(a,b)\geq2d_G(a,b)^2.}
$$

The case $a=b$ is trivial. A [path graph](../../../graph-theory.md#path-graph), with $a,b$ its endpoints, attains equality.

## 4

↑ **Parent:** [Paper 214](paper-214.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use the usual implicit convention that the infinite connected [graph](../../../graph.md) is a [locally finite graph](../../../graph-theory.md#locally-finite-graph). This is needed for the [simple random walk](../../../markov-process.md#simple-random-walk) and the finite wired constructions to be defined. Choose finite vertex sets $V_1\subset V_2\subset\cdots$ exhausting $V$, with each [induced subgraph](../../../graph-theory.md#induced-subgraph) $G[V_k]$ connected.

For the [free uniform spanning forest](../../../combinatorics.md#free-uniform-spanning-forest), sample a [uniform spanning tree](../../../combinatorics.md#uniform-spanning-tree) of $G[V_k]$, using only the internal edges. Its limiting law on edge subsets of $G$ is the [free uniform spanning forest](../../../combinatorics.md#free-uniform-spanning-forest) measure:

$$
\boxed{\mathrm{FSF}=\lim_{k\to\infty}\operatorname{UST}(G[V_k]).}
$$

The limit is [weak convergence of probability measures](../../../convergence-of-random-variables.md#weak-convergence-of-probability-measures) on $\{0,1\}^E$, equivalently convergence of every finite-edge event.

For the [wired uniform spanning forest](../../../combinatorics.md#wired-uniform-spanning-forest), form $G_k^{\mathrm w}$ by identifying every vertex outside $V_k$ to one boundary vertex $\partial_k$. Retain all edges with at least one endpoint in $V_k$, preserve parallel edges, and discard loops at $\partial_k$. Sample a [uniform spanning tree](../../../combinatorics.md#uniform-spanning-tree) of this finite multigraph and restrict it to the original internal edges. The limiting law is

$$
\boxed{\mathrm{WSF}=\lim_{k\to\infty}\operatorname{UST}(G_k^{\mathrm w})\big|_E.}
$$

For each fixed finite set of edges the restriction is unambiguous once $k$ is large. The standard exhaustion theorem guarantees that both limits exist and do not depend on the chosen connected exhaustion. Both are random spanning [forests](../../../combinatorics.md#forest); despite their names, they need not be connected.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Fix a root $r$. On a [recurrent graph](../../../markov-process.md#recurrent-graph), a [simple random walk](../../../markov-process.md#simple-random-walk) started at any vertex hits $r$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Run [Wilson's algorithm](../../../combinatorics.md#wilson-s-algorithm) with root $r$: successively attach the [loop-erased random walk](../../../markov-process.md#loop-erased-random-walk) from each new starting vertex, stopped when it hits the existing tree. Every walk terminates [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), because that tree already contains $r$.

To compare the two finite approximations, fix a finite set of edges $K$ and put all their endpoints first in the ordering of starting vertices. In the infinite [graph](../../../graph.md), these finitely many [Wilson's algorithm](../../../combinatorics.md#wilson-s-algorithm) walks have finite lengths [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Their visited vertices, together with their neighbors, are therefore contained in $V_k$ for all sufficiently large $k$ on each realization.

Couple the walks in $G[V_k]$, in $G_k^{\mathrm w}$, and in $G$ using the same neighbor choices while they are in the interior of $V_k$. On the event just described, they encounter neither boundary, so the walks, their chronological [loop erasures](../../../markov-process.md#loop-erasure), and the resulting partial trees agree. Once every endpoint of $K$ has entered the partial tree, later walks cannot add any edge of $K$: they stop on their first hit of the existing tree. Thus the indicators of membership for all edges of $K$ agree in the free and wired [uniform spanning trees](../../../combinatorics.md#uniform-spanning-tree), with probability tending to one.

The two limiting measures agree on every finite-edge event, and therefore

$$
\boxed{\mathrm{WSF}=\mathrm{FSF}.}
$$

This argument also shows that the common [uniform spanning forest](../../../combinatorics.md#uniform-spanning-forest) is a single spanning [tree](../../../combinatorics.md#tree-graph-theory) on a [recurrent graph](../../../markov-process.md#recurrent-graph). The equality refers to probability measures, not to independently sampled forests being identical.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Assume first that deleting an edge leaves two [transient graph](../../../markov-process.md#transient-graph) components. One component supports a finite-energy [unit flow](../../../graph-theory.md#unit-flow) from its endpoint to infinity by the [finite-energy flow criterion for transience](../../../graph-theory.md#finite-energy-flow-criterion-for-transience). Extend that [flow](../../../graph-theory.md#flow) by zero across the deleted edge and throughout the other component. It remains a finite-energy [unit flow](../../../graph-theory.md#unit-flow) on the whole [tree](../../../combinatorics.md#tree-graph-theory), so the [tree](../../../combinatorics.md#tree-graph-theory) is a [transient graph](../../../markov-process.md#transient-graph).

Conversely, root a transient [tree](../../../combinatorics.md#tree-graph-theory) at $o$ and take its finite-energy unit electrical [flow](../../../graph-theory.md#flow) to infinity. On a [tree](../../../combinatorics.md#tree-graph-theory) this [flow](../../../graph-theory.md#flow) can be chosen nonnegative in every direction away from the root: it is obtained as the limit of the currents to wired boundaries, each of which sends nonnegative current into descendant subtrees. At each nonroot vertex its incoming current equals the sum of its outgoing currents, by [flow conservation](../../../graph-theory.md#flow-conservation).

If every vertex reached by positive current had exactly one positive-current child, the unit current would run along a single infinite ray. Every edge of that ray would carry current one, so its [energy of a flow](../../../graph-theory.md#energy-of-a-flow) would be $\sum_{j\geq1}1=\infty$, a contradiction. Thus there is a vertex $v$ with two positive-current child edges, say $(v,x)$ and $(v,y)$.

The restricted [flow](../../../graph-theory.md#flow) below $x$, rescaled by its incoming current, is a finite-energy [unit flow](../../../graph-theory.md#unit-flow) from $x$ to infinity; hence the component below $x$ is a [transient graph](../../../markov-process.md#transient-graph). After removing $(v,x)$, the other component contains $v$, the edge $(v,y)$, and the descendant subtree below $y$. Send unit current along $(v,y)$ and then use the rescaled descendant [flow](../../../graph-theory.md#flow) below $y$, with zero current elsewhere. Its [energy of a flow](../../../graph-theory.md#energy-of-a-flow) is finite, so this component is a [transient graph](../../../markov-process.md#transient-graph) too. Therefore

$$
\boxed{G\text{ is transient}\quad\Longleftrightarrow\quad\exists e\in E:\ G\setminus e\text{ has two transient components}.}
$$

Unit edge resistances are essential here: an infinite ray with sufficiently rapidly decreasing resistances can be transient without any such splitting edge.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

On a [tree](../../../combinatorics.md#tree-graph-theory), every finite connected [induced subgraph](../../../graph-theory.md#induced-subgraph) is itself a [tree](../../../combinatorics.md#tree-graph-theory), and its only [spanning tree](../../../combinatorics.md#spanning-tree) contains all its edges. Thus the [free uniform spanning forest](../../../combinatorics.md#free-uniform-spanning-forest) is deterministic:

$$
\mathrm{FSF}=\delta_E.
$$

Suppose for a contradiction that $G$ is a [transient graph](../../../markov-process.md#transient-graph). By part (c), choose $e=\{a,b\}$ whose removal leaves two [transient graph](../../../markov-process.md#transient-graph) components $T_a,T_b$. Let $R_a,R_b<\infty$ be their [effective resistances to infinity](../../../markov-process.md#effective-resistance-to-infinity) measured from their respective endpoints.

In a wired finite exhaustion, the edge $e$ of resistance one is in parallel with the route from $a$ through $T_a$ to the wired boundary and back through $T_b$ to $b$. The latter route has resistance $R_{a,k}+R_{b,k}$, converging to $R_a+R_b$. Consequently the limiting wired [effective resistance](../../../markov-process.md#effective-resistance) is

$$
R_{\mathrm{eff}}^{\mathrm w}(a,b)=\frac{R_a+R_b}{1+R_a+R_b}<1.
$$

The [edge-inclusion formula for a uniform spanning tree](../../../combinatorics.md#edge-inclusion-formula-for-a-uniform-spanning-tree), the one-edge case of the [transfer-current theorem](../../../combinatorics.md#transfer-current-theorem), states that an edge of conductance $c_e$ is present with probability $c_eR_{\mathrm{eff}}(a,b)$. Passing to the wired limit and using $c_e=1$ gives

$$
\boxed{\mathbb P_{\mathrm{WSF}}(e\notin F)=\frac1{1+R_a+R_b}>0.}
$$

But under the [free uniform spanning forest](../../../combinatorics.md#free-uniform-spanning-forest), $e$ is present with probability one. This contradicts $\mathrm{WSF}=\mathrm{FSF}$. Therefore **the tree is recurrent**. Combined with part (b), this characterizes equality of the free and wired [uniform spanning forests](../../../combinatorics.md#uniform-spanning-forest) on locally finite unweighted [trees](../../../combinatorics.md#tree-graph-theory).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
