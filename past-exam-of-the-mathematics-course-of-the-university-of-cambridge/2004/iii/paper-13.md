# Paper 13

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper13.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper13.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $P$ be the transition matrix of a finite [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain) with at least two states, reversible with [stationary distribution](../../../markov-process.md#stationary-distribution) $\pi$. Its [Dirichlet form of a Markov chain](../../../markov-process.md#dirichlet-form-of-a-markov-chain) is

$$
\mathcal E(f,f)=\frac12\sum_{x,y}\pi(x)P(x,y)(f(x)-f(y))^2.
$$

The [Discrete Poincare inequality](../../../markov-process.md#poincare-inequality-for-a-reversible-markov-chain) states that $\operatorname{Var}_\pi f\leq C\mathcal E(f,f)$ for every real $f$. Its optimal constant is $C=(1-\lambda_2)^{-1}$, where $\lambda_2$ is the second largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of $P$. Indeed, [detailed balance](../../../markov-process.md#detailed-balance) makes $P$ [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) on $L^2(\pi)$. Expand $f-\pi(f)=\sum_{j\geq2}a_jv_j$ in an [orthonormal eigenbasis](../../../linear-operator-theory.md#orthonormal-eigenbasis). Then $\operatorname{Var}_\pi f=\sum a_j^2$ and $\mathcal E(f,f)=\sum(1-\lambda_j)a_j^2$, proving the inequality and its sharpness.

The useful constructive version is the [canonical paths Poincare bound](../../../markov-process.md#canonical-paths-poincare-bound). Choose transition [graph paths](../../../graph-theory.md#path-in-a-graph) $\gamma_{xy}$ between each ordered pair, write $Q(u,v)=\pi(u)P(u,v)$, and define

$$
\rho=\max_{(u,v):Q(u,v)>0}\frac1{Q(u,v)}
\sum_{x,y}\pi(x)\pi(y)|\gamma_{xy}|N_{uv}(\gamma_{xy}),
$$

where $N_{uv}$ counts occurrences of the directed transition. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) along each [path in a graph](../../../graph-theory.md#path-in-a-graph) gives $(f(x)-f(y))^2\leq|\gamma_{xy}|\sum_{\gamma_{xy}}(f(u)-f(v))^2$. Multiply by $\pi(x)\pi(y)/2$ and sum. The identity $\operatorname{Var}_\pi f=\frac12\sum_{x,y}\pi(x)\pi(y)(f(x)-f(y))^2$ proves $\operatorname{Var}_\pi f\leq\rho\mathcal E(f,f)$.

For a [lazy Markov chain](../../../markov-process.md#lazy-markov-chain) this also proves the [mixing time](../../../markov-process.md#mixing-time-of-a-markov-chain) estimate

$$
\|P^t(x,\cdot)-\pi\|_{\mathrm{TV}}
\leq\frac1{2\sqrt{\pi(x)}}e^{-t/\rho}.
$$

To see this, the centred initial density has $L^2(\pi)$ norm at most $\pi(x)^{-1/2}$; laziness puts all nonconstant [eigenvalues](../../../linear-operator-theory.md#eigenvalue) between zero and $1-\rho^{-1}$. Their powers contract that norm, and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) bounds [total variation distance](../../../probability-and-statistics.md#total-variation-distance) by half the density's $L^2(\pi)$ norm.

Here is a precise sufficient density condition for the permanent application: **every row and every column has more than $n/2$ ones**. Interpret the [permanent of a matrix](../../../linear-algebra.md#permanent-mathematics) as the number $m_n$ of [perfect matchings](../../../graph-theory.md#perfect-matching) in its [bipartite graph](../../../graph-theory.md#bipartite-graph), with $n$ [vertices](../../../graph.md#vertex-graph-theory) per side. Write $m_k$ for the number of $k$-edge [matchings in a graph](../../../graph-theory.md#matching-graph-theory).

First prove the [short augmenting paths in a dense bipartite graph](../../../graph-theory.md#short-augmenting-paths-in-a-dense-bipartite-graph) bound. Given a nonperfect [matching in a graph](../../../graph-theory.md#matching-graph-theory), choose unmatched $u,v$ on opposite sides. If either has an unmatched [neighbour](../../../graph-theory.md#neighbour-of-a-vertex), augment with one [edge](../../../graph-theory.md#edge-of-a-graph). Otherwise the matched partners of $N(u)$ and the [neighbours](../../../graph-theory.md#neighbour-of-a-vertex) $N(v)$ are subsets of the same $n$-element side whose total size exceeds $n$. Their intersection gives an alternating [path in a graph](../../../graph-theory.md#path-in-a-graph) $u,b,a,v$ of length three, with $ab$ a matching [edge](../../../graph-theory.md#edge-of-a-graph). Repeating proves $m_n>0$. Choose augmentations by a fixed deterministic rule. A reverse augmentation is specified by at most four [vertices](../../../graph.md#vertex-graph-theory), so a next-size [matching in a graph](../../../graph-theory.md#matching-graph-theory) has at most $C_0=2n^4$ preimages. Therefore

$$
m_k\leq C_0m_{k+1},\qquad m_{n-j}\leq C_0^jm_n.
$$

Use the [matching generating function](../../../graph-theory.md#matching-generating-function) $Z(\lambda)=\sum_{k=0}^nm_k\lambda^k$ and the [weighted matching Markov chain](../../../markov-process.md#weighted-matching-markov-chain) on all [matchings in a graph](../../../graph-theory.md#matching-graph-theory), with stationary weights $\pi_\lambda(M)=\lambda^{|M|}/Z(\lambda)$. It stays put with probability $1/2$; otherwise it chooses a [graph](../../../graph.md) [edge](../../../graph-theory.md#edge-of-a-graph) uniformly and proposes its deletion, its addition if both endpoints are unmatched, or its exchange for the unique incident matching [edge](../../../graph-theory.md#edge-of-a-graph) if precisely one endpoint is matched. Other proposals stay put. Accept with probability $\min(1,\lambda^{|M'|-|M|})$. Reverse proposals use the opposite exchanged [edge](../../../graph-theory.md#edge-of-a-graph), so [detailed balance](../../../markov-process.md#detailed-balance) holds. Deletions connect every state to the empty [matching in a graph](../../../graph-theory.md#matching-graph-theory).

For completeness, the [canonical paths for the weighted matching chain](../../../markov-process.md#canonical-paths-for-the-weighted-matching-chain) give a polynomial bound without assuming a mixing theorem. The [symmetric difference](../../../set.md#symmetric-difference) $I\triangle F$ consists of alternating [graph paths](../../../graph-theory.md#path-in-a-graph) and [graph cycles](../../../graph-theory.md#cycle-in-a-graph). Order its components deterministically, orient open components from their smaller endpoint, and convert them from $I$ to $F$ by moving an unmatched endpoint with exchanges. If the first [edge](../../../graph-theory.md#edge-of-a-graph) belongs to $I$, delete it first. For a [graph cycle](../../../graph-theory.md#cycle-in-a-graph), delete one $I$-[edge](../../../graph-theory.md#edge-of-a-graph), move the unmatched endpoint around the opened cycle, then insert the last $F$-[edge](../../../graph-theory.md#edge-of-a-graph). Each intermediate state is a [matching in a graph](../../../graph-theory.md#matching-graph-theory), and each entire transition [path in a graph](../../../graph-theory.md#path-in-a-graph) has length at most $4n$.

Fix a directed transition with initial state $M$. The complementary edge set $K=I\triangle F\triangle M$ agrees with one of the two [matchings in a graph](../../../graph-theory.md#matching-graph-theory) outside the active component and has at most two degree-two [vertices](../../../graph.md#vertex-graph-theory) on that component. Remove at most two offending [edges](../../../graph-theory.md#edge-of-a-graph) to obtain a [matching in a graph](../../../graph-theory.md#matching-graph-theory) $K'$. Store those [edges](../../../graph-theory.md#edge-of-a-graph) and one bit specifying the initial alternating colour of the active component. This encoding is injective for the fixed transition: it restores $K$ and $I\triangle F=M\triangle K$, identifies the active component from the changed [edges](../../../graph-theory.md#edge-of-a-graph), and recovers the two colours using the fixed component order. Completed components have $F$'s colour in $M$, pending components have $I$'s colour, and the stored bit resolves the active component. Common [edges](../../../graph-theory.md#edge-of-a-graph) are $M\cap K$.

There are at most $2(m+1)^2$ auxiliary records per $K'$, where $m$ is the number of [graph](../../../graph.md) [edges](../../../graph-theory.md#edge-of-a-graph). If $d=|K|-|K'|\leq2$, then

$$
\pi_\lambda(I)\pi_\lambda(F)=\lambda^d\pi_\lambda(M)\pi_\lambda(K').
$$

Also $Q(M,M')\geq\pi_\lambda(M)/(2m\max(\lambda,\lambda^{-1}))$. Sum over the encodings and use the [path](../../../geometry-and-topology.md#continuous-path) length bound to obtain

$$
\rho\leq16nm(m+1)^2\max(1,\lambda^2)\max(\lambda,\lambda^{-1}).
$$

This is polynomial whenever $\lambda$ and $\lambda^{-1}$ are polynomially bounded. Starting at the empty [matching in a graph](../../../graph-theory.md#matching-graph-theory), $\log(1/\pi_\lambda(\varnothing))=\log Z(\lambda)\leq m\log(1+\lambda)$, so the [Discrete Poincare inequality](../../../markov-process.md#poincare-inequality-for-a-reversible-markov-chain) gives polynomial-time sampling to any prescribed [total variation distance](../../../probability-and-statistics.md#total-variation-distance). The addition/deletion/exchange construction is also described in [Section 12.4 of Jerrum and Sinclair's survey](https://people.eecs.berkeley.edu/~sinclair/mcmc.pdf).

It remains to turn sampling into a relative count; merely sampling [perfect matchings](../../../graph-theory.md#perfect-matching) would not do that. For $0<\varepsilon\leq1/2$, choose $\lambda_0=\varepsilon/(8m)$ and $\lambda_*=8C_0/\varepsilon$. The elementary bounds above give

$$
1\leq Z(\lambda_0)\leq(1+\lambda_0)^m\leq1+\varepsilon/4,
\qquad
1\leq\frac{Z(\lambda_*)}{m_n\lambda_*^n}
\leq\sum_{j=0}^n(C_0/\lambda_*)^j\leq1+\varepsilon/4.
$$

Choose a schedule $\lambda_0<\lambda_1<\cdots<\lambda_J=\lambda_*$ whose successive ratios are at most $1+1/n$. It has $J=O(n\log(n/\varepsilon))$ stages. The [annealing ratios for a matching generating function](../../../graph-theory.md#annealing-ratios-for-a-matching-generating-function) satisfy

$$
\frac{Z(\lambda_{j+1})}{Z(\lambda_j)}
=\mathbb E_{\pi_{\lambda_j}}\left(\frac{\lambda_{j+1}}{\lambda_j}\right)^{|M|}.
$$

Each observable lies in $[1,e]$, so the [Hoeffding inequality](../../../probability-inequality.md#hoeffding-inequality) gives relative accuracy $\eta=\varepsilon/(10J)$ with $O(\eta^{-2}\log(J/\delta))$ independent samples per stage. Run independent copies of the chain from the empty [matching in a graph](../../../graph-theory.md#matching-graph-theory); make the [total variation distance](../../../probability-and-statistics.md#total-variation-distance) per sample at most $\delta/(3JK)$, where $K$ is that sample count. The [coupling characterization of total variation distance](../../../probability-and-statistics.md#coupling-characterization-of-total-variation-distance) and the [union bound](../../../probability-inequality.md#boole-s-inequality) make the entire sample collection coincide with exact stationary samples except with probability at most $\delta/3$. Choose the sample-count constant so all stationary sample means are accurate except with probability at most $\delta/3$.

Let $\widehat R$ be the product of the sample means, and output $\widehat p=\widehat R/\lambda_*^n$. On the successful event its multiplicative error relative to $Z(\lambda_*)/Z(\lambda_0)$ lies between $e^{-\varepsilon/5}$ and $e^{\varepsilon/5}$. Combining the two endpoint bounds proves

$$
\boxed{\mathbb P\bigl((1-\varepsilon)\operatorname{per}A\leq\widehat p\leq(1+\varepsilon)\operatorname{per}A\bigr)\geq1-\delta.}
$$

Activities, sample counts, simulation lengths and rational bit lengths are polynomial in $n,\varepsilon^{-1},\log(\delta^{-1})$. Thus this is a [fully polynomial randomized approximation scheme](../../../mathematical-optimization.md#fully-polynomial-randomized-approximation-scheme). Small dimensions can be evaluated directly.

## 2

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For disjoint [vertex sets](../../../graph.md#vertex-set) $A,B$, define their [edge density of a bipartite graph](../../../probabilistic-combinatorics.md#edge-density-of-a-bipartite-graph) by $d(A,B)=e(A,B)/(|A||B|)$. They form a [regular pair](../../../probabilistic-combinatorics.md#regular-pair-of-vertex-sets) with parameter $\varepsilon$ if every $A'\subseteq A,B'\subseteq B$ with $|A'|\geq\varepsilon|A|$, $|B'|\geq\varepsilon|B|$ satisfies $|d(A',B')-d(A,B)|\leq\varepsilon$.

The [Szemerédi regularity lemma](../../../probabilistic-combinatorics.md#szemeredi-regularity-lemma) says that for every $\varepsilon>0$ and minimum cell count $k_0$, some $K,n_0$ have the following property. Every [graph](../../../graph.md) on $n\geq n_0$ [vertices](../../../graph.md#vertex-graph-theory) admits

$$
V=V_0\sqcup V_1\sqcup\cdots\sqcup V_k,
\qquad k_0\leq k\leq K,
$$

with $|V_0|\leq\varepsilon n$, equal-sized $V_1,\ldots,V_k$, and at most $\varepsilon k^2$ unordered [irregular pairs](../../../probabilistic-combinatorics.md#irregular-pair-of-vertex-sets). It is enough to consider $0<\varepsilon<1/2$.

Prove this using [equitable regularity energy](../../../probabilistic-combinatorics.md#equitable-regularity-energy). Treat exceptional [vertices](../../../graph.md#vertex-graph-theory) as singleton cells and set

$$
q(\mathcal P)=\frac1{n^2}\sum_{A,B\in\mathcal P}|A||B|d(A,B)^2,
$$

with ordered pairs and the adjacency indicator also defining diagonal densities. Then $0\leq q\leq1$. The [refinement variance identity for regularity energy](../../../probabilistic-combinatorics.md#refinement-variance-identity-for-regularity-energy) proves refinement cannot decrease $q$:

$$
\sum_{a,b}|A_a||B_b|d(A_a,B_b)^2-|A||B|d(A,B)^2
=\sum_{a,b}|A_a||B_b|(d(A_a,B_b)-d(A,B))^2.
$$

An [irregular pair](../../../probabilistic-combinatorics.md#irregular-pair-of-vertex-sets) supplies witness subsets of relative sizes at least $\varepsilon$ whose density differs by more than $\varepsilon$. Refining along those witnesses raises $q$ by more than $\varepsilon^4L^2/n^2$ per orientation, where $L$ is the common cell size. If there are more than $\varepsilon k^2$ [irregular pairs](../../../probabilistic-combinatorics.md#irregular-pair-of-vertex-sets), the increase is greater than $\varepsilon^5(kL/n)^2\geq\varepsilon^5/4$, provided the exceptional set has size at most $n/2$.

Refine each cell by all its witness subsets; this produces at most $2^k$ atoms per cell. Restore equal sizes by the [equalization with a controlled exceptional set](../../../probabilistic-combinatorics.md#equalization-with-a-controlled-exceptional-set): cut each atom into blocks of size $\lfloor L/4^k\rfloor$ and declare its remainder exceptional, still retaining every such [vertex](../../../graph.md#vertex-graph-theory) as a singleton in the energy. This is another refinement, so no energy is lost. At most $k2^k\lfloor L/4^k\rfloor\leq n2^{-k}$ [vertices](../../../graph.md#vertex-graph-theory) become exceptional, and, when $L\geq2\cdot4^k$, at most $2k4^k$ new nonexceptional cells occur.

Put $T=\lceil4\varepsilon^{-5}\rceil$ and start with $k\geq k_0$ so large that $T2^{-k}\leq\varepsilon/2$. An initial equitable partition has at most $\varepsilon n/2$ exceptional [vertices](../../../graph.md#vertex-graph-theory) when $n$ is sufficiently large. Subsequent cell counts only increase, so the total added exceptional set has size at most $\varepsilon n/2$. The recurrence $k\mapsto2k4^k$, iterated at most $T$ times, supplies a finite bound $K$; choose $n_0$ large enough that every intermediate $L$ meets the size requirement. More than $T$ unsuccessful refinements would raise $q$ above one. The process must therefore stop with the required [regular pairs](../../../probabilistic-combinatorics.md#regular-pair-of-vertex-sets). This proves the lemma.

Its usefulness comes from replacing an arbitrarily large [graph](../../../graph.md) by the bounded [reduced graph of a regularity partition](../../../probabilistic-combinatorics.md#reduced-graph-of-a-regularity-partition). For fixed positive cross-density, the [graph embedding lemma for regular pairs](../../../probabilistic-combinatorics.md#graph-embedding-lemma-for-regular-pairs) lifts fixed configurations from the reduced [graph](../../../graph.md) to the original one. In particular, three sufficiently regular positive-density pairs contain many [triangles in a graph](../../../graph.md#triangle-in-a-graph). Deleting exceptional, intracell, irregular and sparse-pair [edges](../../../graph-theory.md#edge-of-a-graph) then gives the [triangle removal lemma](../../../probabilistic-combinatorics.md#triangle-removal-lemma): a [graph](../../../graph.md) with sufficiently few triangles can be made [triangle-free](../../../graph.md#triangle-free-graph) by deleting $o(n^2)$ [edges](../../../graph-theory.md#edge-of-a-graph). A triangle surviving in the reduced [graph](../../../graph.md) would force a positive proportion of the original possible triangles, a contradiction. More generally this approach yields the [clique removal lemma](../../../probabilistic-combinatorics.md#clique-removal-lemma) and the asymptotic [Erdős-Stone theorem](../../../graph-theory.md#erdos-stone-theorem). Applied to the tripartite [graph](../../../graph.md) encoding $x+z=2y$, triangle removal also gives [Roth theorem](../../../number-theory.md#roth-s-theorem) on three-term [arithmetic progressions](../../../arithmetic.md#arithmetic-progression). The price is that the energy argument gives a very rapidly growing, iterated-exponential bound on $K(\varepsilon)$; the lemma is a structural tool, not a promise of small practical constants.

## 3

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $t$ be the maximum number of positive [Euclidean distances](../../../topological-analysis.md#euclidean-distance) from one of the $n$ points to the others. It suffices to prove the stronger [Székely distinct-distance bound](../../../combinatorics.md#szekely-distinct-distance-bound), $t\geq cn^{4/5}$. Here $n\geq2$; enlarge constants to handle bounded $n$.

First prove the [crossing lemma for multigraphs](../../../graph-theory.md#crossing-lemma-for-multigraphs). In an optimal drawing of a loopless [multigraph](../../../graph.md#multigraph) with $v$ [vertices](../../../graph.md#vertex-graph-theory), $e$ [edges](../../../graph-theory.md#edge-of-a-graph) and maximum parallel multiplicity $\mu$, crossings of incident [edges](../../../graph-theory.md#edge-of-a-graph) can be removed by interchanging initial segments, so each remaining crossing involves four distinct [vertices](../../../graph.md#vertex-graph-theory). In each parallel class choose one of its [edges](../../../graph-theory.md#edge-of-a-graph) with probability $1/\mu$ per [edge](../../../graph-theory.md#edge-of-a-graph), selecting none with the remaining probability. Independently keep each [vertex](../../../graph.md#vertex-graph-theory) with probability $p$. The resulting [simple graph](../../../graph.md#simple-graph) has expected [edge](../../../graph-theory.md#edge-of-a-graph) count $p^2e/\mu$, expected [vertex](../../../graph.md#vertex-graph-theory) count $pv$, and expected crossings $p^4X/\mu^2$, where $X$ is the original crossing count. Deleting one [edge](../../../graph-theory.md#edge-of-a-graph) per crossing and using the allowed [planar graph edge bound](../../../graph-theory.md#planar-graph-edge-bound) yields

$$
\frac{p^4X}{\mu^2}\geq\frac{p^2e}{\mu}-3pv.
$$

If $e\geq4\mu v$, take $p=4\mu v/e$ to obtain

$$
X\geq\frac{e^3}{64\mu v^2}.
$$

The case $\mu=1$ is the ordinary [crossing lemma](../../../graph-theory.md#crossing-lemma).

We also need the [rich line bound](../../../combinatorics.md#rich-line-bound). Given $L$ [lines](../../../geometry-and-topology.md#straight-line), connect consecutive incidence points on each [line](../../../geometry-and-topology.md#straight-line) by straight [edges](../../../graph-theory.md#edge-of-a-graph). This [simple graph](../../../graph.md#simple-graph) has at least $I-L$ [edges](../../../graph-theory.md#edge-of-a-graph), where $I$ is the total number of incidences, and at most $L^2$ crossings. The [crossing lemma](../../../graph-theory.md#crossing-lemma) gives $I=O((nL)^{2/3}+n+L)$, proving the [Szemerédi–Trotter theorem](../../../combinatorics.md#szemeredi-trotter-theorem) here rather than assuming it. For [lines](../../../geometry-and-topology.md#straight-line) containing at least $k$ points, $I\geq kL$, and absorbing the additive $L$ term gives

$$
L_{\geq k}=O(n^2/k^3+n/k),\qquad k\geq2.
$$

For bounded $k$, counting point pairs gives the same estimate with a larger absolute constant. Grouping rich [lines](../../../geometry-and-topology.md#straight-line) into occupancy ranges $2^jk\leq s<2^{j+1}k$ and summing the resulting geometric series proves

$$
\sum_{\ell:\,|P\cap\ell|\geq k}|P\cap\ell|
=O(n^2/k^2+n\log n).
$$

Now form the [circular-arc graph for distinct distances](../../../combinatorics.md#circular-arc-graph-for-distinct-distances). Around every point draw each positive-distance [circle](../../../topology.md#circle) centred there; there are at most $nt$ such [circles](../../../topology.md#circle). A [circle](../../../topology.md#circle) with at least three of the original points contributes one [edge](../../../graph-theory.md#edge-of-a-graph) between each consecutive pair around it. Discard the [circles](../../../topology.md#circle) with at most two points. Since the total number of centre-to-point incidences is $n(n-1)$, the remaining loopless [multigraph](../../../graph.md#multigraph) has

$$
e\geq n(n-1)-2nt.
$$

Its circular-arc drawing has $O(n^2t^2)$ crossings: two distinct [circles](../../../topology.md#circle) have at most two intersections, and small perturbations remove tangencies and multiple crossings without changing this order.

The apparent difficulty is unbounded parallel multiplicity. The [rich-bisector deletion bound](../../../combinatorics.md#rich-bisector-deletion-bound) controls it. Every centre supporting an arc between fixed endpoints lies on their [perpendicular bisector](../../../geometry-and-topology.md#perpendicular-bisector). Distinct parallel arcs come from distinct centres, since their common endpoints determine the radius once the centre is fixed. Thus multiplicity at least $k$ makes that [line](../../../geometry-and-topology.md#straight-line) contain at least $k$ of the points. For a [line](../../../geometry-and-topology.md#straight-line) with $s$ centres, each of its at most $st$ [circles](../../../topology.md#circle) has at most two consecutive-point arcs symmetric about that [line](../../../geometry-and-topology.md#straight-line), one at each end of its diameter along the [line](../../../geometry-and-topology.md#straight-line). The occupancy sum above therefore bounds the number of high-multiplicity arcs by

$$
O(tn^2/k^2+tn\log n).
$$

If $t\geq n^{4/5}$ there is nothing to prove. Otherwise $t\log n=o(n)$ and $t=o(n)$. Choose $k=\lceil K\sqrt t\rceil$ with a sufficiently large absolute constant $K$. The first deletion term is at most a small fixed fraction of $n^2$ and the second is $o(n^2)$. A remaining [multigraph](../../../graph.md#multigraph) therefore has $e_1\geq c_1n^2$ [edges](../../../graph-theory.md#edge-of-a-graph) and multiplicity at most $k$. For large $n$, $e_1\geq4kn$, so the [crossing lemma for multigraphs](../../../graph-theory.md#crossing-lemma-for-multigraphs) gives

$$
Cn^2t^2\geq X_1\geq\frac{e_1^3}{64kn^2}
\geq c_2\frac{n^4}{\sqrt t}.
$$

Rearranging,

$$
\boxed{t^{5/2}\geq c_3n^2,\qquad t\geq cn^{4/5}.}
$$

The whole [distinct-distance set](../../../combinatorics.md#distinct-distance-set) contains those distances from the selected point, proving the requested bound. The circular-arc method and the stronger one-point conclusion are due to [Székely](https://www.cs.tau.ac.il/~michas/szekely.pdf).

## 4

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $\operatorname{CLIQUE}_{n,m}$ be the [monotone Boolean function](../../../combinatorics.md#monotone-boolean-function) of the [edge](../../../graph-theory.md#edge-of-a-graph) indicators asserting that an $n$-[vertex](../../../graph.md#vertex-graph-theory) [graph](../../../graph.md) contains an $m$-[clique](../../../graph-theory.md#clique-graph-theory). We prove a [superpolynomial monotone clique lower bound](../../../computer-science.md#superpolynomial-monotone-clique-lower-bound) using a finite [lattice](../../../mathematical-logic.md#lattice) of approximations. The only circuit theorem assumed is the [Razborov gate-by-gate approximation lemma](../../../computer-science.md#razborov-gate-by-gate-approximation-lemma).

Fix integers $\ell,r\geq2$. Consider upward-closed [set families](../../../extremal-set-theory.md#set-family) $A$ of subsets of $[n]$ of size at most $\ell$. Impose the [Razborov closure](../../../computer-science.md#razborov-closure) rule: if $W_1,\ldots,W_r\in A$ have pairwise intersections contained in $W$, adjoin $W$ whenever $|W|\leq\ell$. Also normalize a family containing a set of size zero or one to the full family, since its clique predicate is identically true. Represent it by

$$
\langle A\rangle=\{G:G[W]\text{ is complete for some }W\in A\}.
$$

Closed families form the [finite lattice approximation for monotone clique circuits](../../../computer-science.md#finite-lattice-approximation-for-monotone-clique-circuits), with meet $A\cap B$ and join $\operatorname{cl}(A\cup B)$. An input [edge](../../../graph-theory.md#edge-of-a-graph) is represented by the family of its supersets up to size $\ell$. The constant predicates have the empty and full families. The assumed approximation theorem says that a size-$S$ circuit's output disagreement is covered by at most $S$ local gate errors:

$$
\delta_\wedge(A,B)=(\langle A\rangle\cap\langle B\rangle)\setminus\langle A\cap B\rangle,
\qquad
\delta_\vee(A,B)=\langle\operatorname{cl}(A\cup B)\rangle\setminus(\langle A\rangle\cup\langle B\rangle).
$$

We need the [Erdős–Rado sunflower lemma](../../../set-theory.md#erdos-rado-sunflower-lemma): an $s$-[uniform set family](../../../extremal-set-theory.md#uniform-set-family) with more than $s!(r-1)^s$ members contains $r$ members with a common pairwise intersection. Its short induction proves the bound. A maximal disjoint subfamily either has $r$ members, already the required empty-core [delta-system](../../../set-theory.md#delta-system), or its union has at most $s(r-1)$ points and meets every member. Some point then occurs in more than $(s-1)!(r-1)^{s-1}$ members. Delete it, apply the induction hypothesis, and restore it to the core. Thus an $r$-closed family has at most

$$
a_s\leq s!(r-1)^s
$$

inclusion-minimal $s$-sets: a sunflower among those members would force its proper core and contradict minimality. This is the [sunflower bound for minimal members of a Razborov-closed family](../../../computer-science.md#sunflower-bound-for-minimal-members-of-a-razborov-closed-family).

For positive inputs choose a uniform $m$-subset $Z$ and the [graph](../../../graph.md) $K_Z$ having exactly the [edges](../../../graph-theory.md#edge-of-a-graph) of its [clique](../../../graph-theory.md#clique-graph-theory). Put $q=\ell rm/n$ and suppose $q\leq1/2$. A nonuniversal family has no minimal member of size at most one, so it accepts at most

$$
\sum_{s=2}^\ell s!(r-1)^s\left(\frac mn\right)^s
\leq\sum_{s=2}^\ell q^s\leq2q^2
$$

of positive inputs. Here $\mathbb P(W\subseteq Z)=(m)_{|W|}/(n)_{|W|}\leq(m/n)^{|W|}$.

If $K_Z$ is in a meet-error set, it contains minimal witnesses $X\in A,Y\in B$. Their union must have size greater than $\ell$, since otherwise upward closure would put it in $A\cap B$. At least one witness therefore has size greater than $\ell/2$. The same counting and the [union bound](../../../probability-inequality.md#boole-s-inequality) give the [positive clique error of a truncated lattice meet](../../../computer-science.md#positive-clique-error-of-a-truncated-lattice-meet):

$$
\mathbb P(K_Z\in\delta_\wedge(A,B))
\leq2\sum_{s>\ell/2}s!(r-1)^s(m/n)^s
\leq4q^{\ell/2}.
$$

For negative inputs independently assign one of $m-1$ colours to each [vertex](../../../graph.md#vertex-graph-theory), joining differently coloured [vertices](../../../graph.md#vertex-graph-theory). Every resulting [complete multipartite graph](../../../graph-theory.md#complete-multipartite-graph) is $m$-[clique](../../../graph-theory.md#clique-graph-theory)-free. Consider one forcing step adjoining $W$. If its [clique](../../../graph-theory.md#clique-graph-theory) is newly accepted, $W$ is rainbow while all witnesses $W_i$ are not. Condition on the colours of $W$. The sets $W_i\setminus W$ are disjoint, so their non-rainbow events are [conditionally independent](../../../random-variable.md#conditional-independence). For each witness, every possible collision either involves two random petal colours or one petal colour and one fixed core colour; its probability is at most

$$
\frac{\binom\ell2}{m-1}.
$$

When this is at most $1/2$, a step makes a negative error with probability at most $2^{-r}$. Upward closure itself introduces no extra accepted [graphs](../../../graph.md), and normalization introduces no extra error beyond the forcing step that produced a set of size at most one. At most $\sum_{j=0}^\ell\binom nj\leq n^{\ell+1}$ sets can be forced. The [negative colouring error of a forced-set closure](../../../computer-science.md#negative-colouring-error-of-a-forced-set-closure) is therefore

$$
\mathbb P(G_{\mathrm{colour}}\in\delta_\vee(A,B))\leq n^{\ell+1}2^{-r}.
$$

Set $m=r=\lfloor n^{1/4}\rfloor$ and $\ell=\lfloor\log_2n\rfloor$. For sufficiently large $n$, both probability conditions hold and $2q^2<1/2$. If the output approximation is nonuniversal, it misses at least half the positive inputs, so the [Razborov gate-by-gate approximation lemma](../../../computer-science.md#razborov-gate-by-gate-approximation-lemma) forces $1/2\leq4Sq^{\ell/2}$. If it is universal, it accepts every negative colouring input, forcing $1\leq Sn^{\ell+1}2^{-r}$. Consequently

$$
S\geq\min\left\{\frac1{8q^{\ell/2}},\frac{2^r}{n^{\ell+1}}\right\}.
$$

Since $\log(1/q)\geq\frac12\log n-\log\ell$ and $r$ grows faster than $(\log n)^2$, both terms imply

$$
\boxed{S\geq\exp(c(\log n)^2)=n^{c\log n}}
$$

for an absolute positive $c$ and all sufficiently large $n$. This is superpolynomial in the $\binom n2$ input bits. The argument concerns AND/OR [monotone circuits](../../../computer-science.md#monotone-circuit); it gives no such bound for circuits allowed negation.

## 5

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The [Frankl-Wilson theorem](../../../extremal-set-theory.md#frankl-wilson-theorem) is a striking example of the [polynomial method in combinatorics](../../../combinatorics.md#polynomial-method-in-combinatorics): an intersection restriction creates a family of [linearly independent](../../../vector-space.md#linear-independence) low-degree [polynomials](../../../polynomial.md), whose dimension bounds the set family. Let $p$ be a [prime number](../../../number-theory.md#prime-number), let $L\subseteq\mathbb F_p$ have $s$ elements, and let $\mathcal F$ be a [set family](../../../extremal-set-theory.md#set-family) such that member sizes modulo $p$ avoid $L$ while every distinct pair has intersection size in $L$ modulo $p$. Its general modular form gives

$$
|\mathcal F|\leq\sum_{j=0}^s\binom nj.
$$

If all members have the same size $k$ and $s\leq k$, the uniform refinement gives **$|\mathcal F|\leq\binom ns$**.

For the proof, work over the [finite field](../../../algebra.md#finite-field) $\mathbb F_p$ and associate to $A\in\mathcal F$ the [modular intersection polynomial](../../../extremal-set-theory.md#modular-intersection-polynomial)

$$
P_A(x)=\prod_{\lambda\in L}\left(\sum_{i\in A}x_i-\lambda\right).
$$

At the [characteristic vector of a set](../../../extremal-set-theory.md#characteristic-vector-of-a-set) $B$, this equals zero for $B\ne A$ and is nonzero for $B=A$. A linear relation among the evaluation functions therefore has every coefficient zero. The [multilinear reduction on the Boolean cube](../../../polynomial.md#multilinear-reduction-on-the-boolean-cube), replacing $x_i^a$ by $x_i$ for $a\geq1$, preserves these evaluations and the degree bound $s$. There are $\sum_{j=0}^s\binom nj$ possible square-free [monomials](../../../polynomial.md#monomial), proving the general form.

For uniform members, the [low-degree evaluation rank on a uniform layer](../../../extremal-set-theory.md#low-degree-evaluation-rank-on-a-uniform-layer) supplies the sharper dimension bound. To verify this without division modulo $p$, form the integer incidence [matrix](../../../vector-space.md#matrix) with rows indexed by subsets $S$ of size at most $s$, columns indexed by $k$-subsets $B$, and entries $\mathbf1_{S\subseteq B}$. Over the [rational numbers](../../../number-theory.md#rational-number), a row with $|S|=j$ is $\binom{k-j}{s-j}^{-1}$ times the sum of all size-$s$ rows containing $S$. Its [matrix rank](../../../vector-space.md#matrix-rank) is at most $\binom ns$. Every larger integer minor is consequently zero and remains zero modulo $p$, giving the same bound over $\mathbb F_p$. The nonzero diagonal evaluation [matrix](../../../vector-space.md#matrix) of the $P_A$ then forces $|\mathcal F|\leq\binom ns$.

The theorem, proved by Frankl and Wilson in 1981, extends the theme of the [Ray-Chaudhuri–Wilson theorem](../../../extremal-set-theory.md#ray-chaudhuri-wilson-theorem) from ordinary intersection sizes to residues. Modular restrictions can be weaker than exact intersection restrictions yet still force unexpectedly small families. Here are three consequences from one explicit [modular intersection graph](../../../extremal-set-theory.md#modular-intersection-graph).

Take $N=4p-1$, $k=2p-1$, and let the [vertices](../../../graph.md#vertex-graph-theory) be all $k$-subsets of $[N]$, with an [edge](../../../graph-theory.md#edge-of-a-graph) exactly when the intersection has size $p-1$. An [independent set](../../../graph-theory.md#independent-set-graph-theory) avoids the only possible off-diagonal intersection congruent to $k$ modulo $p$, so applying the [Frankl-Wilson theorem](../../../extremal-set-theory.md#frankl-wilson-theorem) with $L=\mathbb F_p\setminus\{p-1\}$ gives

$$
\alpha(G)\leq B:=\binom N{p-1}.
$$

A [clique](../../../graph-theory.md#clique-graph-theory) has one exact intersection size. Apply the uniform theorem modulo a prime larger than $k$, with $L=\{p-1\}$, to get $\omega(G)\leq N$. Since there are $v=\binom Nk$ [vertices](../../../graph.md#vertex-graph-theory), this gives the explicit asymmetric [Ramsey number](../../../ramsey-theory.md#ramsey-number) bound **$R(N+1,B+1)>v$**. It illustrates how algebraic constructions produce graphs with simultaneously restricted [cliques](../../../graph-theory.md#clique-graph-theory) and [independent sets](../../../graph-theory.md#independent-set-graph-theory).

For a geometric application, map each [vertex](../../../graph.md#vertex-graph-theory) to $x_A=\mathbf1_A/\sqrt{2p}$ in $\mathbb R^N$. Then $|x_A-x_B|^2=(k-|A\cap B|)/p$, so [edges](../../../graph-theory.md#edge-of-a-graph) have unit [Euclidean distance](../../../topological-analysis.md#euclidean-distance). Every proper colouring of Euclidean space therefore colours this finite [graph](../../../graph.md), giving

$$
\chi(\mathbb R^N)\geq\chi(G)\geq\frac{\binom N{2p-1}}{\binom N{p-1}}.
$$

The [Stirling formula](../../../real-analysis.md#stirling-formula) gives the ratio as $\exp((\log2-H(1/4)+o(1))N)$, where $H(a)=-a\log a-(1-a)\log(1-a)$ is the [binary entropy function](../../../combinatorics.md#binary-entropy-function) in natural-log units. The positive constant $\log2-H(1/4)$ proves an exponential [chromatic number of Euclidean space](../../../graph-theory.md#chromatic-number-of-euclidean-space) lower bound along these dimensions.

Finally, a quadratic embedding converts this same forbidden intersection into a forbidden [diameter](../../../topological-analysis.md#diameter) pair. Set $u_A=2\mathbf1_A-\mathbf1$ and $Q_A=u_Au_A^T$. The [quadratic sign-vector diameter formula](../../../geometry-and-topology.md#quadratic-sign-vector-diameter-formula) follows from the [Frobenius inner product](../../../linear-algebra.md#frobenius-inner-product):

$$
\|Q_A-Q_B\|_F^2=2\bigl(N^2-(u_A\cdot u_B)^2\bigr),
\qquad
u_A\cdot u_B=4|A\cap B|-4p+3.
$$

For distinct members the smallest possible absolute inner product is one, attained exactly when the intersection is $p-1$. Thus maximum-distance pairs are exactly [edges](../../../graph-theory.md#edge-of-a-graph) of $G$. The matrices have common diagonal; using their off-diagonal coordinates, multiplied by $\sqrt2$, realizes them isometrically in $D=\binom N2$ dimensions. They are distinct because equal outer products require $u_A=\pm u_B$, and complements have size $2p$, not $k$.

Any subset of smaller [diameter](../../../topological-analysis.md#diameter) contains at most $B$ points, so a partition into smaller-[diameter](../../../topological-analysis.md#diameter) pieces needs at least $v/B=\exp(c_0N+o(N))$ pieces. For sufficiently large primes this exceeds $D+1$, disproving the [Borsuk conjecture](../../../geometry-and-topology.md#borsuk-conjecture). This is the mechanism behind the [Kahn-Kalai counterexample to the Borsuk conjecture](../../../geometry-and-topology.md#kahn-kalai-counterexample-to-the-borsuk-conjecture): the number of required pieces grows exponentially in the original set-system parameter while dimension grows quadratically. Their [1993 paper](https://arxiv.org/abs/math/9307229) establishes the resulting high-dimensional counterexample.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
