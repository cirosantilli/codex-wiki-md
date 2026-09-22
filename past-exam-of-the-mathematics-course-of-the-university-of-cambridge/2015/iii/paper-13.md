# Paper 13

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_13.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_13.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The [Lusternik-Schnirelmann-Borsuk theorem](../../../algebraic-topology.md#lusternik-schnirelmann-theorem) has the following two equivalent covering formulations. For every integer $d\geq0$, a cover of the [sphere](../../../geometry-and-topology.md#sphere) $S^d$ by $d+1$ [closed sets](../../../topology.md#closed-set) has a member containing an [antipodal pair](../../../geometry-and-topology.md#antipodal-pair). The same assertion holds with [open sets](../../../topology.md#open-set) in place of [closed sets](../../../topology.md#closed-set). Thus **$d+1$ antipodal-pair-free open sets, or $d+1$ antipodal-pair-free closed sets, cannot cover $S^d$.** The dimension-zero case simply says that one set covering the two-point [sphere](../../../geometry-and-topology.md#sphere) contains both points.

Here is why the two versions agree. A finite [open cover](../../../topology.md#open-cover) of a [compact metric space](../../../topological-analysis.md#compact-metric-space) admits a [closed](../../../topology.md#closed-set) shrinking that still covers: sufficiently small [closed balls](../../../topological-analysis.md#closed-ball) subordinate to the [open cover](../../../topology.md#open-cover) can be grouped according to their containing open member. Applying the closed version to that shrinking proves the open version. Conversely, if a nonempty [closed](../../../topology.md#closed-set) subset $C$ of $S^d$ avoids [antipodal pairs](../../../geometry-and-topology.md#antipodal-pair), [compactness](../../../topology.md#compact-space) gives positive distance between $C$ and $-C$. A sufficiently small open neighbourhood of $C$ still avoids [antipodal pairs](../../../geometry-and-topology.md#antipodal-pair). Enlarge each member of a hypothetical closed counterexample in this way; the open version rules it out. Empty members cause no difficulty.

Another common equivalent formulation is the [Borsuk-Ulam theorem](../../../algebraic-topology.md#borsuk-ulam-theorem): every [continuous](../../../calculus.md#continuous-function) $f:S^d\to\mathbb R^d$ has $f(x)=f(-x)$ for some $x$, or, equivalently, every [continuous](../../../calculus.md#continuous-function) [odd function](../../../calculus.md#odd-function) $g:S^d\to\mathbb R^d$ has a zero. For example, if $d+1$ antipodal-pair-free [open sets](../../../topology.md#open-set) covered $S^d$, a subordinate [partition of unity](../../../differential-geometry.md#partition-of-unity) $(\phi_1,\ldots,\phi_{d+1})$ would give the [odd function](../../../calculus.md#odd-function)

$$
g(x)=(\phi_i(x)-\phi_i(-x))_{i=1}^{d+1}
\in\{y\in\mathbb R^{d+1}:\textstyle\sum_i y_i=0\}\cong\mathbb R^d.
$$

It cannot vanish, since some $\phi_i(x)>0$, whereas antipodal-pair-freeness forces $\phi_i(-x)=0$. In the other direction, if an [odd function](../../../calculus.md#odd-function) $g:S^d\to\mathbb R^d$ never vanishes, choose $d+1$ vectors $u_i$ forming a [regular simplex](../../../algebraic-topology.md#regular-simplex) centred at the origin in $\mathbb R^d$. For $d\geq1$, the [open sets](../../../topology.md#open-set) $\{x:u_i\cdot g(x)>0\}$ cover $S^d$ and none contains an [antipodal pair](../../../geometry-and-topology.md#antipodal-pair), contradicting the covering theorem.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [Kneser graph](../../../graph-theory.md#kneser-graph) $KG(n,k)$ has the $k$-element subsets of $[n]$ as its [vertices](../../../graph.md#vertex-graph-theory); two [vertices](../../../graph.md#vertex-graph-theory) are adjacent exactly when the corresponding subsets are disjoint. The [Lovász theorem on Kneser graphs](../../../graph-theory.md#lovasz-theorem-on-kneser-graphs) determines its [chromatic number](../../../graph-theory.md#chromatic-number). A [graph colouring](../../../graph-theory.md#graph-coloring) is therefore a partition of the $k$-sets into [intersecting families](../../../extremal-set-theory.md#intersecting-family).

First construct a [graph colouring](../../../graph-theory.md#graph-coloring) with $d+2=n-2k+2$ colours. If a $k$-set meets $[d+1]$, give it the colour of its least element. Give every remaining $k$-set colour $d+2$. Two sets with one of the first $d+1$ colours share that colour's element. The last colour consists of $k$-sets in a $(2k-1)$-element ground set, so it too is an [intersecting family](../../../extremal-set-theory.md#intersecting-family). Thus $\chi(KG(n,k))\leq d+2$.

For the converse we establish the [Gale hemisphere lemma](../../../geometry-and-topology.md#gale-hemisphere-lemma) explicitly, using a signed [moment curve](../../../fourier-analysis.md#moment-curve). Choose $t_1<\cdots<t_n$ and put

$$
w_i=(-1)^i(1,t_i,\ldots,t_i^d),\qquad v_i=w_i/\|w_i\|\in S^d.
$$

Every [open hemisphere](../../../geometry-and-topology.md#open-hemisphere) $\{v:x\cdot v>0\}$ contains at least $k$ labelled points $v_i$. To see this, put $p(t)=x_0+x_1t+\cdots+x_dt^d$. It is a nonzero [polynomial](../../../polynomial.md) of [polynomial degree](../../../polynomial.md#degree-of-a-polynomial) at most $d$. First suppose none of the $p(t_i)$ vanishes. Write $b_i=\operatorname{sgn}((-1)^ip(t_i))$. If only $P\leq k-1$ of the $b_i$ were positive, the $N=n-P$ negative signs would occupy at most $P+1$ consecutive blocks. There would be at least

$$
N-(P+1)=n-2P-1\geq d+1
$$

adjacent pairs with both $b_i,b_{i+1}$ negative. Each such pair forces $p(t_i)$ and $p(t_{i+1})$ to have opposite signs. The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) would give $d+1$ distinct [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial), a contradiction.

If $p$ vanishes at $z$ of the sample points, then $z\leq d$. A [Lagrange interpolation polynomial](../../../numerical-analysis.md#lagrange-polynomial) $q$ of [polynomial degree](../../../polynomial.md#degree-of-a-polynomial) at most $z-1$ can be chosen with $(-1)^iq(t_i)<0$ at all those points. For sufficiently small $\varepsilon>0$, the [polynomial](../../../polynomial.md) $p+\varepsilon q$ keeps every previously nonzero sign, has no zero sample values, and makes every previously zero value negative after multiplication by $(-1)^i$. Its positive count is exactly the positive count of $p$, so the preceding argument proves the [open hemisphere](../../../geometry-and-topology.md#open-hemisphere) assertion also in this case. For $d=0$, the labelled points alternate between the two points of $S^0$; distinct labels, rather than distinct positions, are what is needed.

Suppose now that $KG(n,k)$ had a [graph colouring](../../../graph-theory.md#graph-coloring) with at most $d+1$ colours, padding the palette with unused colours if necessary. For each colour $j$, let

$$
U_j=\bigcup_{\substack{A\subseteq[n],\ |A|=k\\A\text{ has colour }j}}
\{x\in S^d:x\cdot v_i>0\text{ for every }i\in A\}.
$$

These are [open sets](../../../topology.md#open-set), and the [Gale hemisphere lemma](../../../geometry-and-topology.md#gale-hemisphere-lemma) says that they cover $S^d$. If both $x$ and $-x$ belonged to $U_j$, two $k$-sets of colour $j$ would lie in opposite [open hemispheres](../../../geometry-and-topology.md#open-hemisphere). They would be disjoint, hence adjacent in the [Kneser graph](../../../graph-theory.md#kneser-graph), contradicting the [graph colouring](../../../graph-theory.md#graph-coloring). The [Lusternik-Schnirelmann-Borsuk theorem](../../../algebraic-topology.md#lusternik-schnirelmann-theorem) excludes this cover. Therefore **the lower bound matches the explicit colouring**:

$$
\boxed{\chi(KG(n,k))=d+2=n-2k+2.}
$$

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Use the identification of two-element subsets of $[n]$ with the [edges](../../../graph-theory.md#edge-of-a-graph) of the [complete graph](../../../graph-theory.md#complete-graph) $K_n$. A colour class in the [Kneser graph](../../../graph-theory.md#kneser-graph) $KG(n,2)$ is an [intersecting two-element set family](../../../extremal-set-theory.md#intersecting-two-element-set-family), so its [edges](../../../graph-theory.md#edge-of-a-graph) must pairwise meet.

Such a class is contained either in a [star graph](../../../graph-theory.md#star-graph-theory) or in a [triangle in a graph](../../../graph.md#triangle-in-a-graph). Indeed, if not all [edges](../../../graph-theory.md#edge-of-a-graph) have a common [vertex](../../../graph.md#vertex-graph-theory), take two meeting [edges](../../../graph-theory.md#edge-of-a-graph) $ab,ac$. An [edge](../../../graph-theory.md#edge-of-a-graph) not containing $a$ must then be $bc$. Any further [edge](../../../graph-theory.md#edge-of-a-graph) meeting all three of $ab,ac,bc$ is one of these three. Classes with at most two [edges](../../../graph-theory.md#edge-of-a-graph) already lie in a [star graph](../../../graph-theory.md#star-graph-theory).

Assume that a [graph colouring](../../../graph-theory.md#graph-coloring) used $c\leq n-3$ colours. Classify $s$ classes as stars and the remaining $t=c-s$ classes as triangles. Delete a chosen centre of each star class, leaving $m\geq n-s\geq t+3$ [vertices](../../../graph.md#vertex-graph-theory). Every [edge](../../../graph-theory.md#edge-of-a-graph) between those remaining [vertices](../../../graph.md#vertex-graph-theory) must belong to a triangle class, of which each covers at most three [edges](../../../graph-theory.md#edge-of-a-graph). Hence

$$
\binom m2\leq3t.
$$

But

$$
\binom{t+3}{2}-3t=\frac{t^2-t+6}{2}>0,
$$

a contradiction. Thus $\chi(KG(n,2))\geq n-2$. For the matching upper bound, assign a two-set the colour of its smaller element if that element is at most $n-3$, and otherwise give it colour $n-2$. The last class comprises the three pairs on the last three elements, an [intersecting family](../../../extremal-set-theory.md#intersecting-family). Consequently **an entirely combinatorial argument gives**

$$
\boxed{\chi(KG(n,2))=n-2\quad(n\geq4).}
$$

## 2

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Take [information entropy](../../../information-theory.md#information-entropy) in bits and put $H(X_\varnothing)=0$. Write $C=A\cap B$, $U=A\setminus B$, and $V=B\setminus A$. The [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy) gives

$$
\begin{aligned}
H(X_A)+H(X_B)-H(X_{A\cup B})-H(X_{A\cap B})
&=H(X_U\mid X_C)+H(X_V\mid X_C)-H(X_U,X_V\mid X_C)\\
&=H(X_U\mid X_C)-H(X_U\mid X_C,X_V)\\
&=I(X_U;X_V\mid X_C)\geq0.
\end{aligned}
$$

The last line uses nonnegativity of [conditional mutual information](../../../information-theory.md#conditional-mutual-information), equivalently the conditional version of [conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy). All [random variables](../../../random-variable.md) are finite-valued, so every [conditional entropy](../../../information-theory.md#conditional-entropy) here is finite. Therefore **the entropy [set function](../../../function.md#set-function) is a [submodular set function](../../../function.md#submodular-set-function)**:

$$
\boxed{H(X_A)+H(X_B)\geq H(X_{A\cup B})+H(X_{A\cap B}).}
$$

This is [entropy submodularity](../../../information-theory.md#entropy-submodularity), with equality precisely when $X_U$ and $X_V$ satisfy [conditional independence](../../../random-variable.md#conditional-independence) given $X_C$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

An elementary [union-intersection compression](../../../extremal-set-theory.md#union-intersection-compression) replaces two occurrences $A_1,A_2$ in a [multiset](../../../set.md#multiset) by $A_1\cup A_2,A_1\cap A_2$. By [entropy submodularity](../../../information-theory.md#entropy-submodularity), this changes the sum of [information entropies](../../../information-theory.md#information-entropy) by

$$
H(X_{A_1\cup A_2})+H(X_{A_1\cap A_2})-H(X_{A_1})-H(X_{A_2})\leq0.
$$

A [compression of an entropy sum](../../../information-theory.md#compression-of-an-entropy-sum) is obtained by iterating these elementary [union-intersection compressions](../../../extremal-set-theory.md#union-intersection-compression). Summing the inequalities over the sequence, with repetitions counted according to their [multiset](../../../set.md#multiset) multiplicities, proves **the required monotonicity**:

$$
\boxed{\sum_{A\in\mathcal A}H(X_A)\geq\sum_{B\in\mathcal B}H(X_B).}
$$

Neither the number of occurrences of an individual coordinate nor the total number of sets changes under [union-intersection compression](../../../extremal-set-theory.md#union-intersection-compression).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The empty family satisfies the bound, so assume $\mathcal F$ is nonempty and choose a [graph](../../../graph.md) according to the [uniform distribution on a finite set](../../../discrete-probability-distribution.md#discrete-uniform-distribution) $F\in\mathcal F$. Let $Y$ be its [random vector](../../../random-variable.md#random-vector) of [edge](../../../graph-theory.md#edge-of-a-graph) indicators, indexed by $E=\binom{[n]}2$. Then its [information entropy](../../../information-theory.md#information-entropy) is $H(Y)=\log_2|\mathcal F|$.

For each [vertex](../../../graph.md#vertex-graph-theory) $v$, put $S_v=\{e\in E:v\in e\}$, so $Y_{S_v}$ records the [graph neighbourhood](../../../graph-theory.md#graph-neighbourhood) of $v$. The possible [graph neighbourhoods](../../../graph-theory.md#graph-neighbourhood) form an [intersecting family](../../../extremal-set-theory.md#intersecting-family) of subsets of $[n]\setminus\{v\}$: the [graph intersection](../../../graph-theory.md#graph-intersection) of any two members of $\mathcal F$ has no [isolated vertex](../../../graph-theory.md#isolated-vertex) at $v$. A subset and its complement cannot both occur. Pairing the $2^{n-1}$ subsets into complementary pairs gives at most $2^{n-2}$ possible [graph neighbourhoods](../../../graph-theory.md#graph-neighbourhood). The [maximum entropy on a finite alphabet](../../../information-theory.md#maximum-entropy-on-a-finite-alphabet) therefore gives

$$
H(Y_{S_v})\leq n-2.
$$

This argument applies for $n\geq2$. For $n=1$ the assumed nonempty family cannot exist, since its only possible [graph](../../../graph.md) has an [isolated vertex](../../../graph-theory.md#isolated-vertex).

Each [edge](../../../graph-theory.md#edge-of-a-graph) belongs to exactly two of the sets $S_v$. To obtain the needed instance of [Shearer inequality](../../../information-theory.md#shearer-s-inequality) directly from the preceding compression argument, repeatedly apply a [union-intersection compression](../../../extremal-set-theory.md#union-intersection-compression) to incomparable members of the [multiset](../../../set.md#multiset) $(S_v)_{v=1}^n$. Each such step strictly increases $\sum_S|S|^2$, by

$$
2|A\setminus B|\,|B\setminus A|>0.
$$

The potential is bounded and integer-valued, so the process terminates in a chain under inclusion. Coordinate multiplicities stay equal to two, so, for $E\ne\varnothing$, the terminal chain consists of two copies of $E$ and $n-2$ empty sets. The [compression of an entropy sum](../../../information-theory.md#compression-of-an-entropy-sum) now gives

$$
2H(Y)\leq\sum_v H(Y_{S_v})\leq n(n-2).
$$

Exponentiating proves **the [entropy bound for graphs with isolated-vertex-free intersections](../../../information-theory.md#entropy-bound-for-graphs-with-isolated-vertex-free-intersections)**:

$$
\boxed{|\mathcal F|\leq2^{n(n-2)/2}=2^{n^2/2-n}.}
$$

## 3

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Throughout this question the [binomial random graph](../../../graph-theory.md#binomial-random-graph) has $p=1/2$, as fixed in the introduction. Let $L=\log_2n$ and $s=\lceil2L\rceil$. Count the $s$-vertex [independent sets](../../../graph-theory.md#independent-set-graph-theory) by a [random variable](../../../random-variable.md) $I_s$. [Linearity of expectation](../../../probability-theory.md#linearity-of-expectation) gives

$$
\mathbb EI_s=\binom ns2^{-\binom s2}
\leq\frac{n^s2^{-s(s-1)/2}}{s!}
\leq\frac{\sqrt2\,n}{s!}=o(1).
$$

For the second inequality, $s\geq2L$ implies $sL-s(s-1)/2\leq s/2\leq L+1/2$. For the limit, $s!\geq(s/2)^{\lfloor s/2\rfloor}$ grows faster than $n$. By the [first moment method](../../../probability-inequality.md#first-moment-method), [with high probability](../../../probabilistic-combinatorics.md#with-high-probability) there is no such [independent set](../../../graph-theory.md#independent-set-graph-theory); any larger [independent set](../../../graph-theory.md#independent-set-graph-theory) would contain one. Thus the [independence number](../../../graph-theory.md#independence-number) satisfies $\alpha(G)\leq s-1<2L$ [with high probability](../../../probabilistic-combinatorics.md#with-high-probability).

Every class of a proper [graph coloring](../../../graph-theory.md#graph-coloring) is an [independent set](../../../graph-theory.md#independent-set-graph-theory), giving **the claimed chromatic lower bound**:

$$
\boxed{\chi(G)\geq\frac n{\alpha(G)}\geq\frac n{2\log_2n}\quad\text{with high probability}.}
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For the [clique count in a binomial random graph](../../../graph-theory.md#clique-count-in-a-binomial-random-graph), write

$$
\mu_r=\mathbb EX_r=\binom nr2^{-\binom r2},\qquad L=\log_2n.
$$

Fix $0<\varepsilon<1$. At $r_- =\lfloor(2-\varepsilon)L\rfloor$, the estimates $\binom nr\geq(n/r)^r$ and $r=O(L)$ give

$$
\log_2\mu_{r_-}\geq r_-L-\frac{r_-(r_--1)}2-r_-\log_2r_-
=\left(\varepsilon-\frac{\varepsilon^2}{2}\right)L^2-O(L\log L).
$$

This eventually exceeds $(9/5)L$. At $r_+=\lceil(2+\varepsilon)L\rceil$, the upper bound $\binom nr\leq n^r$ instead gives

$$
\log_2\mu_{r_+}\leq-\left(\varepsilon+\frac{\varepsilon^2}{2}\right)L^2+O(L),
$$

so $\mu_{r_+}<n^{9/5}$. Moreover

$$
\frac{\mu_{r+1}}{\mu_r}=\frac{n-r}{r+1}\,2^{-r}<1\qquad(r\geq r_+),
$$

so no later [clique](../../../graph-theory.md#clique-graph-theory) size can regain the threshold. The maximum defining $r_0$ exists for sufficiently large $n$, since $\mu_2=\binom n2/2\geq n^{9/5}$ then. We have $r_-\leq r_0<r_+$. Letting $\varepsilon$ decrease to zero proves **the asymptotic size**:

$$
\boxed{r_0=(2+o(1))\log_2n.}
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

We need [independent sets](../../../graph-theory.md#independent-set-graph-theory) in every sufficiently large remaining [induced subgraph](../../../graph-theory.md#induced-subgraph), rather than just one in the initial [random graph](../../../graph-theory.md#random-graph). The useful concentration variable is the maximum [edge-disjoint clique packing](../../../graph-theory.md#edge-disjoint-clique-packing) in the [complement graph](../../../graph-theory.md#complement-graph); changing one [edge](../../../graph-theory.md#edge-of-a-graph) changes that variable by at most one. This avoids the much larger sensitivity of the ordinary [clique count in a binomial random graph](../../../graph-theory.md#clique-count-in-a-binomial-random-graph).

First work in a [binomial random graph](../../../graph-theory.md#binomial-random-graph) $H\sim G(m,1/2)$, take $r=r_0(m)$, and let $X$ count its $r$-[cliques](../../../graph-theory.md#clique-graph-theory). Put $\mu=\mathbb EX\geq m^{9/5}$ and let $Z$ be its maximum [edge-disjoint clique packing](../../../graph-theory.md#edge-disjoint-clique-packing) size. Form the [clique conflict graph](../../../graph-theory.md#clique-conflict-graph) whose [vertices](../../../graph.md#vertex-graph-theory) are these [cliques](../../../graph-theory.md#clique-graph-theory), adjacent when they share an [edge](../../../graph-theory.md#edge-of-a-graph). If $Q$ counts unordered conflicting pairs, the [Caro-Wei bound](../../../graph-theory.md#caro-wei-bound) gives, for each realization,

$$
Z\geq\frac{X^2}{X+2Q}.
$$

To verify the bound, randomly order the [vertices](../../../graph.md#vertex-graph-theory) of a finite [graph](../../../graph.md) and retain each [vertex](../../../graph.md#vertex-graph-theory) preceding all its [graph neighbours](../../../graph-theory.md#neighbour-of-a-vertex). These retained [vertices](../../../graph.md#vertex-graph-theory) are an [independent set](../../../graph-theory.md#independent-set-graph-theory), with expected size $\sum_v(1+\deg v)^{-1}\geq X^2/(X+2Q)$ by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Interpret the ratio as zero when $X=0$. A second application of the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), now to [expectations](../../../probability-theory.md#expected-value), gives

$$
\mathbb EZ\geq\frac{\mu^2}{\mathbb E(X+2Q)}.
$$

Counting ordered pairs of $r$-sets with $j$ common [vertices](../../../graph.md#vertex-graph-theory), including identical sets when $j=r$, yields

$$
\Delta:=\frac{\mathbb E(X+2Q)}{\mu^2}
=\sum_{j=2}^r D_j,\qquad
D_j=\frac{\binom rj\binom{m-r}{r-j}}{\binom mr}\,2^{\binom j2}.
$$

The shared [edges](../../../graph-theory.md#edge-of-a-graph) account for the factor $2^{\binom j2}$. We claim

$$
\Delta=O(r^5/m^2)+O(1/\mu).
$$

Here are the estimates, including the large overlaps. For $2\leq j\leq\lfloor r/2\rfloor$, the probability that a random $r$-set contains any specified $j$ elements is at most $(r/(m-r))^j$. Summing over their choices inside the first $r$-set gives

$$
D_j\leq T_j:=\left(\frac{r^2}{m-r}\right)^j2^{j(j-1)/2}.
$$

The [logarithm](../../../calculus.md#logarithm) of $T_j$ is a [convex function](../../../real-analysis.md#convex-function), a quadratic in $j$, so the maximum on this interval is at an endpoint. We have $T_2=O(r^4/m^2)$. As $r=(2+o(1))\log_2m$, the other endpoint satisfies

$$
\log_2T_{\lfloor r/2\rfloor}
=-\left(\frac12+o(1)\right)(\log_2m)^2,
$$

and is smaller than $T_2$ for sufficiently large $m$. Summing at most $r$ terms gives $O(r^5/m^2)$.

For the other half of the overlaps, write $j=r-s$, where $0\leq s\leq\lceil r/2\rceil$. The exact identity and an upper bound are

$$
D_{r-s}=\frac1\mu\binom rs\binom{m-r}s2^{-sr+s(s+1)/2}
\leq\frac1\mu\left(rm\,2^{-3r/4+2}\right)^s.
$$

The quantity in parentheses is $m^{-1/2+o(1)}$, which tends to zero. The [geometric series](../../../real-analysis.md#geometric-series) is thus at most $2/\mu$ for sufficiently large $m$. This proves the claim. In fact $r^5/m^2=o(m^{-9/5})$ and $1/\mu\leq m^{-9/5}$, so eventually

$$
\Delta\leq3m^{-9/5},\qquad \mathbb EZ\geq\frac13m^{9/5}.
$$

Now expose the $N=\binom m2$ independent [edge](../../../graph-theory.md#edge-of-a-graph) indicators one at a time. The [edge-exposure martingale](../../../martingale.md#edge-exposure-martingale) $M_i=\mathbb E[Z\mid\text{first }i\text{ indicators}]$ starts at $\mathbb EZ$ and ends at $Z$. Deleting one [edge](../../../graph-theory.md#edge-of-a-graph) destroys at most one member of any [edge-disjoint clique packing](../../../graph-theory.md#edge-disjoint-clique-packing). Hence changing one indicator changes $Z$ by at most one; coupling the remaining indicators shows $|M_i-M_{i-1}|\leq1$.

Precisely, the [Azuma-Hoeffding inequality](../../../martingale.md#azuma-s-inequality) says that if $(M_i)_{i=0}^N$ is a [martingale](../../../martingale.md) and $|M_i-M_{i-1}|\leq c_i$ almost surely for deterministic $c_i$, then, for $t>0$,

$$
\mathbb P(M_N-M_0\leq-t)\leq
\exp\left(-\frac{t^2}{2\sum_{i=1}^Nc_i^2}\right),
\qquad
\mathbb P(M_N-M_0\geq t)\leq
\exp\left(-\frac{t^2}{2\sum_{i=1}^Nc_i^2}\right).
$$

If all $c_i=0$, the [martingale](../../../martingale.md) is constant. Applying the lower-tail inequality with $c_i=1$ and $t=\mathbb EZ$ gives

$$
\mathbb P(Z=0)\leq\exp\left(-\frac{(\mathbb EZ)^2}{2N}\right)
\leq\exp(-m^{8/5}/9)
$$

for sufficiently large $m$. This is the only [martingale](../../../martingale.md) concentration inequality needed.

Return to the original [binomial random graph](../../../graph-theory.md#binomial-random-graph) $G\sim G(n,1/2)$ and set $m=\lceil n/(\log_2n)^2\rceil$. For each fixed $m$-element [vertex](../../../graph.md#vertex-graph-theory) set $U$, the [complement graph](../../../graph-theory.md#complement-graph) of $G[U]$ has distribution $G(m,1/2)$. The [union bound](../../../probability-inequality.md#boole-s-inequality) therefore gives

$$
\mathbb P(\text{some }U\text{ has no independent }r_0(m)\text{-set in }G[U])
\leq\binom nm e^{-m^{8/5}/9}\leq2^n e^{-m^{8/5}/9}=o(1),
$$

since $m^{8/5}/n\to\infty$. Thus [with high probability](../../../probabilistic-combinatorics.md#with-high-probability) every [vertex](../../../graph.md#vertex-graph-theory) set of size at least $m$ contains an [independent set](../../../graph-theory.md#independent-set-graph-theory) of size

$$
r_0(m)=(2+o(1))\log_2m=(2+o(1))\log_2n.
$$

Apply [greedy colouring by removing independent sets](../../../graph-theory.md#greedy-colouring-by-removing-independent-sets): remove such an [independent set](../../../graph-theory.md#independent-set-graph-theory), give it a fresh colour, and repeat while at least $m$ [vertices](../../../graph.md#vertex-graph-theory) remain. Give each of the fewer than $m$ final [vertices](../../../graph.md#vertex-graph-theory) its own colour. This uses at most

$$
\frac n{r_0(m)}+m=(1+o(1))\frac n{2\log_2n}
$$

colours, since $m=o(n/\log_2n)$. Together with the lower bound, **this gives the [chromatic number of the half-density binomial random graph](../../../graph-theory.md#chromatic-number-of-the-half-density-binomial-random-graph)**:

$$
\boxed{\chi(G(n,1/2))=(1+o(1))\frac n{2\log_2n}\quad\text{with high probability}.}
$$

## 4

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For each element $x$ of the [product set](../../../additive-combinatorics.md#product-set) $A\cdot B$, let $s_x$ count its representations as $ab$ with $(a,b)\in A\times B$. The ratio equality $a/b=c/d$ is equivalent to $ad=cb$. Swapping the two $B$ coordinates is a [bijection](../../../function.md#bijection) between the ratio-equality quadruples and the equal-product quadruples. Therefore the [multiplicative energy](../../../additive-combinatorics.md#multiplicative-energy) satisfies

$$
E(A,B)=\sum_{x\in A\cdot B}s_x^2,\qquad
\sum_{x\in A\cdot B}s_x=|A||B|.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives **the energy lower bound**:

$$
\boxed{E(A,B)\geq\frac{|A|^2|B|^2}{|A\cdot B|}.}
$$

For the upper bound, place the [Cartesian product](../../../set-theory.md#cartesian-product) $P=A\times B$ in the strictly positive quadrant. For every occupied [Euclidean ray](../../../geometry-and-topology.md#euclidean-ray) from the origin let $P_\lambda$ be its points and $r_\lambda=|P_\lambda|$. The slope is $\lambda=b/a$, so

$$
E(A,B)=\sum_\lambda r_\lambda^2,\qquad 1\leq r_\lambda\leq |B|.
$$

Take $\log$ to be the [natural logarithm](../../../calculus.md#natural-logarithm) and put $L=\lceil\log|B|\rceil\geq1$, using the non-triviality assumption $|B|\geq2$. Partition the possible occupancies into $L$ classes: $[e^j,e^{j+1})$ for $0\leq j<L-1$, and $[e^{L-1},|B|]$ for the last class. This last closed endpoint ensures that the partition works even when the top endpoint is attained. Within each class the ratio of any two occupancies is at most $e$.

Fix one class and order its occupied [Euclidean rays](../../../geometry-and-topology.md#euclidean-ray) by increasing slope, with occupancies $r_1,\ldots,r_t$. Write $S=|A+A||B+B|$, the [cardinality](../../../set-theory.md#cardinality) of $(A+A)\times(B+B)$. If $t=1$, then $r_1^2\leq|A||B|\leq S$, since adding any fixed element gives an [injection](../../../algebra.md#injective-function) of $A$ into its [sumset](../../../additive-combinatorics.md#sumset) $A+A$, and similarly for $B$.

If $t\geq2$, the sums $P_i+P_{i+1}$ contain exactly $r_ir_{i+1}$ different points, by [injectivity of sums on two distinct rays](../../../geometry-and-topology.md#injectivity-of-sums-on-two-distinct-rays). Indeed, the two direction vectors are [linearly independent](../../../vector-space.md#linear-independence), so the [coefficients](../../../vector-space.md#coefficient) of a sum uniquely recover its two summands. Positivity puts every sum strictly inside the [open planar sector](../../../geometry-and-topology.md#open-planar-sector) between those two [Euclidean rays](../../../geometry-and-topology.md#euclidean-ray). The sectors between successive selected [Euclidean rays](../../../geometry-and-topology.md#euclidean-ray) are disjoint, even if there are additional unselected rays between them. All these sums belong to $(A+A)\times(B+B)$, and hence

$$
S\geq\sum_{i=1}^{t-1}r_ir_{i+1}.
$$

For neighbouring occupancies their ratio lies between $e^{-1}$ and $e$, so

$$
r_i^2+r_{i+1}^2\leq(e+e^{-1})r_ir_{i+1}<4r_ir_{i+1}.
$$

Summing covers every $r_i^2$ at least once, and gives $\sum_i r_i^2\leq4S$. The same bound holds for empty or singleton classes by the preceding observations. Adding over the $L$ classes proves the [multiplicative energy sumset bound](../../../additive-combinatorics.md#multiplicative-energy-sumset-bound) $E(A,B)\leq4LS$. Combining both bounds yields **the sum-product conclusion**:

$$
\boxed{\frac{|A|^2|B|^2}{4\lceil\log|B|\rceil}
\leq |A\cdot B|\,|A+A|\,|B+B|.}
$$

If instead $\log$ is interpreted as base two, use the same $L=\lceil\log_2|B|\rceil$ occupancy classes with $2$ in place of $e$; $2+2^{-1}<4$ proves that convention as well. Positivity is essential to the sector argument.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
