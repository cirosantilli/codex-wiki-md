# Paper 12

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_12.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_12.pdf)

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

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $K_s(t)$ for the balanced [graph blow-up](../../../graph.md#graph-blow-up) of a [complete graph](../../../graph-theory.md#complete-graph), with $s$ classes of size $t$; containment here is as a subgraph, not necessarily an induced subgraph. The logarithmic form of the [Erdős-Stone theorem](../../../graph-theory.md#erdos-stone-theorem) is: for fixed $r\ge1$ and $0<\epsilon<1/r$, there are $d=d(r,\epsilon)>0$ and $n_0$ such that

$$
e(G)\ge\left(1-\frac1r+\epsilon\right)\binom n2,\qquad n\ge n_0
\quad\Longrightarrow\quad K_{r+1}(\lfloor d\log n\rfloor)\subseteq G.
$$

Thus **the guaranteed balanced part size is at least $\lfloor d\log n\rfloor$**, with $d$ independent of $n$. We prove the [logarithmic Erdős-Stone theorem](../../../graph-theory.md#logarithmic-erdos-stone-theorem) by a density-to-cliques step and a constructive [dense clique family blow-up lemma](../../../graph.md#dense-clique-family-blow-up-lemma).

First choose a fixed $m$ large enough that $t_r(m)/\binom m2\le1-1/r+\epsilon/2$, where $t_r(m)$ is the [edge](../../../graph-theory.md#edge-of-a-graph) count of the [Turán graph](../../../graph-theory.md#turan-graph). A uniformly chosen $m$-vertex subset has expected [edge](../../../graph-theory.md#edge-of-a-graph) count at least $(1-1/r+\epsilon)\binom m2$. If its induced [graph](../../../graph.md) contains no $K_{r+1}$, the [Turan theorem](../../../graph-theory.md#turan-s-theorem) bounds that count by $t_r(m)$. Since the count is always at most $\binom m2$, the probability that the subset contains an $(r+1)$-clique is at least $\epsilon/2$. Double counting the incidences between such subsets and their [cliques](../../../graph-theory.md#clique-graph-theory) gives, for $s=r+1$,

$$
k_s(G)\ge\frac\epsilon2\frac{\binom nm}{\binom{n-s}{m-s}}=\frac\epsilon2\frac{(n)_s}{(m)_s}\ge\eta n^s
$$

for a fixed $\eta>0$ and all sufficiently large $n$. Here $(x)_s=x(x-1)\cdots(x-s+1)$. This is [clique supersaturation by sampling](../../../graph-theory.md#clique-supersaturation-by-sampling).

We now prove the needed [dense clique family blow-up lemma](../../../graph.md#dense-clique-family-blow-up-lemma), with the following stronger induction invariant. Given any family $\mathcal M$ of at least $\eta n^s$ distinct $s$-cliques, there is a complete $s$-partite subgraph with each class of size $\lfloor a_s(\eta)\log n\rfloor$, containing that many pairwise vertex-disjoint transversal members of $\mathcal M$, each with one vertex in every class. Extra [edges](../../../graph-theory.md#edge-of-a-graph) within its classes can be ignored. We may suppose $0<\eta<1/2$. For $s=1$, any $\eta n$ singletons suffice, and we may take $a_1(\eta)=1$ once $n$ is large.

For $s\ge2$, put $\theta=\eta/2$. Repeatedly delete every member of the current family containing an $(s-1)$-clique whose number of extensions is at most $\theta n$. Each such face is processed at most once, and there are at most $n^{s-1}$ possible faces. At most $\theta n^s$ members are deleted. The remaining family $\mathcal L$ has size at least $(\eta/2)n^s$, and every face that remains has more than $\theta n$ extensions. Its family of $(s-1)$-faces has size at least $s|\mathcal L|/n\ge(\eta/2)n^{s-1}$, since each face is in at most $n$ members.

Apply the induction hypothesis to these faces. It gives a complete $(s-1)$-partite subgraph with $m=\lfloor a_{s-1}(\eta/2)\log n\rfloor$ [vertices](../../../graph.md#vertex-graph-theory) in each class and a matching $R_1,\ldots,R_m$ of transversal $(s-1)$-faces from the family. Form a [bipartite graph](../../../graph-theory.md#bipartite-graph) whose left [vertices](../../../graph.md#vertex-graph-theory) are the $R_i$ and whose right [vertices](../../../graph.md#vertex-graph-theory) are the original $n$ [vertices](../../../graph.md#vertex-graph-theory); join $R_i$ to $v$ when $R_i\cup\{v\}\in\mathcal L$. Every left degree exceeds $\theta n$.

The following [common neighbourhood from bipartite density](../../../graph-theory.md#common-neighbourhood-from-bipartite-density) estimate is elementary. In a bipartite [graph](../../../graph.md) with class sizes $m,n$ and at least $\theta mn$ [edges](../../../graph-theory.md#edge-of-a-graph), averaging over left subsets $S$ of size $u$ and using convexity of the integer sequence $j\mapsto\binom ju$ gives

$$
\max_{|S|=u}|N(S)|\ge\frac{\sum_{v\text{ on right}}\binom{d(v)}u}{\binom mu}
\ge n\frac{\binom{\lfloor\theta m\rfloor}u}{\binom mu}\ge n(\theta/2)^u
$$

whenever $1\le u\le\theta m/2$. The last inequality follows by comparing the $u$ factors in the two binomial coefficients; the integer convexity follows from the nondecreasing first differences $\binom j{u-1}$.

Choose

$$
a_s(\eta)=\min\left\{\frac{\theta a_{s-1}(\eta/2)}8,\ \frac1{2\log(2/\theta)}\right\},\qquad u=\lfloor a_s(\eta)\log n\rfloor.
$$

For large $n$, $m\ge\tfrac12a_{s-1}(\eta/2)\log n$, so $u\le\theta m/4$. The estimate supplies $u$ selected faces with a common extension set of size at least $n(\theta/2)^u\ge\sqrt n$. This extension set is disjoint from the selected faces: a [vertex](../../../graph.md#vertex-graph-theory) in any one of them cannot extend that face. Their union has $u$ [vertices](../../../graph.md#vertex-graph-theory) in each of the old $s-1$ classes, with all required cross [edges](../../../graph-theory.md#edge-of-a-graph); choose $u$ distinct common extension [vertices](../../../graph.md#vertex-graph-theory) as a new class. Attaching one different extension [vertex](../../../graph.md#vertex-graph-theory) to each selected face also gives $u$ disjoint members of $\mathcal L$. This completes the induction, with positive constants independent of $n$. Apply it to the [clique](../../../graph-theory.md#clique-graph-theory) family above and take $d=a_{r+1}(\eta)$.

The logarithmic order cannot be increased in a uniform forcing result. Put $\rho=1-1/r+\epsilon<1$, choose $p$ strictly between $\rho$ and one, and take a [binomial random graph](../../../graph-theory.md#binomial-random-graph). Its [edge](../../../graph-theory.md#edge-of-a-graph) density exceeds $\rho$ with probability tending to one, by the variance estimate for a sum of independent [edge](../../../graph-theory.md#edge-of-a-graph) indicators. With $s=r+1$, the expected number of ordered embeddings of $K_s(t)$ is at most

$$
n^{st}p^{\binom s2t^2}.
$$

For $t=\lceil C\log n\rceil$ and $C>2/((s-1)\log(1/p))$, the logarithm of this bound is negative of order $(\log n)^2$. [Markov's inequality](../../../probability-inequality.md#markov-inequality) therefore makes the probability of any such copy tend to zero. Both events hold simultaneously for some [graphs](../../../graph.md) of every sufficiently large order. **There are [graphs](../../../graph.md) meeting the density hypothesis whose largest balanced blow-up has part size $O(\log n)$.** This upper bound concerns what density can force; it is not an upper bound for every dense [graph](../../../graph.md), since a complete [graph](../../../graph.md) has much larger blow-ups.

Finally, $H_k$ is the [square of a cycle](../../../graph.md#square-of-a-cycle), for $k\ge3$. Any three consecutive [vertices](../../../graph.md#vertex-graph-theory) form a [triangle in a graph](../../../graph.md#triangle-in-a-graph). In a proper three-colouring, once the first three colours are fixed, each subsequent [vertex](../../../graph.md#vertex-graph-theory) must repeat the colour three positions earlier. Closing the cycle is possible precisely when $3\mid k$. Conversely, repeating the three colours gives such a colouring whenever $3\mid k$. In that case $H_k$ embeds in $K_3(k/3)$, and the density $0.51\binom n2$ exceeds the bipartite [Turan theorem](../../../graph-theory.md#turan-s-theorem) threshold by a fixed amount, so the theorem forces $H_k$ eventually. If $3\nmid k$, the balanced [Turán graphs](../../../graph-theory.md#turan-graph) $T_3(n)$ have density at least $2/3$ and contain no [graph](../../../graph.md) of chromatic number greater than three. They give a counterexample sequence. **Exactly the cycle lengths $k\ge3$ divisible by three have the required property.**

## 2

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a fixed [uniform hypergraph](../../../hypergraph.md#uniform-hypergraph) $H$ with $h$ [vertices](../../../graph.md#vertex-graph-theory), uniformity $\ell$, and at least one [edge](../../../graph-theory.md#edge-of-a-graph), define its [Turán density](../../../hypergraph.md#turan-density) by

$$
\pi(H)=\lim_{n\to\infty}\frac{\operatorname{ex}(n,H)}{\binom n\ell},
$$

where $\operatorname{ex}(n,H)$ is the maximum [edge](../../../graph-theory.md#edge-of-a-graph) count of an $H$-free hypergraph. The limit exists: averaging the [edge](../../../graph-theory.md#edge-of-a-graph) count over all $m$-vertex subsets of an extremal $n$-vertex hypergraph, with $n\ge m\ge\ell$, shows that the displayed normalized extremal numbers are nonincreasing. Thus their limit is their infimum.

For [hypergraph supersaturation by sampling](../../../hypergraph.md#hypergraph-supersaturation-by-sampling), choose $m\ge h$ so that $\operatorname{ex}(m,H)/\binom m\ell\le\pi(H)+\epsilon/2$. The expected [edge](../../../graph-theory.md#edge-of-a-graph) count in a uniform $m$-vertex subset of $G$ is at least $(\pi(H)+\epsilon)\binom m\ell$. A subset containing no copy of $H$ has at most $(\pi(H)+\epsilon/2)\binom m\ell$ [edges](../../../graph-theory.md#edge-of-a-graph), while any subset has at most $\binom m\ell$. Hence at least an $\epsilon/2$ fraction of the subsets contain $H$. Every particular copy of $H$ lies in exactly $\binom{n-h}{m-h}$ such subsets, so their number is at least

$$
\frac\epsilon2\frac{\binom nm}{\binom{n-h}{m-h}}=\frac\epsilon2\frac{(n)_h}{(m)_h}\ge\frac{\epsilon}{2^{h+1}(m)_h}n^h
$$

for $n\ge N=\max(m,2h)$. Take

$$
\delta=\min\left\{\frac{\epsilon}{2^{h+1}(m)_h},\ \frac1{2N^h}\right\}.
$$

For $n<N$, the requested integer lower bound is zero; for $n\ge N$, the calculation proves it. **This positive $\delta$ depends only on $H$ and $\epsilon$.** If the density hypothesis is impossible there is nothing to prove. For an edgeless $H$, every $h$-set is already a copy and the conclusion follows directly.

For the edge-triangle objective, let $N(v)$ be the open neighbourhood of $v$ and define its local score

$$
s(v)=d(v)-c\,e(G[N(v)]).
$$

It counts the contribution to $k_2-ck_3$ of [edges](../../../graph-theory.md#edge-of-a-graph) and [triangles in a graph](../../../graph.md#triangle-in-a-graph) containing $v$. If $u,v$ are nonadjacent, making $u$ a [false twin](../../../graph.md#false-twin) of $v$ changes the objective by $s(v)-s(u)$, since no [edge](../../../graph-theory.md#edge-of-a-graph) or [triangle in a graph](../../../graph.md#triangle-in-a-graph) uses both. More generally, partition [vertices](../../../graph.md#vertex-graph-theory) into [false-twin classes](../../../graph.md#false-twin-class), meaning equal open neighbourhoods. If distinct classes $U,V$ have no [edges](../../../graph-theory.md#edge-of-a-graph) between them, making every [vertex](../../../graph.md#vertex-graph-theory) of $U$ a twin of a representative of $V$ changes the objective by $|U|(s(v)-s(u))$. Choose the direction with nonnegative change.

Among [graphs](../../../graph.md) maximizing the objective, choose one maximizing the sum of squared false-twin class sizes. The operation cannot split any old false-twin class and merges $U,V$, so it would strictly increase that secondary quantity. Therefore no two distinct classes can be nonadjacent. **An objective maximizer is a complete multipartite [graph](../../../graph.md).** This [edge-triangle symmetrization](../../../graph-theory.md#edge-triangle-symmetrization) works for every real $c$, with no assumption on its sign.

For positive part sizes $a_1,\ldots,a_q$, the correct multipartite formula is

$$
F(a_1,\ldots,a_q)=\sum_{i<j}a_ia_j-c\sum_{i<j<k}a_ia_ja_k.
$$

The first sum in the printed intermediate formula has inconsistent indices; the [edge](../../../graph-theory.md#edge-of-a-graph) count is the pairwise-product sum above. Fix two part sizes with sum $A$ and let $B$ be the sum of all other sizes. All terms varying with the pair have the form

$$
\text{constant}+(1-cB)a_ia_j.
$$

Choose a maximizing partition with the fewest nonempty parts. If $1-cB\le0$, merging those two parts cannot decrease $F$ and reduces the number of parts, a contradiction. Therefore this coefficient is positive for every pair. If two integer sizes differ by at least two, moving one [vertex](../../../graph.md#vertex-graph-theory) from the larger to the smaller increases their product and hence $F$, again a contradiction. **All sizes differ by at most one, so a maximizer is a Turan [graph](../../../graph.md).** This is [balancing a multipartite edge-triangle objective](../../../graph-theory.md#balancing-a-multipartite-edge-triangle-objective).

Next maximize the same polynomial on the compact simplex of nonnegative real sizes summing to $n$, starting with at least two possible parts. Choose a maximizer with the smallest positive support. The merging argument still applies, and now varying two positive unequal sizes towards equality improves the product. Thus every positive size is $n/q$ for some integer $q$. A two-part choice has value $n^2/4>0$ when $n>0$, so $q\ge2$. The optimum is attained at rational sizes, and therefore

$$
\boxed{k_2(G)-ck_3(G)\le\binom q2(n/q)^2-c\binom q3(n/q)^3\quad\text{for some integer }q\ge2.}
$$

One may take the initial simplex to have $\max(n,2)$ coordinates, so it includes every multipartite [graph](../../../graph.md) obtained above; zero coordinates are discarded.

Set $c=9/(4n)$. Dividing the right side by $n^2$ gives

$$
\frac{(q-1)(q+6)}{8q^2}=\frac14-\frac{(q-2)(q-3)}{8q^2}\le\frac14,
$$

because $q$ is an integer at least two. Rearranging proves

$$
\boxed{k_3(G)\ge\frac{4n}{9}\left(k_2(G)-\frac{n^2}{4}\right).}
$$

Equality in the continuous calculation occurs at two or three equal parts, explaining the [triangle support line between bipartite and tripartite Turan graphs](../../../graph-theory.md#triangle-support-line-between-bipartite-and-tripartite-turan-graphs).

## 3

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

We prove [edit-distance stability for clique-free graphs](../../../graph-theory.md#edit-distance-stability-for-clique-free-graphs) by induction on $r$, using the [symmetric difference](../../../set.md#symmetric-difference) of [edge](../../../graph-theory.md#edge-of-a-graph) sets as the distance. For $r=1$, a $K_2$-free [graph](../../../graph.md) is edgeless, and there is nothing to change. For $r\ge2$, choose a [vertex](../../../graph.md#vertex-graph-theory) of maximum degree $d$, let $A$ be its neighbourhood and put $B=V(G)\setminus A$. Then $G[A]$ is $K_r$-free. Write

$$
D=t_r(n)-e(G),\qquad D_A=t_{r-1}(d)-e(G[A]),\qquad b=e(G[B]),\qquad m=|A||B|-e_G(A,B).
$$

Both deficits are nonnegative by the [Turan theorem](../../../graph-theory.md#turan-s-theorem). Since every [vertex](../../../graph.md#vertex-graph-theory) of $B$ has degree at most $d=|A|$,

$$
e_G(A,B)+2b\le |B|d,\qquad m\ge2b.
$$

The complete $r$-partite [graph](../../../graph.md) formed from an $(r-1)$-partite [Turán graph](../../../graph-theory.md#turan-graph) on $A$ and the new class $B$ has at most $t_r(n)$ [edges](../../../graph-theory.md#edge-of-a-graph). Thus $L=t_r(n)-t_{r-1}(d)-|A||B|\ge0$, and direct subtraction gives

$$
D=L+D_A+m-b.
$$

By induction, edit $G[A]$ into a complete $(r-1)$-partite [graph](../../../graph.md) using at most $3D_A$ changes. Delete the $b$ [edges](../../../graph-theory.md#edge-of-a-graph) inside $B$, and add the $m$ missing [edges](../../../graph-theory.md#edge-of-a-graph) between $A$ and $B$. The resulting [graph](../../../graph.md) is complete $r$-partite on the same [vertex](../../../graph.md#vertex-graph-theory) set, and

$$
3D_A+b+m\le3D_A+3(m-b)+3L=3D\le3k,
$$

where the inequality uses $m\ge2b$. **The required edit distance is at most $3k$.** Empty partition classes are allowed; a sufficiently dense nondegenerate case has the usual full complement of classes.

For the odd-cycle conclusion, use two standard consequences of the [Szemerédi regularity lemma](../../../probabilistic-combinatorics.md#szemeredi-regularity-lemma), stated explicitly. The [triangle removal lemma](../../../probabilistic-combinatorics.md#triangle-removal-lemma) says that for every $\alpha>0$, some $\beta>0$ ensures that a [graph](../../../graph.md) with at most $\beta n^3$ [triangles in a graph](../../../graph.md#triangle-in-a-graph) can be made triangle-free by deleting at most $\alpha\binom n2$ [edges](../../../graph-theory.md#edge-of-a-graph), for all sufficiently large $n$. Also, for each fixed odd length $\ell\ge3$ and each $\beta>0$, there is $\zeta>0$ such that a [graph](../../../graph.md) with at least $\beta n^3$ [triangles in a graph](../../../graph.md#triangle-in-a-graph) contains at least $\zeta n^\ell$ copies of $C_\ell$.

For clarity, the latter [odd-cycle copies from positive triangle density](../../../probabilistic-combinatorics.md#odd-cycle-copies-from-positive-triangle-density) consequence follows by applying regularity with error small relative to $\beta$, removing exceptional, irregular and very sparse pairs, and retaining a [triangle in a graph](../../../graph.md#triangle-in-a-graph) among the remaining regular dense pairs. The [graph embedding lemma for regular pairs](../../../probabilistic-combinatorics.md#graph-embedding-lemma-for-regular-pairs) counts a positive constant times $n^\ell$ embeddings of any fixed [graph](../../../graph.md) properly three-coloured into those three clusters, including $C_\ell$. Dividing by the fixed number of descriptions of a cycle gives the same conclusion for unlabelled copies.

Apply [triangle in a graph](../../../graph.md#triangle-in-a-graph) removal with $\alpha=\epsilon$, and take the resulting $\beta$. A $C_{2013}$-free [graph](../../../graph.md) cannot have $\beta n^3$ [triangles in a graph](../../../graph.md#triangle-in-a-graph) for large $n$, by the preceding consequence. Delete at most $\epsilon\binom n2$ [edges](../../../graph-theory.md#edge-of-a-graph) to obtain a triangle-free $G'$. With $N=\binom n2$,

$$
e(G')\ge(1/2-2\epsilon)N,\qquad t_2(n)-e(G')\le2\epsilon N+n/4.
$$

Apply the proved stability result with $r=2$. The resulting complete bipartite [graph](../../../graph.md) $H$ satisfies

$$
|E(G)\mathbin\triangle E(H)|\le\epsilon N+3(2\epsilon N+n/4)=7\epsilon N+3n/4.
$$

Choose $n_0(\epsilon)$ also large enough that $3n/4\le4\epsilon N$. **Then the distance is at most $11\epsilon\binom n2$.**

For the unheaded continuation, use the same $\beta$ and its associated $\zeta$, and set $\delta=\zeta/2$. Having at most $\delta n^{2013}$ cycles rules out $\beta n^3$ [triangles in a graph](../../../graph.md#triangle-in-a-graph) just as before. The identical deletion and stability calculation applies. **A sufficiently small $\delta=\delta(\epsilon)>0$ gives the same $11\epsilon$ bound.**

## 4

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

In this enumeration problem, monotone means [subgraph-closed graph property](../../../graph-theory.md#subgraph-closed-graph-property): both deleting [vertices](../../../graph.md#vertex-graph-theory) and deleting [edges](../../../graph-theory.md#edge-of-a-graph) preserve membership. This is a decreasing convention, rather than the increasing-edge convention often used for random-graph thresholds. Assume first that the property is proper and has [graphs](../../../graph.md) of arbitrarily large orders. These are the usual nondegenerate hypotheses for the formula.

Put $r+1=\min\{\chi(F):F\notin\mathcal Q\}$. Every [graph](../../../graph.md) of [chromatic number](../../../graph-theory.md#chromatic-number) at most $r$ belongs to $\mathcal Q$. In particular, all subgraphs of a fixed balanced [Turán graph](../../../graph-theory.md#turan-graph) $T_r(n)$ belong. Choosing each of its [edges](../../../graph-theory.md#edge-of-a-graph) independently as present or absent gives

$$
|\mathcal Q_n|\ge2^{t_r(n)}=2^{(1-1/r)\binom n2+O(n)}.
$$

For the upper bound, fix $F\notin\mathcal Q$ with $\chi(F)=r+1$. Every member of $\mathcal Q$ is $F$-free, by closure under subgraphs.

We use the following standard regularity consequences. For every sufficiently small regularity error $\eta$, large minimum cluster count $q_0$, and fixed positive density cutoff $d$, the [Szemerédi regularity lemma](../../../probabilistic-combinatorics.md#szemeredi-regularity-lemma) gives an equitable partition into $q_0\le q\le M$ clusters and an exceptional set of at most $\eta n$ [vertices](../../../graph.md#vertex-graph-theory), with at most $\eta q^2$ irregular pairs. The [graph embedding lemma for regular pairs](../../../probabilistic-combinatorics.md#graph-embedding-lemma-for-regular-pairs) says that a fixed [graph](../../../graph.md) with a prescribed proper colouring embeds into the corresponding clusters if all its required cross pairs are regular with density at least $d$, provided $\eta$ is sufficiently small relative to $d$ and the [graph](../../../graph.md). Hence the [reduced graph of a regularity partition](../../../probabilistic-combinatorics.md#reduced-graph-of-a-regularity-partition), joining regular pairs of density at least $d$, is $K_{r+1}$-free: such a [clique](../../../graph-theory.md#clique-graph-theory) would embed $F$.

By the [Turan theorem](../../../graph-theory.md#turan-s-theorem), this reduced [graph](../../../graph.md) has at most $(1-1/r)q^2/2$ [edges](../../../graph-theory.md#edge-of-a-graph). On its dense pairs allow arbitrary choices of original [edges](../../../graph-theory.md#edge-of-a-graph), giving at most $(1-1/r)n^2/2+O(n)$ free binary choices. All [edges](../../../graph-theory.md#edge-of-a-graph) within clusters, touching the exceptional set, or lying in irregular pairs contribute $O((\eta+1/q_0)n^2)$ further choices. On each remaining pair there are at most $d$ times its number of possible [edges](../../../graph-theory.md#edge-of-a-graph). The elementary [binary entropy](../../../information-theory.md#binary-entropy) estimate

$$
\sum_{j\le dL}\binom Lj\le2^{H_2(d)L},\qquad H_2(d)=-d\log_2d-(1-d)\log_2(1-d),\quad 0<d<1/2,
$$

bounds the total sparse-pair contribution by $H_2(d)n^2/2$. The partition and pair classifications have at most $(M+1)^n2^{O(M^2)}$ descriptions, whose logarithm is $O(n)$ since $M$ is fixed. Choose $q_0$ large, then $d$ small, then $\eta$ sufficiently small; their total error can be made arbitrarily small. This proves

$$
\boxed{\log_2|\mathcal Q_n|=(1-1/r+o(1))\binom n2.}
$$

It is the [enumeration of subgraph-closed graph properties](../../../graph-theory.md#enumeration-of-subgraph-closed-graph-properties).

For the hereditary extension, a [hereditary graph property](../../../graph-theory.md#hereditary-graph-property) is closed under induced subgraphs. Define the [clique-independent partition class](../../../graph-theory.md#clique-independent-partition-class) $\mathcal C(a,b)$, for $0\le b\le a$, to consist of [graphs](../../../graph.md) partitionable into $a$ possibly empty classes, exactly $b$ designated as [cliques](../../../graph-theory.md#clique-graph-theory) and the other $a-b$ designated as independent sets; cross [edges](../../../graph-theory.md#edge-of-a-graph) are unrestricted. Thus $a$ is the total number of classes. The [colouring number of a hereditary graph property](../../../graph-theory.md#colouring-number-of-a-hereditary-graph-property) is

$$
r(\mathcal P)=\max\{a:\mathcal C(a,b)\subseteq\mathcal P\text{ for some }0\le b\le a\}.
$$

Use value zero if this set is empty, and infinity for the class of all [graphs](../../../graph.md).

**$r(\mathcal C(a,b))=a$ for $a\ge1$.** The lower bound follows from the definition. For the upper bound, fix any $s\in\{0,\ldots,a+1\}$ and a balanced partition of a large $N$-vertex set into $a+1$ classes with $s$ [clique](../../../graph-theory.md#clique-graph-theory) classes. Independent choices of cross [edges](../../../graph-theory.md#edge-of-a-graph) give $2^{(1-1/(a+1))N^2/2-O(1)}$ distinct [graphs](../../../graph.md) in $\mathcal C(a+1,s)$. On the other hand, all [graphs](../../../graph.md) in $\mathcal C(a,b)$ can be described by at most $a^N$ partitions, each with at most $(1-1/a)N^2/2$ unrestricted cross pairs. The former count is strictly larger for large $N$, so $\mathcal C(a+1,s)$ is not contained in $\mathcal C(a,b)$ for any $s$. A contained class with even more parts would contain one of these $(a+1)$-part classes by making unused parts empty, so it is also impossible.

The main changes for the [hereditary graph enumeration theorem](../../../graph-theory.md#hereditary-graph-enumeration-theorem) are as follows. The lower bound now uses a contained class $\mathcal C(r,b)$: within-class [edges](../../../graph-theory.md#edge-of-a-graph) are fixed as complete or empty, and the balanced cross pairs still give $(1-1/r)n^2/2-O(1)$ free [edge](../../../graph-theory.md#edge-of-a-graph) choices. For the upper bound, since no $\mathcal C(r+1,b)$ is wholly contained in $\mathcal P$, choose one forbidden induced [graph](../../../graph.md) $F_b\in\mathcal C(r+1,b)\setminus\mathcal P$ for each $b=0,\ldots,r+1$.

Use the standard [induced regularity template lemma](../../../probabilistic-combinatorics.md#induced-regularity-template-lemma): for a fixed finite forbidden induced family and any error tolerance, a regularity refinement gives bounded-size templates with internal [clique](../../../graph-theory.md#clique-graph-theory)/independent types and cross pairs classified as sparse, almost complete, or intermediate. A [clique](../../../graph-theory.md#clique-graph-theory) of intermediate pairs on $a$ classes realizes every fixed induced pattern consistent with the internal types of those classes. This induced embedding conclusion uses a Ramsey refinement within clusters and regularity for both [edges](../../../graph-theory.md#edge-of-a-graph) and nonedges; the total exceptional-pair cost can be made arbitrarily small. Applied to the $F_b$, a [clique](../../../graph-theory.md#clique-graph-theory) on $r+1$ intermediate classes would realize the forbidden $F_b$ whose number of [clique](../../../graph-theory.md#clique-graph-theory) types is $b$. Thus the [graph](../../../graph.md) of intermediate pairs is $K_{r+1}$-free. Only intermediate pairs contribute unrestricted binary choices; sparse pairs and the missing [edges](../../../graph-theory.md#edge-of-a-graph) in almost-complete pairs each have the same entropy bound as before. The [Turan theorem](../../../graph-theory.md#turan-s-theorem) and the earlier counting argument now give

$$
\boxed{|\mathcal P_n|=2^{(1-1/r+o(1))\binom n2},\qquad r=r(\mathcal P).}
$$

This formula assumes $1\le r<\infty$. For the universal property the count is exactly $2^{\binom n2}$; a hereditary property of bounded order has $r=0$ and has no [graphs](../../../graph.md) on sufficiently large [vertex](../../../graph.md#vertex-graph-theory) sets, so the displayed expression with $1/r$ is not applicable.

For a proper [subgraph-closed graph property](../../../graph-theory.md#subgraph-closed-graph-property), any contained $\mathcal C(a,b)$ must have $b=0$: if $b\ge1$, it contains arbitrarily large complete [graphs](../../../graph.md), and closure under subgraphs would force every [graph](../../../graph.md) into the property. Consequently its colouring number is exactly one less than the least chromatic number of an excluded [graph](../../../graph.md). The excluded family of an intersection is the union of the two excluded families, whose minimum chromatic number is the smaller of their minima. Therefore **$r(\mathcal P\cap\mathcal Q)=\min(r(\mathcal P),r(\mathcal Q))$ for subgraph-closed properties**, with the universal case treated by $r=\infty$.

For hereditary properties take $\mathcal P=\mathcal C(2,0)$ and $\mathcal Q=\mathcal C(2,2)$, both of colouring number two. A [graph](../../../graph.md) in their intersection is both bipartite and a union of two [cliques](../../../graph-theory.md#clique-graph-theory). A [clique](../../../graph-theory.md#clique-graph-theory) in a bipartite [graph](../../../graph.md) has at most two [vertices](../../../graph.md#vertex-graph-theory); hence every such [graph](../../../graph.md) has at most four [vertices](../../../graph.md#vertex-graph-theory). The intersection contains no complete clique-independent class on arbitrarily large orders, so **$r(\mathcal P\cap\mathcal Q)=0<2$**. This also demonstrates why the bounded-order exception to the enumeration formula is necessary.

## 5

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Expose the independent coordinates one at a time and define the [Doob exposure martingale](../../../martingale.md#doob-exposure-martingale)

$$
M_i=\mathbb E[f\mid Z_1,\ldots,Z_i],\qquad M_0=\mathbb Ef,\qquad M_n=f.
$$

For a fixed exposed prefix, couple the future coordinates identically under two choices of $Z_i$. The coordinate-change hypothesis bounds the difference of the resulting conditional expectations by $c_i$. Thus the increment $D_i=M_i-M_{i-1}$ has conditional mean zero and lies in a conditional interval of length at most $c_i$. This range bound, rather than merely $|D_i|\le c_i$, gives the sharp constant in the [McDiarmid inequality](../../../probability-inequality.md#mcdiarmid-s-inequality).

Here is a proof of the needed [Hoeffding lemma](../../../probability-inequality.md#hoeffding-lemma). For a mean-zero random variable $X$ in an interval of length $c$, let $h(u)=\log\mathbb E e^{uX}$. Its second derivative is the variance under the exponentially tilted distribution. A random variable in $[a,b]$ has variance at most $(b-a)^2/4$: the inequality $\mathbb E[(X-a)(b-X)]\ge0$ gives $\operatorname{Var}X\le(\mathbb EX-a)(b-\mathbb EX)\le(b-a)^2/4$. Hence $h''(u)\le c^2/4$, and $h(0)=h'(0)=0$ imply $h(u)\le u^2c^2/8$, for either sign of $u$.

Apply this conditionally to each increment and iterate the [conditional expectation](../../../measure-theory.md#conditional-expectation):

$$
\mathbb E e^{u(f-\mathbb Ef)}\le\exp\left(\frac{u^2}{8}\sum_{i=1}^n c_i^2\right).
$$

For $u>0$, [Markov's inequality](../../../probability-inequality.md#markov-inequality) bounds the upper tail by $\exp(-ut+u^2\sum c_i^2/8)$. Taking $u=4t/\sum c_i^2$ and then applying the same argument to $-f$ gives

$$
\boxed{\mathbb P(|f-\mathbb Ef|\ge t)\le2\exp\left(-\frac{2t^2}{\sum_i c_i^2}\right).}
$$

At $t=0$ the bound is immediate. If all $c_i$ vanish, $f$ is constant on the product support and the positive tails are zero, so that degenerate case is handled directly.

For a [binomial random graph](../../../graph-theory.md#binomial-random-graph), let coordinate $i$ be the entire vector of [edges](../../../graph-theory.md#edge-of-a-graph) from [vertex](../../../graph.md#vertex-graph-theory) $i$ to [vertices](../../../graph.md#vertex-graph-theory) of smaller label. The coordinates are independent finite probability spaces. Changing coordinate $i$ changes only [edges](../../../graph-theory.md#edge-of-a-graph) incident to that one [vertex](../../../graph.md#vertex-graph-theory). Deleting the [vertex](../../../graph.md#vertex-graph-theory) gives the same [graph](../../../graph.md) under both outcomes, and each outcome's [chromatic number](../../../graph-theory.md#chromatic-number) is either that [graph](../../../graph.md)'s chromatic number or one more. Thus the coordinate range is at most one. Taking all $c_i=1$ and $t=\lambda\sqrt n$ proves [vertex exposure for chromatic number](../../../graph-theory.md#vertex-exposure-for-chromatic-number):

$$
\boxed{\mathbb P\bigl(|\chi(G)-\mathbb E\chi(G)|\ge\lambda\sqrt n\bigr)\le2e^{-2\lambda^2}.}
$$

Using individual [edges](../../../graph-theory.md#edge-of-a-graph) as coordinates would give a weaker scale; grouping the incident [edges](../../../graph-theory.md#edge-of-a-graph) is what yields the required bound.

For the expectation asymptotic, take fixed $0<p<1$, put $b=1/(1-p)$, and write $L=\log_b n$. We outline both bounds and the step that turns probability estimates into an expectation estimate. For each fixed $\gamma>0$, the expected number of independent sets of size $k=\lceil(2+\gamma)L\rceil$ is

$$
\binom nk(1-p)^{\binom k2}.
$$

Its logarithm is $k\log n-\tfrac12k(k-1)\log b-O(k\log k)=-\Omega_\gamma((\log n)^2)$. Thus [Markov's inequality](../../../probability-inequality.md#markov-inequality) gives $\alpha(G)\le(2+\gamma)L$ with probability tending to one, and $\chi(G)\ge n/\alpha(G)$ yields the corresponding lower bound on its expectation.

For the upper bound, set $m_0=\lceil n/(\log n)^2\rceil$ and $k=\lfloor(2-\gamma)L\rfloor$, with $0<\gamma<1$. The key uniform fact is that **every [vertex](../../../graph.md#vertex-graph-theory) subset of size at least $m_0$ contains an independent $k$-set with probability tending to one**. For a fixed subset of size $m$, let $X$ count its independent $k$-sets and let $\mu=\binom mk b^{-\binom k2}$. The normalized dependency sum in [Janson inequality](../../../probability-inequality.md#janson-inequality) is bounded by

$$
\frac{\Delta}{\mu^2}\le\sum_{j=2}^{k-1}\frac{\binom kj\binom{m-k}{k-j}}{\binom mk}\,b^{\binom j2}.
$$

The $j=2$ term is $O(k^4/m^2)$. The remaining overlap terms give the same order or less: use $\binom kj\binom{m-k}{k-j}/\binom mk\le(2k^2/m)^j$ for large $n$, and split the sum at $k/2$. For the lower half the terms beyond $j=2$ decrease at the initial endpoint and are exponentially small at the other endpoint; for the upper half, $k\le(2-\gamma/2)\log_b m$ makes every endpoint exponent negative of order $(\log n)^2$. Also $1/\mu$ is exponentially small on that scale. The exponential form of [Janson inequality](../../../probability-inequality.md#janson-inequality) therefore gives, uniformly for $m\ge m_0$,

$$
\mathbb P(X=0)\le\exp(-c_\gamma m^2/k^4)
$$

for a positive constant depending only on $p,\gamma$. A union bound over at most $2^n$ subsets succeeds, because $m_0^2/k^4$ is of order $n^2/(\log n)^8\gg n$. This is [independent sets in every large subset of a dense random graph](../../../graph-theory.md#independent-sets-in-every-large-subset-of-a-dense-random-graph).

On that event, repeatedly remove an independent $k$-set and assign it one new colour until fewer than $m_0$ [vertices](../../../graph.md#vertex-graph-theory) remain; colour the remainder individually. This gives $\chi(G)\le n/k+m_0$. The failure probability is exponentially small compared with $1/\log n$, and always $\chi(G)\le n$, so the failure event contributes negligibly to the expectation. Combining the upper and lower bounds and then letting $\gamma\downarrow0$ proves

$$
\boxed{\mathbb E\chi(G)=(1+o(1))\frac{n}{2\log_{1/(1-p)}n}.}
$$

This is the [chromatic number of a binomial random graph](../../../graph-theory.md#chromatic-number-of-a-binomial-random-graph) asymptotic. The slash in the printed expression must be read with $2\log_{1/(1-p)}n$ as the denominator; a multiplicative reading would eventually exceed $n$. At the endpoint probabilities $p=0$ and $p=1$, the chromatic numbers are respectively one and $n$ for $n\ge1$, so this logarithmic formula is intended for $0<p<1$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
