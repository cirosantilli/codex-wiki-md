# Paper 214

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_214.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_214.pdf)

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

## 1

↑ **Parent:** [Paper 214](paper-214.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $\alpha=\inf_{k\geq1}x_k/k$. The relevant version of the [Fekete lemma](../../../real-analysis.md#fekete-s-lemma) is the [extended-real Fekete lemma](../../../real-analysis.md#fekete-s-lemma): $\alpha$ may be $-\infty$, but cannot be $+\infty$ because $x_1$ is real. We show that this is exactly the [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence).

Fix $k\geq1$ and, for $n\geq k$, write $n=qk+r$, where $q\geq1$ and $0\leq r<k$. Iterating the defining inequality gives $x_{qk}\leq qx_k$. If $r>0$, it also gives $x_n\leq qx_k+x_r$; if $r=0$, there is no remainder term. Thus, with $C_k=\max(0,x_1,\ldots,x_{k-1})$ and $C_1=0$,

$$
\frac{x_n}{n}\leq\frac qn x_k+\frac{C_k}n.
$$

As $n\to\infty$, $q/n\to1/k$, so $\limsup_n x_n/n\leq x_k/k$. This holds for every positive $k$. On the other hand every $x_n/n\geq\alpha$. If $\alpha$ is finite, these two bounds give the desired equality. If $\alpha=-\infty$, for every real $M$ choose $k$ with $x_k/k<M-1$; the same upper bound makes $x_n/n<M$ for all sufficiently large $n$. Therefore

$$
\boxed{\lim_{n\to\infty}\frac{x_n}{n}=\inf_{k\geq1}\frac{x_k}{k}\in[-\infty,\infty).}
$$

The index $k=0$ is excluded because its ratio is undefined, and $x_0$ is irrelevant since the defining inequality was required only at positive indices. If the printed word “[limit of a sequence](../../../real-analysis.md#limit-of-a-sequence)” is interpreted as a finite real [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence), an additional lower bound is necessary: $x_n=-n^2$ defines a [subadditive sequence](../../../real-analysis.md#subadditive-sequence) but $x_n/n=-n\to-\infty$. The extended-real statement is the correct unrestricted conclusion.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Put $q_k(n)=\mathbb P_p((0,0)\leftrightarrow(n,0)\text{ inside }T_k)$, with $q_k(0)=1$. The connection event is increasing in the open [edges](../../../graph-theory.md#edge-of-a-graph). Apply the [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) to connection from $(0,0)$ to $(n,0)$ and connection from $(n,0)$ to $(n+m,0)$, both constrained to the strip. Their intersection implies connection between the outer endpoints, while horizontal translation invariance makes the second event's [probability](../../../probability-theory.md#probability) $q_k(m)$. Hence

$$
q_k(n+m)\geq q_k(n)q_k(m).
$$

These events may depend on infinitely many strip [edges](../../../graph-theory.md#edge-of-a-graph). To justify the inequality directly, first restrict each connecting [graph path](../../../graph-theory.md#path-in-a-graph) to a finite box, apply [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) in the finite independent [edge](../../../graph-theory.md#edge-of-a-graph) family, and then let the box grow. Every connection has a finite witness [graph path](../../../graph-theory.md#path-in-a-graph), so continuity from below gives the stated inequality.

The direct horizontal [graph path](../../../graph-theory.md#path-in-a-graph) supplies $q_k(n)\geq p^n>0$, and [probabilities](../../../probability-theory.md#probability) are at most one. Thus $a_k(n)=-\log q_k(n)$ is a finite nonnegative [subadditive sequence](../../../real-analysis.md#subadditive-sequence) with $a_k(n)\leq-n\log p$. The [Fekete lemma](../../../real-analysis.md#fekete-s-lemma) now gives a finite [connection decay rate in a percolation strip](../../../bond-percolation.md#connection-decay-rate-in-a-percolation-strip):

$$
\boxed{f_k(p)=\lim_{n\to\infty}\frac{a_k(n)}n=\inf_{n\geq1}\frac{a_k(n)}n,\qquad0\leq f_k(p)\leq-\log p.}
$$

Each individual ratio is at least its [infimum](../../../real-analysis.md#infimum), so $-\log q_k(n)\geq nf_k(p)$ and therefore

$$
\boxed{q_k(n)\leq e^{-nf_k(p)}.}
$$

At $n=0$ this reads $1\leq1$. Only nonnegative separations are intended by this notation; horizontal reflection supplies the analogous bound with $|n|$ for negative separations.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The strips are nested. Every connection permitted inside $T_k$ is also permitted inside $T_{k+1}$, so $q_k(n)\leq q_{k+1}(n)$ for every fixed separation. Consequently

$$
f_{k+1}(p)=\inf_{n\geq1}\frac{-\log q_{k+1}(n)}n\leq\inf_{n\geq1}\frac{-\log q_k(n)}n=f_k(p).
$$

The preceding nonnegative bound makes this a decreasing [sequence](../../../real-analysis.md#sequence) bounded below. By monotone convergence of real [sequences](../../../real-analysis.md#sequence),

$$
\boxed{\lim_{k\to\infty}f_k(p)=\inf_{k\geq1}f_k(p)\in[0,-\log p].}
$$

There is no assertion that this [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) is strictly positive: positivity at each fixed width need not survive an increasing-width [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence).

One can also identify the [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence). Let $q(n)$ be the [percolation two-point connection probability](../../../bond-percolation.md#percolation-two-point-connection-probability) in the whole [square lattice](../../../graph.md#square-lattice). Every finite connecting [graph path](../../../graph-theory.md#path-in-a-graph) has a bounded vertical extent, so $q_k(n)\uparrow q(n)$. Commuting infima gives the [strip approximation to the planar connection decay rate](../../../bond-percolation.md#strip-approximation-to-the-planar-connection-decay-rate):

$$
\inf_k f_k(p)=\inf_k\inf_{n\geq1}\frac{-\log q_k(n)}n=\inf_{n\geq1}\inf_k\frac{-\log q_k(n)}n=\inf_{n\geq1}\frac{-\log q(n)}n.
$$

The same positive-association argument identifies the final [infimum](../../../real-analysis.md#infimum) with the whole-plane normalized logarithmic [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence). This is an interchange of infima justified by monotonicity at fixed $n$. For example, when $p>1/2$, the threshold proved in question 2 and uniqueness give an [infinite percolation cluster](../../../bond-percolation.md#infinite-percolation-cluster) with root [probability](../../../probability-theory.md#probability) $\theta(p)>0$. The [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) makes the [probability](../../../probability-theory.md#probability) that both endpoints belong to it at least $\theta(p)^2$, so $q(n)\geq\theta(p)^2$. The whole-plane rate, and hence $\lim_k f_k(p)$, is then zero, despite the strict positivity of every finite-strip rate.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

For each integer $j$, consider the cut of horizontal [edges](../../../graph-theory.md#edge-of-a-graph) joining column $j$ to column $j+1$ inside the strip. It contains exactly $2k+1$ [edges](../../../graph-theory.md#edge-of-a-graph). Its being completely closed has [probability](../../../probability-theory.md#probability)

$$
r_k=(1-p)^{2k+1}>0.
$$

Different cuts use disjoint [edge](../../../graph-theory.md#edge-of-a-graph) sets, so these closed-cut events are independent. Any [graph path](../../../graph-theory.md#path-in-a-graph) from column zero to column $n>0$, even one that wanders to other columns first, must cross each cut with $j=0,\ldots,n-1$. None of those $n$ cuts may therefore be completely closed. This gives the [closed-cut bound for percolation in a strip](../../../bond-percolation.md#closed-cut-bound-for-percolation-in-a-strip):

$$
q_k(n)\leq(1-r_k)^n.
$$

Taking negative logarithms, dividing by $n$ and taking the established [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) yields

$$
\boxed{f_k(p)\geq-\log\bigl(1-(1-p)^{2k+1}\bigr)>0.}
$$

The strict inequality uses both finite width and $p<1$. It is consistent with $f_k(p)\leq-\log p$, since $1-(1-p)^{2k+1}\geq p$. At $p=1$ all strip connections occur and the decay rate is zero, so that excluded endpoint would invalidate strict positivity. The mechanism is a positive [probability](../../../probability-theory.md#probability) of an impermeable finite cut, rather than any assumption that the unrestricted lattice is subcritical.

## 2

↑ **Parent:** [Paper 214](paper-214.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the nearest-neighbour lattice [graph](../../../graph.md) with [graph vertex](../../../graph.md#vertex-graph-theory) set $\mathbb Z^d$: an unordered pair $\{x,y\}$ is an [edge](../../../graph-theory.md#edge-of-a-graph) precisely when $\|x-y\|_1=1$. A bond configuration is $\omega\in\{0,1\}^{E_d}$; under the [product measure](../../../probability-theory.md#product-measure) $\mathbb P_p$, its [edge](../../../graph-theory.md#edge-of-a-graph) coordinates are independent [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) with success [probability](../../../probability-theory.md#probability) $p$. [Edges](../../../graph-theory.md#edge-of-a-graph) with coordinate one are open. The open cluster $C(0)$ is the [connected component of a graph](../../../graph.md#component-graph-theory) reachable from the origin through open [edges](../../../graph-theory.md#edge-of-a-graph).

Define the [percolation probability](../../../probability-theory.md#percolation-probability) and [percolation critical probability](../../../probability-theory.md#percolation-critical-probability) by

$$
\boxed{\theta_d(p)=\mathbb P_p(|C(0)|=\infty),\qquad p_c(d)=\inf\{p\in[0,1]:\theta_d(p)>0\}.}
$$

Equivalently, $p_c(d)=\sup\{p:\theta_d(p)=0\}$. The [monotone coupling of Bernoulli percolation](../../../probability-theory.md#monotone-coupling-of-bernoulli-percolation) proves the equivalence: assign independent [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) $U_e$ to the [edges](../../../graph-theory.md#edge-of-a-graph) and open $e$ at parameter $p$ when $U_e\leq p$. Connection events and $\theta_d$ then increase with $p$. For $d\geq1$, $\theta_d(0)=0$ and $\theta_d(1)=1$, so the defining set is nonempty. The definition does not settle what happens at $p=p_c(d)$.

By translation invariance all roots have the same [probability](../../../probability-theory.md#probability). Since the [graph vertex](../../../graph.md#vertex-graph-theory) set is countable, $\theta_d(p)=0$ implies that no [graph vertex](../../../graph.md#vertex-graph-theory) lies in an [infinite percolation cluster](../../../bond-percolation.md#infinite-percolation-cluster) [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Conversely a positive root [probability](../../../probability-theory.md#probability) gives positive [probability](../../../probability-theory.md#probability) of an [infinite percolation cluster](../../../bond-percolation.md#infinite-percolation-cluster), and [translation ergodicity of Bernoulli percolation](../../../bond-percolation.md#translation-ergodicity-of-bernoulli-percolation) then makes existence an almost-sure event. In question 2(b), $\theta$ means $\theta_2$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

We use [planar duality for rectangle crossings](../../../graph-theory.md#planar-duality-for-rectangle-crossings), [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) and the permitted [exponential decay of subcritical percolation](../../../probability-theory.md#exponential-decay-of-subcritical-percolation). A critical-point detail matters: uniqueness stated only for $p>p_c$ cannot by itself be applied at $p=p_c$. We prove the [Burton-Keane theorem](../../../bond-percolation.md#uniqueness-of-the-infinite-percolation-cluster) by the [boundary counting proof of percolation uniqueness](../../../bond-percolation.md#boundary-counting-proof-of-percolation-uniqueness), establishing at most one [infinite percolation cluster](../../../bond-percolation.md#infinite-percolation-cluster) at every parameter and avoiding that gap.

For $0<p<1$, the number $N$ of [infinite percolation clusters](../../../bond-percolation.md#infinite-percolation-cluster) is [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) constant by [translation ergodicity of Bernoulli percolation](../../../bond-percolation.md#translation-ergodicity-of-bernoulli-percolation). It cannot be a finite constant greater than one. A sufficiently large box meets two different [infinite percolation clusters](../../../bond-percolation.md#infinite-percolation-cluster) with positive [probability](../../../probability-theory.md#probability); opening its finitely many interior [edges](../../../graph-theory.md#edge-of-a-graph) joins them without creating a new [infinite percolation cluster](../../../bond-percolation.md#infinite-percolation-cluster), decreasing $N$. [Finite modification of Bernoulli percolation](../../../probability-theory.md#finite-modification-of-bernoulli-percolation) gives positive [probability](../../../probability-theory.md#probability) to this modification, contradicting constancy.

Nor can $N=\infty$. A finite box then meets three different [infinite percolation clusters](../../../bond-percolation.md#infinite-percolation-cluster) with positive [probability](../../../probability-theory.md#probability). Select one infinite exterior branch from each. In the box and a finite collar retain just an embedded three-armed [tree](../../../combinatorics.md#tree-graph-theory) joining those branches and close all other incident [edges](../../../graph-theory.md#edge-of-a-graph) there. Its branching [graph vertex](../../../graph.md#vertex-graph-theory) separates three infinite components when removed, so is a [trifurcation vertex in percolation](../../../bond-percolation.md#trifurcation-vertex-in-percolation). All selections concern finitely many possible entrances and [edge](../../../graph-theory.md#edge-of-a-graph) patterns; [finite-energy property of Bernoulli percolation](../../../probability-theory.md#finite-energy-property-of-bernoulli-percolation) gives positive [probability](../../../probability-theory.md#probability) for at least one such pattern. Translation invariance then gives a common positive trifurcation [probability](../../../probability-theory.md#probability) $q$.

Here is the counting contradiction in detail. For a finite box $W$, contract each open component outside $W$ that touches $W$ to a boundary terminal. In each cluster, the resulting incidence [graph](../../../graph.md) is finite and connected. Every trifurcation in $W$ separates at least three sets of terminals, since each infinite branch must leave $W$. A minimal subtree joining all terminals must therefore contain that [graph vertex](../../../graph.md#vertex-graph-theory) with [degree of a vertex](../../../graph-theory.md#degree-graph-theory) at least three. Its leaves are terminals. The [tree](../../../combinatorics.md#tree-graph-theory) identity $\sum_v(\deg(v)-2)=-2$ bounds the number of those branching [graph vertices](../../../graph.md#vertex-graph-theory) by the terminal count. Different terminals are represented by different exterior [graph neighbours](../../../graph-theory.md#neighbour-of-a-vertex) of $W$. Thus the [trifurcation boundary-counting lemma](../../../bond-percolation.md#trifurcation-boundary-counting-lemma) gives

$$
q|W|=\mathbb E\bigl[\#\{v\in W:v\text{ trifurcates}\}\bigr]\leq|\partial^+W|.
$$

For $W=[-r,r]^2\cap\mathbb Z^2$, the two sizes are $(2r+1)^2$ and $8r+4$. Letting $r\to\infty$ contradicts $q>0$. Therefore $N\in\{0,1\}$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), with the same conclusion for the translated [planar dual graph](../../../graph-theory.md#planar-dual-graph).

Now prove absence of percolation at $p=1/2$ by [Zhang's argument](../../../probability-theory.md#alternating-arms-argument-at-the-self-dual-percolation-parameter). Suppose instead that $\theta(1/2)>0$. [Almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) an infinite primal cluster exists, and self-duality gives an infinite dual cluster as well. An infinite connected subgraph of this locally finite lattice contains a [graph ray](../../../graph-theory.md#ray-in-a-graph), by the [König infinity lemma](../../../combinatorics.md#konig-s-lemma). Expanding square boxes meet the [infinite percolation clusters](../../../bond-percolation.md#infinite-percolation-cluster) with [probability](../../../probability-theory.md#probability) tending to one.

For $B_r=[-r,r]^2\cap\mathbb Z^2$, let $A_N,A_E,A_S,A_W$ mean that an open [graph ray](../../../graph-theory.md#ray-in-a-graph) takes an outward [edge](../../../graph-theory.md#edge-of-a-graph) through the indicated side and subsequently uses [graph vertices](../../../graph.md#vertex-graph-theory) outside $B_r$. The union occurs whenever the box meets an [infinite percolation cluster](../../../bond-percolation.md#infinite-percolation-cluster): take the last exit of an infinite [graph ray](../../../graph-theory.md#ray-in-a-graph) from the finite box. Conversely an exterior arm supplies an [infinite percolation cluster](../../../bond-percolation.md#infinite-percolation-cluster) meeting its boundary. Quarter-turn symmetry makes the four [probabilities](../../../probability-theory.md#probability) equal. Their complements are [decreasing events](../../../probability-inequality.md#decreasing-event), so the [square-root trick for positively associated events](../../../probability-inequality.md#square-root-trick-for-positively-associated-events) gives

$$
\mathbb P_{1/2}(A_N)\geq1-\mathbb P_{1/2}(B_r\not\leftrightarrow\infty)^{1/4}\longrightarrow1.
$$

For the [planar dual graph](../../../graph-theory.md#planar-dual-graph) use the box with boundary coordinates $\pm(r+1/2)$ and define its exterior side-arm events in the same way. This box also has quarter-turn symmetry and meets the dual [infinite percolation cluster](../../../bond-percolation.md#infinite-percolation-cluster) with [probability](../../../probability-theory.md#probability) tending to one. Thus each dual side has an infinite exterior arm with [probability](../../../probability-theory.md#probability) tending to one. Primal outward [edges](../../../graph-theory.md#edge-of-a-graph) cross this dual-box contour on the corresponding sides; their remaining [graph vertices](../../../graph.md#vertex-graph-theory) stay outside it. A [union bound](../../../probability-inequality.md#boole-s-inequality) makes the simultaneous event of primal north/south arms and dual east/west arms have positive [probability](../../../probability-theory.md#probability) for a sufficiently large box.

The four arms alternate around the contour. Open all [edges](../../../graph-theory.md#edge-of-a-graph) with both endpoints in $B_r$, leaving all outward and exterior [edges](../../../graph-theory.md#edge-of-a-graph) intact. This joins the two primal entrance points and preserves all four exterior arms. [Finite-energy property of Bernoulli percolation](../../../probability-theory.md#finite-energy-property-of-bernoulli-percolation) keeps the event's [probability](../../../probability-theory.md#probability) positive. The primal north and south arms are now connected through the box. The two dual arms must lie in different infinite dual clusters. To see the separation, a hypothetical finite dual [graph path](../../../graph-theory.md#path-in-a-graph) joining the east and west arms cannot enter the dual-box interior: its boundary-crossing and interior [edges](../../../graph-theory.md#edge-of-a-graph) cross primal [edges](../../../graph-theory.md#edge-of-a-graph) that were just opened. Erase its loops and cut it at successive hits of the contour. A resulting exterior dual crosscut, together with the corresponding contour arc, encloses one of the two intervening primal entrance points. The infinite primal [graph ray](../../../graph-theory.md#ray-in-a-graph) from that point would have to cross a dual-open [edge](../../../graph-theory.md#edge-of-a-graph), which is impossible. This is the planar separation used in the [alternating arms argument at the self-dual percolation parameter](../../../probability-theory.md#alternating-arms-argument-at-the-self-dual-percolation-parameter). It contradicts uniqueness of the infinite dual cluster. Hence

$$
\boxed{\theta(1/2)=0,\qquad p_c(2)\geq1/2.}
$$

Finally suppose $p_c(2)>1/2$. At $p=1/2$ the permitted [exponential decay of subcritical percolation](../../../probability-theory.md#exponential-decay-of-subcritical-percolation) would supply $C,c>0$ with $\mathbb P_{1/2}(v\leftrightarrow\partial B_n(v))\leq Ce^{-cn}$. Use the rectangle with [graph vertices](../../../graph.md#vertex-graph-theory) $\{0,\ldots,n\}\times\{0,\ldots,n-1\}$, and let $H_n$ be its left-to-right open crossing. [Planar duality for rectangle crossings](../../../graph-theory.md#planar-duality-for-rectangle-crossings) identifies its complement with a dual top-to-bottom crossing of a rectangle of width $n-1$ and height $n$. Rotation and translation give the same crossing law; side [edges](../../../graph-theory.md#edge-of-a-graph) at the entrance and exit boundaries are irrelevant. Thus the [exact self-dual rectangle crossing probability](../../../graph-theory.md#exact-self-dual-rectangle-crossing-probability) is

$$
\mathbb P_{1/2}(H_n)=\frac12.
$$

But a crossing has some starting [graph vertex](../../../graph.md#vertex-graph-theory) on its $n$-vertex left side connected to distance $n$. The [union bound](../../../probability-inequality.md#boole-s-inequality) and [exponential decay of subcritical percolation](../../../probability-theory.md#exponential-decay-of-subcritical-percolation) imply $\mathbb P_{1/2}(H_n)\leq nCe^{-cn}\to0$, a contradiction. Therefore

$$
\boxed{p_c(2)=1/2\quad\text{and}\quad\theta(1/2)=0.}
$$

No Russo-Seymour-Welsh theorem or continuity assertion for $\theta$ is being used, and critical uniqueness was proved rather than inferred from the supercritical hypothesis.

## 3

↑ **Parent:** [Paper 214](paper-214.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Fix an [edge](../../../graph-theory.md#edge-of-a-graph) $e=\{u,v\}$ and orient it from $u$ to $v$. For each [spanning tree](../../../combinatorics.md#spanning-tree) $T$, let $\gamma_T$ be its unique [graph path](../../../graph-theory.md#path-in-a-graph) from $u$ to $v$. Assign a signed unit [graph path](../../../graph-theory.md#path-in-a-graph) flow $j_T$ to oriented [edges](../../../graph-theory.md#edge-of-a-graph): value $+1$ in the direction used by $\gamma_T$, value $-1$ on the reversed orientation, and zero otherwise. Define its mean

$$
J(x,y)=\mathbb E\,j_T(x,y).
$$

Each $j_T$ has net divergence one at $u$, minus one at $v$ and zero elsewhere, so $J$ is a [unit flow](../../../graph-theory.md#unit-flow). The [mean spanning-tree path current](../../../combinatorics.md#mean-spanning-tree-path-current) also satisfies the [Kirchhoff cycle law](../../../markov-process.md#kirchhoff-cycle-law). Although its verification is permitted to be omitted, a short counting argument makes it explicit. Let $\mathcal F_{uv}$ be the [two-component spanning forests](../../../combinatorics.md#two-component-spanning-forest) separating $u$ and $v$, write $A_F$ for the component containing $u$, and let $N_T$ be the number of [spanning trees](../../../combinatorics.md#spanning-tree). Deleting an [edge](../../../graph-theory.md#edge-of-a-graph) used by the oriented [tree](../../../combinatorics.md#tree-graph-theory) [graph path](../../../graph-theory.md#path-in-a-graph) gives one such forest. Conversely adjoining an [edge](../../../graph-theory.md#edge-of-a-graph) across its two components gives a unique [tree](../../../combinatorics.md#tree-graph-theory) with that [edge](../../../graph-theory.md#edge-of-a-graph) on its $u$-to-$v$ [graph path](../../../graph-theory.md#path-in-a-graph). Consequently

$$
J(x,y)=\frac1{N_T}\sum_{F\in\mathcal F_{uv}}\bigl(\mathbf1_{A_F}(x)-\mathbf1_{A_F}(y)\bigr)=h(x)-h(y),\qquad h(x)=\frac1{N_T}\sum_{F\in\mathcal F_{uv}}\mathbf1_{A_F}(x).
$$

The gradient form proves the [Kirchhoff cycle law](../../../markov-process.md#kirchhoff-cycle-law) directly and is [Ohm's law](../../../electromagnetism.md#ohm-s-law) for unit [edge](../../../graph-theory.md#edge-of-a-graph) resistance. The [Kirchhoff node law](../../../markov-process.md#kirchhoff-node-law) then gives $Lh=\delta_u-\delta_v$, and the electrical [unit flow](../../../graph-theory.md#unit-flow) is unique: the difference between two such [voltages](../../../markov-process.md#voltage) is a [harmonic function on a graph](../../../partial-differential-equation.md#discrete-harmonic-function) and hence constant on the connected finite [graph](../../../graph.md).

If $e\in T$, its single-edge route is the unique [tree](../../../combinatorics.md#tree-graph-theory) [graph path](../../../graph-theory.md#path-in-a-graph) from $u$ to $v$, so $j_T(u,v)=1$. If $e\notin T$, that [tree](../../../combinatorics.md#tree-graph-theory) [graph path](../../../graph-theory.md#path-in-a-graph) does not use $e$, so $j_T(u,v)=0$. Therefore

$$
J(u,v)=\mathbb P(e\in T).
$$

By [Ohm's law](../../../electromagnetism.md#ohm-s-law), $J(u,v)=h(u)-h(v)$; for a unit terminal current, this [voltage](../../../markov-process.md#voltage) difference is exactly the [effective resistance](../../../markov-process.md#effective-resistance) between the terminals. We have proved the requested [edge-inclusion formula for a uniform spanning tree](../../../combinatorics.md#edge-inclusion-formula-for-a-uniform-spanning-tree):

$$
\boxed{\mathbb P(e\in T)=R_{\mathrm{eff}}(u,v).}
$$

Now use [linearity of expectation](../../../probability-theory.md#linearity-of-expectation) and the fact that every [spanning tree](../../../combinatorics.md#spanning-tree) has exactly $n-1$ [edges](../../../graph-theory.md#edge-of-a-graph). This gives [Foster's theorem](../../../markov-process.md#foster-s-theorem):

$$
\boxed{\sum_{e\in E}R_{\mathrm{eff}}(e)=\sum_{e\in E}\mathbb P(e\in T)=\mathbb E|T|=n-1.}
$$

The sums here use unoriented [edges](../../../graph-theory.md#edge-of-a-graph) exactly once. For unit conductance this is the displayed identity; with conductances $c_e$ the inclusion [probability](../../../probability-theory.md#probability) and summand become $c_eR_{\mathrm{eff}}(e)$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use [simple random walk](../../../markov-process.md#simple-random-walk) on the loopless undirected unweighted [graph](../../../graph.md), with transition [probability](../../../probability-theory.md#probability) $1/\deg(x)$ to each [graph neighbour](../../../graph-theory.md#neighbour-of-a-vertex), and take $a\ne z$. Set $T_z=\inf\{t\geq0:X_t=z\}$. Returns to $a$ before visiting $z$ do not end the commute. After its first visit to $z$, stop at the subsequent first visit to $a$, so $\tau=T_z+T_a\circ\vartheta_{T_z}$. Count transitions with departure times $0\leq t<\tau$, including the final step arriving at $a$. The [expected hitting times](../../../markov-process.md#expected-hitting-time) are finite: in a finite [connected graph](../../../graph.md#connected-graph) there is a uniformly positive [probability](../../../probability-theory.md#probability) to reach any fixed target within a fixed number of steps, giving a geometric tail bound.

We prove the needed [killed-walk occupation voltage](../../../markov-process.md#killed-walk-occupation-voltage) identity from its visit balance equation. Define

$$
g_{az}(x)=\mathbb E_a\sum_{t=0}^{T_z-1}\mathbf1_{\{X_t=x\}},\qquad v(x)=\frac{g_{az}(x)}{\deg(x)},\qquad v(z)=0.
$$

For $x\ne z$, counting arrivals before absorption gives

$$
g_{az}(x)=\mathbf1_{\{x=a\}}+\sum_{y\sim x}\frac{g_{az}(y)}{\deg(y)}.
$$

Hence, for the [Graph Laplacian](../../../graph-theory.md#laplacian-matrix) $Lv(x)=\deg(x)v(x)-\sum_{y\sim x}v(y)$, we have $Lv(x)=\mathbf1_{\{x=a\}}$ away from $z$. Since the sum of all Laplacian coordinates is zero, $Lv(z)=-1$. Thus $v$ is the electrical [voltage](../../../markov-process.md#voltage) of a [unit flow](../../../graph-theory.md#unit-flow) from $a$ to $z$, grounded at $z$, and $v(a)=R_{\mathrm{eff}}(a,z)$.

Construct $w(x)=g_{za}(x)/\deg(x)$ for the opposite killed leg. It satisfies $Lw=\delta_z-\delta_a$ and $w(a)=0$. Therefore $L(v+w)=0$. The [harmonic maximum principle on a finite graph](../../../partial-differential-equation.md#harmonic-maximum-principle-on-a-finite-graph) makes $v+w$ constant: at a maximum its value equals the average over its [graph neighbours](../../../graph-theory.md#neighbour-of-a-vertex), forcing all of them to share that value, and connectedness propagates it. At $a$ the constant equals $R_{\mathrm{eff}}(a,z)$.

For any oriented [edge](../../../graph-theory.md#edge-of-a-graph) $(x,y)$, each visit to $x$ before the target hit produces a transition to $y$ with conditional [probability](../../../probability-theory.md#probability) $1/\deg(x)$. The expected traversals during the first killed leg are therefore $v(x)$, and those during the second leg are $w(x)$ by the [Strong Markov property](../../../markov-process.md#strong-markov-property) at $T_z$. This proves [directed edge occupation in a random-walk commute](../../../markov-process.md#directed-edge-occupation-in-a-random-walk-commute):

$$
\boxed{\mathbb E_a S(x,y)=v(x)+w(x)=R_{\mathrm{eff}}(a,z).}
$$

In particular, both directions of every unoriented [edge](../../../graph-theory.md#edge-of-a-graph) have this same [expected value](../../../probability-theory.md#expected-value), although their counts on an individual commute need not coincide. Summing over the $2|E|$ directed [edges](../../../graph-theory.md#edge-of-a-graph) also recovers the [commute time identity](../../../markov-process.md#commute-time-identity) $\mathbb E_a\tau=2|E|R_{\mathrm{eff}}(a,z)$.

The distinct-terminal convention is necessary for the printed “returns” interpretation. If $a=z$ and $\tau$ is the first positive return, a [graph](../../../graph.md) with two [graph vertices](../../../graph.md#vertex-graph-theory) and one [edge](../../../graph-theory.md#edge-of-a-graph) gives $S(a,y)=1$ while $R_{\mathrm{eff}}(a,a)=0$. Thus either take $a\ne z$, as intended, or explicitly define the degenerate commute as $\tau=0$. A general nonuniform [random walk](../../../markov-process.md#random-walk) is not covered by the unweighted simple-walk formula.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Group the random resistance cost by unoriented [edges](../../../graph-theory.md#edge-of-a-graph). For $e=\{x,y\}$, its resistance contributes once whenever the walk traverses it in either direction. Pathwise,

$$
\sum_{t=0}^{\tau-1}R_{\mathrm{eff}}(X_t,X_{t+1})=\sum_{\{x,y\}\in E}R_{\mathrm{eff}}(x,y)\bigl(S(x,y)+S(y,x)\bigr).
$$

The [graph](../../../graph.md) is finite and the commute has finite [expected value](../../../probability-theory.md#expected-value). [Linearity of expectation](../../../probability-theory.md#linearity-of-expectation), or [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) for these nonnegative terms, therefore permits taking expectations of the sum. By the [directed edge occupation in a random-walk commute](../../../markov-process.md#directed-edge-occupation-in-a-random-walk-commute), both directed traversal counts have [expected value](../../../probability-theory.md#expected-value) $R_{\mathrm{eff}}(a,z)$. Thus

$$
\mathbb E_a\sum_{t=0}^{\tau-1}R_{\mathrm{eff}}(X_t,X_{t+1})=2R_{\mathrm{eff}}(a,z)\sum_{e\in E}R_{\mathrm{eff}}(e).
$$

Apply [Foster's theorem](../../../markov-process.md#foster-s-theorem) from part (a) to obtain

$$
\boxed{\mathbb E_a\sum_{t=0}^{\tau-1}R_{\mathrm{eff}}(X_t,X_{t+1})=2(n-1)R_{\mathrm{eff}}(a,z).}
$$

The factor two counts the two orientations of each [edge](../../../graph-theory.md#edge-of-a-graph). It would be lost by treating the expected directed count in part (b) as an expected count for both directions together. The same distinct-terminal and simple-random-walk conventions from part (b) remain in force.

## 4

↑ **Parent:** [Paper 214](paper-214.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $\mathcal T(G)$ be the [finite set](../../../set.md#finite-set) of [spanning trees](../../../combinatorics.md#spanning-tree) of the [connected graph](../../../graph.md#connected-graph). A [spanning tree](../../../combinatorics.md#spanning-tree) has all the [graph vertices](../../../graph.md#vertex-graph-theory), is connected, and contains no [graph cycle](../../../graph-theory.md#cycle-in-a-graph). Connectedness ensures that at least one exists, for example by repeatedly deleting an [edge](../../../graph-theory.md#edge-of-a-graph) of a [graph cycle](../../../graph-theory.md#cycle-in-a-graph) while retaining connectedness. The [uniform spanning tree](../../../combinatorics.md#uniform-spanning-tree) is the random [edge](../../../graph-theory.md#edge-of-a-graph) set $T$ with

$$
\boxed{\mathbb P(T=t)=\frac1{|\mathcal T(G)|}\quad\text{for each }t\in\mathcal T(G).}
$$

Every [tree](../../../combinatorics.md#tree-graph-theory) has $|V|-1$ [edges](../../../graph-theory.md#edge-of-a-graph), so uniformity is over complete [trees](../../../combinatorics.md#tree-graph-theory), not over arbitrary subsets of that size. Such subsets can be disconnected or cyclic and do not belong to $\mathcal T(G)$. Nor are indicators of the [tree](../../../combinatorics.md#tree-graph-theory) [edges](../../../graph-theory.md#edge-of-a-graph) generally independent. The [matrix-tree theorem](../../../combinatorics.md#kirchhoff-s-theorem) gives $|\mathcal T(G)|$ as any cofactor of the unweighted [Graph Laplacian](../../../graph-theory.md#laplacian-matrix) if a numerical normalizing constant is needed.

This definition uses the ordinary undirected unweighted [graph](../../../graph.md) convention. With positive conductances the analogous law for [spanning trees](../../../combinatorics.md#spanning-tree) weights $t$ proportionally to $\prod_{e\in t}c_e$ and is generally not uniform. When the [graph](../../../graph.md) has one [graph vertex](../../../graph.md#vertex-graph-theory) the empty [edge](../../../graph-theory.md#edge-of-a-graph) set is the unique [spanning tree](../../../combinatorics.md#spanning-tree), so its [probability](../../../probability-theory.md#probability) is one.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For finite $G$, choose a root $r$ and an ordering of the other [graph vertices](../../../graph.md#vertex-graph-theory). Begin with a [tree](../../../combinatorics.md#tree-graph-theory) consisting only of $r$. At each stage take the first [graph vertex](../../../graph.md#vertex-graph-theory) not already in the [tree](../../../combinatorics.md#tree-graph-theory), run an independent [simple random walk](../../../markov-process.md#simple-random-walk) from it until its first hit of the existing [tree](../../../combinatorics.md#tree-graph-theory), erase the loops chronologically, and add the resulting [graph path](../../../graph-theory.md#path-in-a-graph). In chronological [loop erasure](../../../markov-process.md#loop-erasure), revisiting a [graph vertex](../../../graph.md#vertex-graph-theory) already in the current list deletes all list entries after that [graph vertex](../../../graph.md#vertex-graph-theory); otherwise append the new [graph vertex](../../../graph.md#vertex-graph-theory). The retained final [graph path](../../../graph-theory.md#path-in-a-graph) is simple, with new internal [graph vertices](../../../graph.md#vertex-graph-theory) and exactly one endpoint in the old [tree](../../../combinatorics.md#tree-graph-theory). Adding it therefore preserves connectedness and creates no [graph cycle](../../../graph-theory.md#cycle-in-a-graph). [Graph vertices](../../../graph.md#vertex-graph-theory) already included are skipped. On a finite [connected graph](../../../graph.md#connected-graph) each walk hits the existing [tree](../../../combinatorics.md#tree-graph-theory) [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence); after finitely many attachments all [graph vertices](../../../graph.md#vertex-graph-theory) are present.

The [Wilson algorithm](../../../combinatorics.md#wilson-s-algorithm) theorem states that this [tree](../../../combinatorics.md#tree-graph-theory) is a [uniform spanning tree](../../../combinatorics.md#uniform-spanning-tree), independently of the chosen root and order. The required hypotheses here are an undirected connected finite [graph](../../../graph.md) and transition [probabilities](../../../probability-theory.md#probability) proportional to conductance; unit conductances give [simple random walk](../../../markov-process.md#simple-random-walk) and the uniform law. This is the sampling result being described, not a claim that arbitrary walk transition [probabilities](../../../probability-theory.md#probability) would produce a uniform [tree](../../../combinatorics.md#tree-graph-theory).

For an infinite connected locally finite [recurrent graph](../../../markov-process.md#recurrent-graph), choose a fixed finite root $r$ and enumerate all [graph vertices](../../../graph.md#vertex-graph-theory). A connected [locally finite graph](../../../graph-theory.md#locally-finite-graph) is countable, since its finite-radius balls are finite. Run the same algorithm successively. Recurrence and irreducibility imply that a walk from any [graph vertex](../../../graph.md#vertex-graph-theory) hits $r$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), hence hits the current [tree](../../../combinatorics.md#tree-graph-theory). Every attached [graph path](../../../graph-theory.md#path-in-a-graph) is therefore finite. The countable intersection of these probability-one events has [probability](../../../probability-theory.md#probability) one, and the increasing union is an acyclic connected subgraph containing all [graph vertices](../../../graph.md#vertex-graph-theory): each [graph vertex](../../../graph.md#vertex-graph-theory) receives a finite route to $r$.

This gives the [uniform spanning tree of a recurrent infinite graph](../../../combinatorics.md#uniform-spanning-tree-of-a-recurrent-infinite-graph). It is not a uniform counting measure on all infinite [spanning trees](../../../combinatorics.md#spanning-tree). Equivalently, its joint [probability distributions](../../../probability-theory.md#probability-distribution) on finite collections of [edges](../../../graph-theory.md#edge-of-a-graph) are the common limits of [uniform spanning trees](../../../combinatorics.md#uniform-spanning-tree) along any [graph exhaustion](../../../graph-theory.md#graph-exhaustion), using the approximations defining the [free uniform spanning forest](../../../combinatorics.md#free-uniform-spanning-forest) and the [wired uniform spanning forest](../../../combinatorics.md#wired-uniform-spanning-forest). To check that equivalence, fix a finite [edge](../../../graph-theory.md#edge-of-a-graph) set $F$ and run the chosen enumeration through a finite prefix containing all its endpoints. Once those [graph vertices](../../../graph.md#vertex-graph-theory) are in the [tree](../../../combinatorics.md#tree-graph-theory), later attachments cannot add an [edge](../../../graph-theory.md#edge-of-a-graph) with both endpoints already included, so membership of $F$ is settled permanently. Only finitely many random walks have been used; each has a finite trajectory [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). All their visited [graph vertices](../../../graph.md#vertex-graph-theory) and all their [graph neighbours](../../../graph-theory.md#neighbour-of-a-vertex) lie in a sufficiently large exhaustion set. Couple finite-volume and infinite-volume walks with the same steps there. Whether the exterior is deleted or wired to one boundary [graph vertex](../../../graph.md#vertex-graph-theory), these initial trajectories and their loop erasures then agree. This proves convergence of the [probabilities](../../../probability-theory.md#probability) of [cylinder sets](../../../geometry-and-topology.md#cylinder-set) determined by those [edges](../../../graph-theory.md#edge-of-a-graph).

The limiting law is unchanged by the root and ordering because the laws on finite [graphs](../../../graph.md) have this invariance. The same coupling shows that changing the exhaustion also leaves the law unchanged. Thus

$$
\boxed{\text{recurrent }G:\quad\text{fixed-root Wilson tree}=\text{free limit}=\text{wired limit}.}
$$

The result is a single [spanning tree](../../../combinatorics.md#spanning-tree) because the [graph](../../../graph.md) is recurrent. On a [transient graph](../../../markov-process.md#transient-graph), infinite-volume spanning-tree limits may instead be [uniform spanning forests](../../../combinatorics.md#uniform-spanning-forest); recurrence cannot be omitted from this conclusion.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

First take $x\ne y$. Sample a [uniform spanning tree](../../../combinatorics.md#uniform-spanning-tree) using [Wilson's algorithm](../../../combinatorics.md#wilson-s-algorithm) rooted at $y$, with $x$ processed first. The first walk runs from $x$ until its first hit of $y$, so its [loop erasure](../../../markov-process.md#loop-erasure) is exactly the unique $x$-to-$y$ [graph path](../../../graph-theory.md#path-in-a-graph) of the resulting [tree](../../../combinatorics.md#tree-graph-theory). Later attachments cannot alter that [graph path](../../../graph-theory.md#path-in-a-graph). This is the [uniform-spanning-tree path representation of loop-erased random walk](../../../markov-process.md#uniform-spanning-tree-path-representation-of-loop-erased-random-walk).

Instead root [Wilson's algorithm](../../../combinatorics.md#wilson-s-algorithm) at $x$ and process $y$ first. The resulting [tree](../../../combinatorics.md#tree-graph-theory) still has the same uniform law, while its first attachment has the law of [loop-erased random walk](../../../markov-process.md#loop-erased-random-walk) from $y$ to $x$. A [tree](../../../combinatorics.md#tree-graph-theory)'s [graph path](../../../graph-theory.md#path-in-a-graph) between two fixed [graph vertices](../../../graph.md#vertex-graph-theory) has the same unoriented [edge](../../../graph-theory.md#edge-of-a-graph) set in both directions. Pushing the common [tree](../../../combinatorics.md#tree-graph-theory) law through this [graph path](../../../graph-theory.md#path-in-a-graph) map therefore gives

$$
\boxed{\mathcal E(\operatorname{LERW}_{x\to y})\overset d=\mathcal E(\operatorname{LERW}_{y\to x}).}
$$

Here $\mathcal E$ means the set of unoriented [edges](../../../graph-theory.md#edge-of-a-graph). In fact, reversing the complete [graph vertex](../../../graph.md#vertex-graph-theory) [sequence](../../../real-analysis.md#sequence) from the first loop-erased walk has the law of the second, giving [reversibility of loop-erased random walk](../../../markov-process.md#reversibility-of-loop-erased-random-walk). If $x=y$ and first hitting allows time zero, both [graph paths](../../../graph-theory.md#path-in-a-graph) are empty and the equality is immediate.

This is a distributional assertion, not a pathwise identity between chronological [loop erasure](../../../markov-process.md#loop-erasure) and reversal. For example, the valid walk trajectory $x,a,b,a,c,b,y$ in a [graph](../../../graph.md) containing the triangle on $a,b,c$ and the [edges](../../../graph-theory.md#edge-of-a-graph) $x a,b y$ erases forward to $x,a,c,b,y$. Erasing the reversed trajectory and then reversing the result gives $x,a,b,y$, a different [graph path](../../../graph-theory.md#path-in-a-graph). Wilson's root-independent [tree](../../../combinatorics.md#tree-graph-theory) law is what proves the stated equality of [probability distributions](../../../probability-theory.md#probability-distribution).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
