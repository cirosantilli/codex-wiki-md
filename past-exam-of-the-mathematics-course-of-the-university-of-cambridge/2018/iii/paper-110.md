# Paper 110

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_110.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_110.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 110](paper-110.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $\alpha=1-1/r$. The [Erdős-Stone theorem](../../../graph-theory.md#erdos-stone-theorem) states that, for a fixed [graph](../../../graph.md) $F$ with [chromatic number](../../../graph-theory.md#chromatic-number) $\chi(F)=r+1\geq2$,

$$
\boxed{\operatorname{ex}(n,F)=\left(1-\frac1r+o(1)\right)\binom n2.}
$$

Here $\operatorname{ex}$ is the [extremal number](../../../graph-theory.md#extremal-number), and copies are [subgraphs](../../../graph-theory.md#subgraph), not necessarily [induced subgraphs](../../../graph-theory.md#induced-subgraph). We write $K_a(b)$ for the [balanced complete multipartite blow-up](../../../graph-theory.md#balanced-complete-multipartite-blow-up) with $a$ classes of $b$ [vertices](../../../graph.md#vertex-graph-theory) each. All asymptotic errors below concern $n\to\infty$ with the forbidden [graphs](../../../graph.md) fixed.

**The stability subgraph.** We prove the [high-minimum-degree multipartite stability subgraph](../../../graph-theory.md#high-minimum-degree-multipartite-stability-subgraph) assertion directly from the [Erdős-Stone theorem](../../../graph-theory.md#erdos-stone-theorem). For $r=1$, the edgeless spanning [subgraph](../../../graph-theory.md#subgraph) suffices. Suppose $r\geq2$.

First repeatedly remove a [vertex](../../../graph.md#vertex-graph-theory) whose [degree of a vertex](../../../graph-theory.md#degree-graph-theory) is less than $(\alpha-\varepsilon_n)$ times the current order, where $\varepsilon_n\to0$ sufficiently slowly. The [Erdős-Stone theorem](../../../graph-theory.md#erdos-stone-theorem) gives, uniformly for every $K_{r+1}(t)$-free [subgraph](../../../graph-theory.md#subgraph) $J$ of order at most $n$,

$$
e(J)\leq\frac\alpha2|J|^2+\eta_n n^2,\qquad \eta_n\to0.
$$

Indeed, apply the asymptotic bound at large orders; the contribution from bounded or sufficiently small orders is negligible relative to $n^2$. If $m$ [vertices](../../../graph.md#vertex-graph-theory) survive, the removed [edges](../../../graph-theory.md#edge-of-a-graph) number at most

$$
(\alpha-\varepsilon_n)\sum_{j=m+1}^n j
=\frac{\alpha-\varepsilon_n}{2}(n^2-m^2)+O(n).
$$

Comparing with $e(G_n)=\alpha n^2/2+o(n^2)$ shows that $\varepsilon_n(n^2-m^2)=o(\varepsilon_n n^2)$, provided $\varepsilon_n$ dominates $\eta_n$, the initial relative error, and $1/n$. Consequently $m=n-o(n)$. The surviving [induced subgraph](../../../graph-theory.md#induced-subgraph) $G'$ satisfies $\delta(G')\geq(\alpha-o(1))m$ and $e(G')=\alpha m^2/2+o(m^2)$.

By the [Erdős-Stone theorem](../../../graph-theory.md#erdos-stone-theorem), $G'$ contains $K_r(L)$ for some $L=L_n\to\infty$ as slowly as necessary. This follows because $\alpha$ exceeds the [extremal number](../../../graph-theory.md#extremal-number) density for each fixed $K_r(L)$ by the positive gap $1/(r(r-1))$. Choose $L$ so slowly that $rL=o(m)$ and $\binom Lt^r=o(m)$, and denote its root classes by $A_1,\ldots,A_r$.

An outside [vertex](../../../graph.md#vertex-graph-theory) having at least $t$ [neighbours of a vertex](../../../graph-theory.md#neighbour-of-a-vertex) in every $A_i$ determines one choice of a $t$-subset in each $A_i$. At most $t-1$ outside [vertices](../../../graph.md#vertex-graph-theory) can determine any fixed choice, since otherwise these [vertices](../../../graph.md#vertex-graph-theory) and the chosen root sets form $K_{r+1}(t)$. Thus at most $(t-1)\binom Lt^r=o(m)$ outside [vertices](../../../graph.md#vertex-graph-theory) have this property. Exclude those [vertices](../../../graph.md#vertex-graph-theory) and the root classes; put each remaining [vertex](../../../graph.md#vertex-graph-theory) in a class $C_i$ for which it has fewer than $t$ [neighbours of a vertex](../../../graph-theory.md#neighbour-of-a-vertex) in $A_i$.

Write $\delta(G')\geq(\alpha-\gamma_n)m$, with $\gamma_n\to0$. Counting missing incidences with $A_i$ gives

$$
(L-t+1)|C_i|\leq\sum_{u\in A_i}(m-d(u))\leq L(1/r+\gamma_n)m.
$$

Since $\sum_i|C_i|=m-o(m)$, it follows that $|C_i|=m/r+o(m)$ for every $i$. The total missing incidences from all root [vertices](../../../graph.md#vertex-graph-theory) to assigned [vertices](../../../graph.md#vertex-graph-theory) are at most $(1+r\gamma_n)Lm$. At least $(L-t+1)(m-o(m))$ of them are incidences with a [vertex](../../../graph.md#vertex-graph-theory)'s own assigned root class. Hence only $o(Lm)$ missing incidences go to other root classes.

Choose $\rho_n\to0$ slowly and discard the $o(m)$ assigned [vertices](../../../graph.md#vertex-graph-theory) with more than $\rho_n L$ missing incidences to other root classes. Each remaining [vertex](../../../graph.md#vertex-graph-theory) of $C_i$ is adjacent to all but at most $\rho_n L$ [vertices](../../../graph.md#vertex-graph-theory) of every $A_j$, $j\ne i$. If its class contained a [complete bipartite graph](../../../graph-theory.md#complete-bipartite-graph) $K_{t,t}$, the $2t$ [vertices](../../../graph.md#vertex-graph-theory) of this copy would have at least $L-2t\rho_n L\geq t$ common [neighbours of a vertex](../../../graph-theory.md#neighbour-of-a-vertex) in each other root class. These sets extend the copy to $K_{r+1}(t)$, a contradiction. By the bipartite case of the [Erdős-Stone theorem](../../../graph-theory.md#erdos-stone-theorem), the number of internal [edges](../../../graph-theory.md#edge-of-a-graph) in each surviving class is $o(m^2)$.

The surviving [graph](../../../graph.md) still has $\alpha m^2/2+o(m^2)$ [edges](../../../graph-theory.md#edge-of-a-graph), whereas the total possible cross-class [edges](../../../graph-theory.md#edge-of-a-graph), with these balanced classes, is $\alpha m^2/2+o(m^2)$. Thus only $o(m^2)$ cross-class [edges](../../../graph-theory.md#edge-of-a-graph) are missing. Discard the $o(m)$ [vertices](../../../graph.md#vertex-graph-theory) missing more than $\sigma_n m$ cross-class [edges](../../../graph-theory.md#edge-of-a-graph), with $\sigma_n\to0$ slowly, and delete all internal [edges](../../../graph-theory.md#edge-of-a-graph). The resulting $r$-partite [subgraph](../../../graph-theory.md#subgraph) $H$ has classes $H_i$ of size $n/r+o(n)$ and

$$
\boxed{|H|=n-o(n),\qquad \delta(H)=(1-1/r+o(1))n.}
$$

For the lower bound, every surviving [vertex](../../../graph.md#vertex-graph-theory) misses only $o(n)$ [vertices](../../../graph.md#vertex-graph-theory) outside its class; the upper bound follows from the class sizes. This also records the uniform cross-class error that we need next.

**Minimum degree in an extremal graph.** Fix $F$ with $\chi(F)=r+1$. Choose $t$ large enough that $F$ embeds in $K_{r+1}(t)$. An extremal $F$-free [graph](../../../graph.md) $G$ is therefore $K_{r+1}(t)$-free, and its [edge](../../../graph-theory.md#edge-of-a-graph) count has the required asymptotics by the [Erdős-Stone theorem](../../../graph-theory.md#erdos-stone-theorem). For $r\geq2$ take $H$ as above.

For any [vertex](../../../graph.md#vertex-graph-theory) $v$, remove $v$ and introduce a new [vertex](../../../graph.md#vertex-graph-theory) $v^*$ whose [vertex neighbourhood](../../../graph.md#vertex-neighbourhood) consists precisely of the [vertices](../../../graph.md#vertex-graph-theory) in $H_2\cup\cdots\cup H_r$ other than $v$. The new [degree of a vertex](../../../graph-theory.md#degree-graph-theory) is $\alpha n-o(n)$. This new [graph](../../../graph.md) remains $F$-free. Indeed, a new copy of $F$ must use $v^*$, and all its [neighbours of a vertex](../../../graph-theory.md#neighbour-of-a-vertex) in that copy lie in the other classes of $H$. There are only boundedly many of them. Each misses only $o(n)$ [vertices](../../../graph.md#vertex-graph-theory) in $H_1$, so an unused [vertex](../../../graph.md#vertex-graph-theory) $w\in H_1$ is adjacent to all of them. Replacing $v^*$ by $w$ would give $F$ in $G-v$, which is impossible.

Extremality now forces $d_G(v)\geq\alpha n-o(n)$, uniformly in $v$. The upper bound for the [minimum degree of a graph](../../../graph-theory.md#minimum-degree-of-a-graph) follows from $\delta(G)\leq2e(G)/n$. For $r=1$, $e(G)=o(n^2)$ already gives $0\leq\delta(G)=o(n)$. Thus

$$
\boxed{\delta(G)=(1-1/r+o(1))n.}
$$

This is the [minimum degree of an extremal forbidden-subgraph graph](../../../graph-theory.md#minimum-degree-of-an-extremal-forbidden-subgraph-graph) principle.

**The exact extremal graph for disjoint cliques.** Define

$$
J_s(n)=K_{s-1}+T_r(n-s+1),\qquad
b_s(n)=\binom{s-1}{2}+(s-1)(n-s+1)+e(T_r(n-s+1)).
$$

The plus sign denotes the [join of graphs](../../../graph-theory.md#join-graph-theory). The [Turán graph](../../../graph-theory.md#turan-graph) contains no $K_{r+1}$, so every such [clique](../../../graph-theory.md#clique-graph-theory) in $J_s(n)$ uses a [vertex](../../../graph.md#vertex-graph-theory) of $K_{s-1}$. Therefore $J_s(n)$ contains no $s$ vertex-disjoint such [cliques](../../../graph-theory.md#clique-graph-theory), and the [extremal number](../../../graph-theory.md#extremal-number) is at least $b_s(n)$.

Induct on $s$, with $s=1$ supplied by the [Turan theorem](../../../graph-theory.md#turan-s-theorem), including its equality characterization. Let $s\geq2$ and let $G$ be extremal for $sK_{r+1}$. The preceding results give $\delta(G)\geq\alpha n-o(n)$ and the $r$-partite [subgraph](../../../graph-theory.md#subgraph) $H$. Keep its classes $H_i$ fixed and assign each of the remaining $o(n)$ [vertices](../../../graph.md#vertex-graph-theory) to a class in which it has fewest [neighbours of a vertex](../../../graph-theory.md#neighbour-of-a-vertex) in $H$. Write the resulting classes as $C_i$; all have size $n/r+o(n)$. Choose a positive $\tau_n\to0$ so slowly that $\tau_n n$ dominates the outside count, every cross-class error in $H$, and every error in the [minimum degree of a graph](../../../graph-theory.md#minimum-degree-of-a-graph) bound.

Suppose some [vertex](../../../graph.md#vertex-graph-theory) $x\in C_i$ has at least $\tau_n n$ internal [neighbours of a vertex](../../../graph-theory.md#neighbour-of-a-vertex). If $x\notin H$, the assignment rule shows that $x$ has at least $\tau_n n-o(n)$ [neighbours of a vertex](../../../graph-theory.md#neighbour-of-a-vertex) in every $H_j$. If $x\in H_i$, it has this many in $H_i$ and $n/r-o(n)$ in the other $H_j$. If $G-x$ contained $s-1$ disjoint $K_{r+1}$, we could choose one [vertex](../../../graph.md#vertex-graph-theory) in each $N(x)\cap H_j$, successively avoiding those copies and the $o(n)$ missing cross-neighbours of the already chosen [vertices](../../../graph.md#vertex-graph-theory). This produces a further $K_{r+1}$ through $x$. For $r=1$, this just chooses an unused neighbour of $x$. Hence $G-x$ is $(s-1)K_{r+1}$-free, and induction gives

$$
e(G)\leq b_{s-1}(n-1)+(n-1)=b_s(n).
$$

Since the candidate attains $b_s(n)$, equality holds throughout: $x$ is a [universal vertex](../../../graph-theory.md#universal-vertex) and $G-x$ is the inductively unique extremal [graph](../../../graph.md). Thus $G$ is isomorphic to $J_s(n)$.

It remains to show that this case must occur. Otherwise all internal [vertex degrees](../../../graph-theory.md#degree-graph-theory) are less than $\tau_n n=o(n)$. Together with the lower bound on $\delta(G)$ and $|C_i|=n/r+o(n)$, this implies that every [vertex](../../../graph.md#vertex-graph-theory) misses only $o(n)$ [vertices](../../../graph.md#vertex-graph-theory) outside its own class. If some $C_i$ contains a [matching in a graph](../../../graph-theory.md#matching-graph-theory) of $s$ [edges](../../../graph-theory.md#edge-of-a-graph), extend its [edges](../../../graph-theory.md#edge-of-a-graph) one by one to $K_{r+1}$, choosing one [vertex](../../../graph.md#vertex-graph-theory) from each other class. At every step only $o(n)$ cross-neighbours and boundedly many used [vertices](../../../graph.md#vertex-graph-theory) are excluded. This gives $s$ disjoint forbidden [cliques](../../../graph-theory.md#clique-graph-theory), a contradiction.

A [maximal matching](../../../graph-theory.md#maximal-matching) in each class therefore has at most $s-1$ [edges](../../../graph-theory.md#edge-of-a-graph), and its at most $2(s-1)$ endpoints form a [vertex cover](../../../graph-theory.md#vertex-cover) of the internal [edges](../../../graph-theory.md#edge-of-a-graph). Their internal [vertex degrees](../../../graph-theory.md#degree-graph-theory) are all $o(n)$, so the total internal [edge](../../../graph-theory.md#edge-of-a-graph) count is $o(n)$. The cross-class [edge](../../../graph-theory.md#edge-of-a-graph) count is at most $e(T_r(n))$, whence

$$
e(G)\leq e(T_r(n))+o(n).
$$

But the balanced part sizes of the [Turán graph](../../../graph-theory.md#turan-graph) give

$$
b_s(n)-e(T_r(n))=\frac{s-1}{r}n+O(1),
$$

contradicting extremality for $s\geq2$. This argument also works for $r=1$. Consequently, for all sufficiently large $n$,

$$
\boxed{\operatorname{ex}(n,sK_{r+1})=b_s(n),\quad G\cong K_{s-1}+T_r(n-s+1).}
$$

The uniqueness is up to [isomorphic graphs](../../../graph.md#graph-isomorphism), as usual for an [extremal graph for disjoint cliques](../../../graph-theory.md#extremal-graph-for-disjoint-cliques).

## 2

↑ **Parent:** [Paper 110](paper-110.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

**Symmetrization for an arbitrary real coefficient.** Among [graphs](../../../graph.md) maximizing $f(G)=e(G)-c k_3(G)$, choose one maximizing

$$
Q(G)=\sum_{x\in V(G)}d(x)^2.
$$

For a [vertex](../../../graph.md#vertex-graph-theory) $x$, put $L(x)=d(x)-c e(G[N(x)])$. This is the contribution of [edges](../../../graph-theory.md#edge-of-a-graph) and [triangles in a graph](../../../graph.md#triangle-in-a-graph) containing $x$. If $u,v$ are nonadjacent, [Zykov symmetrization](../../../graph-theory.md#zykov-symmetrization) replacing $u$ by a clone of $v$ changes $f$ by $L(v)-L(u)$; the opposite replacement changes it by $L(u)-L(v)$. Maximality implies $L(u)=L(v)$, so both changes preserve $f$.

Let $S=N(v)\setminus N(u)$ and $T=N(u)\setminus N(v)$. In the first replacement the [vertex degrees](../../../graph-theory.md#degree-graph-theory) in $S$ increase by one and those in $T$ decrease by one; in the opposite replacement these changes reverse. The changes to $d(u)^2+d(v)^2$ cancel when the two replacements are added. Since $(d+1)^2+(d-1)^2-2d^2=2$,

$$
\Delta_{u\gets v}Q+\Delta_{v\gets u}Q=2(|S|+|T|).
$$

If the two [vertex neighbourhoods](../../../graph.md#vertex-neighbourhood) differ, one replacement increases $Q$, a contradiction. Thus every pair of nonadjacent [vertices](../../../graph.md#vertex-graph-theory) has the same [vertex neighbourhood](../../../graph.md#vertex-neighbourhood). Nonadjacency, with equality allowed, is an [equivalence relation](../../../set-theory.md#equivalence-relation): if $u$ and $v$ are nonadjacent and $v$ and $w$ are nonadjacent, their identical [vertex neighbourhoods](../../../graph.md#vertex-neighbourhood) forbid $uw$ as well. Its classes are [independent sets](../../../graph-theory.md#independent-set-graph-theory) and every cross-class [edge](../../../graph-theory.md#edge-of-a-graph) is present. Therefore

$$
\boxed{\text{some maximizer of }e(G)-c k_3(G)\text{ is complete multipartite}.}
$$

This [edge-triangle symmetrization](../../../graph-theory.md#edge-triangle-symmetrization) works for either sign of $c$.

**The exact supporting line.** For $n\geq3$, write

$$
e_2=e(T_2(n)),\quad e_3=e(T_3(n)),\quad t_3=k_3(T_3(n)),\quad c_*=(e_3-e_2)/t_3.
$$

We prove the [triangle support line between bipartite and tripartite Turan graphs](../../../graph-theory.md#triangle-support-line-between-bipartite-and-tripartite-turan-graphs) by maximizing $e-c_*k_3$. First $c_*\geq2/n$. For $n=3,4,5$, its values are respectively $1,1/2,1/2$. For $n\geq6$, the exact balancing of the [Turán graph](../../../graph-theory.md#turan-graph) gives $e_3\geq n^2/3-1/3$, while $e_2\leq n^2/4$ and the [arithmetic-geometric mean inequality](../../../mathematical-optimization.md#arithmetic-geometric-mean-inequality) gives $t_3\leq n^3/27$. Hence

$$
n(e_3-e_2)-2t_3\geq\frac{n^3}{108}-\frac n3\geq0.
$$

By [edge-triangle symmetrization](../../../graph-theory.md#edge-triangle-symmetrization) a maximizing [graph](../../../graph.md) can be taken [complete multipartite graph](../../../graph-theory.md#complete-multipartite-graph); among such maximizers use one with the fewest nonempty parts. If there are at least four parts, let $a,b$ be the two smallest sizes. Then $a+b\leq n/2$. Merging them loses $ab$ [edges](../../../graph-theory.md#edge-of-a-graph) and $ab(n-a-b)$ [triangles in a graph](../../../graph.md#triangle-in-a-graph), so the objective changes by

$$
ab\{c_*(n-a-b)-1\}\geq0.
$$

This contradicts the choice of the number of parts. Thus at most three parts remain.

For three part sizes $a\geq b\geq d>0$, the objective is

$$
ad(1-c_*b)+b(a+d).
$$

If $1-c_*b\leq0$, merging the parts of sizes $a,d$ does not decrease it, again contradicting minimality. If $1-c_*b>0$ and $a-d\geq2$, transferring one [vertex](../../../graph.md#vertex-graph-theory) from the largest to the smallest part raises $ad$ by $a-d-1>0$ and strictly increases the objective. Thus a three-part maximizer has all sizes differing by at most one, and is $T_3(n)$. A maximizer with at most two parts has objective at most $e_2$, since it has no [triangles in a graph](../../../graph.md#triangle-in-a-graph) and the [Mantel theorem](../../../graph-theory.md#mantel-theorem) bounds its [edges](../../../graph-theory.md#edge-of-a-graph). Finally,

$$
e(T_3(n))-c_*k_3(T_3(n))=e_2.
$$

Therefore every [graph](../../../graph.md) satisfies $e(G)-c_*k_3(G)\leq e_2$. At the prescribed [edge](../../../graph-theory.md#edge-of-a-graph) count this gives

$$
\boxed{k_3(G)\geq\theta k_3(T_3(n)).}
$$

For $n\leq2$, the conclusion is simply the nonnegative lower bound zero. All rounding in the [Turán graphs](../../../graph-theory.md#turan-graph) has been retained.

**One edge above the bipartite threshold.** Write $n=2m$. We prove the [Triangle lower bound one edge above the Mantel threshold](../../../graph-theory.md#triangle-lower-bound-one-edge-above-the-mantel-threshold) by induction on $m\geq2$, allowing at least $m^2+1$ [edges](../../../graph-theory.md#edge-of-a-graph). For $m=2$, five [edges](../../../graph-theory.md#edge-of-a-graph) on four [vertices](../../../graph.md#vertex-graph-theory) give two [triangles in a graph](../../../graph.md#triangle-in-a-graph), and adding [edges](../../../graph-theory.md#edge-of-a-graph) preserves this bound.

We will also use the following consequence of an inductive bound: on $2a$ [vertices](../../../graph.md#vertex-graph-theory), at least $a^2+q$ [edges](../../../graph-theory.md#edge-of-a-graph), for an integer $q\geq1$, force at least $a+q-1$ [triangles in a graph](../../../graph.md#triangle-in-a-graph). Delete surplus [edges](../../../graph-theory.md#edge-of-a-graph) first to leave exactly $a^2+q$. Repeatedly delete an [edge](../../../graph-theory.md#edge-of-a-graph) in a [triangle in a graph](../../../graph.md#triangle-in-a-graph) until $a^2+1$ [edges](../../../graph-theory.md#edge-of-a-graph) remain. The [Mantel theorem](../../../graph-theory.md#mantel-theorem) guarantees such a [triangle in a graph](../../../graph.md#triangle-in-a-graph) at every step; each deletion destroys at least one distinct [triangle in a graph](../../../graph.md#triangle-in-a-graph). Apply the inductive bound to the remaining [graph](../../../graph.md).

Now take exactly $m^2+1$ [edges](../../../graph-theory.md#edge-of-a-graph). If every [edge](../../../graph-theory.md#edge-of-a-graph) lies in a [triangle in a graph](../../../graph.md#triangle-in-a-graph), the [edge-triangle incidence bound](../../../graph.md#edge-triangle-incidence-bound) gives $3k_3(G)\geq m^2+1$. This is at least $3m$ for $m\geq3$; the base case was handled separately.

Otherwise choose an [edge](../../../graph-theory.md#edge-of-a-graph) $uv$ in no [triangle in a graph](../../../graph.md#triangle-in-a-graph). Its endpoints have disjoint [vertex neighbourhoods](../../../graph.md#vertex-neighbourhood), so $d(u)+d(v)\leq2m$. Deleting $u,v$ removes exactly $d(u)+d(v)-1$ [edges](../../../graph-theory.md#edge-of-a-graph) and leaves at least $(m-1)^2+1$ [edges](../../../graph-theory.md#edge-of-a-graph). If $d(u)+d(v)\leq2m-1$, it leaves at least $(m-1)^2+2$ [edges](../../../graph-theory.md#edge-of-a-graph), and the strengthened inductive bound gives at least $m$ [triangles in a graph](../../../graph.md#triangle-in-a-graph) already.

If $d(u)+d(v)=2m$, induction gives at least $m-1$ [triangles in a graph](../../../graph.md#triangle-in-a-graph) after deletion. There must be an additional [triangle in a graph](../../../graph.md#triangle-in-a-graph) containing $u$ or $v$. Otherwise both $N(u)$ and $N(v)$ are [independent sets](../../../graph-theory.md#independent-set-graph-theory); since they are disjoint and cover all [vertices](../../../graph.md#vertex-graph-theory), $G$ would be [bipartite graph](../../../graph-theory.md#bipartite-graph), contradicting $e(G)>m^2$ by the [Mantel theorem](../../../graph-theory.md#mantel-theorem). Hence

$$
\boxed{k_3(G)\geq m=n/2.}
$$

The bound is sharp: add one internal [edge](../../../graph-theory.md#edge-of-a-graph) to one class of the [complete bipartite graph](../../../graph-theory.md#complete-bipartite-graph) $K_{m,m}$. Its [triangles in a graph](../../../graph.md#triangle-in-a-graph) are precisely that [edge](../../../graph-theory.md#edge-of-a-graph) together with each of the $m$ [vertices](../../../graph.md#vertex-graph-theory) in the other class.

## 3

↑ **Parent:** [Paper 110](paper-110.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

**Statement and definitions.** For disjoint nonempty sets $A,B$ of [vertices](../../../graph.md#vertex-graph-theory), their [edge density of a bipartite graph](../../../probabilistic-combinatorics.md#edge-density-of-a-bipartite-graph) is $d(A,B)=e(A,B)/(|A||B|)$. They form a [regular pair of vertex sets](../../../probabilistic-combinatorics.md#regular-pair-of-vertex-sets), or an $\varepsilon$-uniform pair, if

$$
|d(X,Y)-d(A,B)|\leq\varepsilon
$$

whenever $X\subseteq A$, $Y\subseteq B$, $|X|\geq\varepsilon|A|$ and $|Y|\geq\varepsilon|B|$.

The [Szemerédi regularity lemma](../../../probabilistic-combinatorics.md#szemeredi-regularity-lemma) states that for every $\varepsilon>0$ and positive integer $m_0$, there are integers $M,n_0$ such that every [graph](../../../graph.md) of order $n\geq n_0$ has a [set partition](../../../combinatorics.md#set-partition)

$$
V(G)=V_0\sqcup V_1\sqcup\cdots\sqcup V_k
$$

with $m_0\leq k\leq M$, $|V_0|\leq\varepsilon n$, equal nonzero sizes $|V_1|=\cdots=|V_k|$, and at most $\varepsilon k^2$ unordered pairs $(V_i,V_j)$, $1\leq i<j\leq k$, that fail to be $\varepsilon$-uniform. It is enough to prove this for $0<\varepsilon\leq1/2$, since decreasing the parameter strengthens the conclusion.

**Energy increment.** For the proof, regard each exceptional [vertex](../../../graph.md#vertex-graph-theory) as a singleton part and use the [equitable regularity energy](../../../probabilistic-combinatorics.md#equitable-regularity-energy)

$$
q(\mathcal P)=\frac1{n^2}\sum_{A,B\in\mathcal P}|A||B|d(A,B)^2.
$$

The sum is over ordered pairs, including diagonal pairs; for those pairs define $d$ as the mean adjacency indicator on $A\times B$. Thus $0\leq q\leq1$. Under a refinement, the subrectangle densities have the original density as their weighted mean. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), equivalently the nonnegativity of their weighted [variance](../../../variance.md), gives $q(\mathcal P')\geq q(\mathcal P)$.

Suppose there are more than $\varepsilon k^2$ irregular pairs, with main cell size $m$. For each such pair choose witnesses $X\subseteq V_i$, $Y\subseteq V_j$ of sizes at least $\varepsilon m$ and with $|d(X,Y)-d(V_i,V_j)|>\varepsilon$. Refine every main cell by all its witness subsets. Each splits into at most $2^{k-1}$ atoms, and we may use the larger bound $2^k$.

For an ordered irregular rectangle, write its refined densities as $d_{ab}$ and relative areas as $w_{ab}$. The energy gain on that rectangle is

$$
\frac{m^2}{n^2}\sum_{a,b}w_{ab}(d_{ab}-d(V_i,V_j))^2.
$$

The witness rectangle has relative area at least $\varepsilon^2$. Applying the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) to the subrectangles it contains shows that this expression is greater than $\varepsilon^4m^2/n^2$. There are two orientations of each irregular pair. Since $km=n-|V_0|\geq n/2$, the total gain is greater than

$$
2\varepsilon^5\frac{k^2m^2}{n^2}\geq\varepsilon^5/2.
$$

**Restoring equal sizes without losing energy.** Put $\ell=\lfloor m/4^k\rfloor$, assuming $m\geq2\cdot4^k$. Split every refined atom into sets of size $\ell$, putting its leftover fewer than $\ell$ [vertices](../../../graph.md#vertex-graph-theory) into the exceptional set as singleton parts. This is a further refinement, so the energy cannot decrease. The number of new exceptional [vertices](../../../graph.md#vertex-graph-theory) is at most

$$
k2^k\ell\leq km/2^k\leq n/2^k.
$$

The number $k'$ of new main cells satisfies

$$
k\leq k'\leq\frac{km}{\ell}\leq2k4^k.
$$

For the first inequality, in each old cell the leftovers have total size less than $2^k\ell<m$, so at least one full chunk survives. All previous exceptional singleton parts are kept. Treating leftovers as singleton parts is what makes the energy increment survive equitabilization exactly.

Take $S=\lceil2\varepsilon^{-5}\rceil+1$ and choose $k_0\geq m_0$ so large that $S2^{-k_0}\leq\varepsilon/2$. Start with $k_0$ equal main cells, with fewer than $k_0$ exceptional [vertices](../../../graph.md#vertex-graph-theory). Define a finite bound $M$ by iterating $x\mapsto2x4^x$ a total of $S$ times, starting from $k_0$. Choose $n_0$ sufficiently large that $k_0\leq\varepsilon n/2$ and $n/(2M)\geq2\cdot4^M$ whenever $n\geq n_0$.

At each of the first $S$ refinements, the exceptional set has size at most

$$
k_0+S n2^{-k_0}\leq\varepsilon n,
$$

the cell count is between $k_0$ and $M$, and $m\geq n/(2M)$, so all the chunk sizes above are valid. But $S$ unsuccessful refinements would raise $q$ by more than $S\varepsilon^5/2>1$, which is impossible. Thus the procedure terminates at a partition satisfying the [Szemerédi regularity lemma](../../../probabilistic-combinatorics.md#szemeredi-regularity-lemma).

**Three linearly large uniform sets.** Apply the [Szemerédi regularity lemma](../../../probabilistic-combinatorics.md#szemeredi-regularity-lemma) with

$$
\varepsilon=10^{-5},\qquad m_0=1000,\qquad d_0=10^{-3}.
$$

For $n\geq n_0$, delete all [edges](../../../graph-theory.md#edge-of-a-graph) touching $V_0$, all internal main-cell [edges](../../../graph-theory.md#edge-of-a-graph), all [edges](../../../graph-theory.md#edge-of-a-graph) of irregular pairs, and all [edges](../../../graph-theory.md#edge-of-a-graph) of regular pairs whose [edge density of a bipartite graph](../../../probabilistic-combinatorics.md#edge-density-of-a-bipartite-graph) is less than $d_0$. The respective losses are bounded by

$$
\varepsilon n^2,\qquad \frac{n^2}{2m_0},\qquad \varepsilon n^2,\qquad \frac{d_0n^2}{2}.
$$

Thus the total loss is at most $0.00102n^2$, and the remaining [graph](../../../graph.md) has at least

$$
(0.255-0.00102)n^2=0.25398n^2>n^2/4
$$

[edges](../../../graph-theory.md#edge-of-a-graph). Form the [reduced graph of a regularity partition](../../../probabilistic-combinatorics.md#reduced-graph-of-a-regularity-partition) $R$, joining two main cells precisely when they are $\varepsilon$-uniform and have [edge density of a bipartite graph](../../../probabilistic-combinatorics.md#edge-density-of-a-bipartite-graph) at least $d_0$. If their common size is $m$, the remaining [edge](../../../graph-theory.md#edge-of-a-graph) count is at most $e(R)m^2$. Since $km\leq n$, we obtain $e(R)>k^2/4$. The [Mantel theorem](../../../graph-theory.md#mantel-theorem) gives a [triangle in a graph](../../../graph.md#triangle-in-a-graph) in $R$. Its three cells $U_1,U_2,U_3$ have the required pairwise density and are $10^{-3}$-uniform: an $\varepsilon$-uniform pair is uniform for any larger parameter.

Each selected cell has size $m\geq(1-\varepsilon)n/M$. Choose

$$
c=\min\left\{\frac{1-\varepsilon}{2M},\frac1{n_0}\right\}>0.
$$

For $n<n_0$, the [Mantel theorem](../../../graph-theory.md#mantel-theorem) gives a [triangle in a graph](../../../graph.md#triangle-in-a-graph) in the original [graph](../../../graph.md), since its [edge](../../../graph-theory.md#edge-of-a-graph) count exceeds $n^2/4$; take its three singleton [vertices](../../../graph.md#vertex-graph-theory). Their pairs have density one and are uniform for every positive parameter, and $1>cn$. Therefore in all cases

$$
\boxed{|U_i|>cn,\quad (U_i,U_j)\text{ is }10^{-3}\text{-uniform},\quad d(U_i,U_j)\geq10^{-3}.}
$$

The constant is absolute; the energy proof gives a very large bound for $M$, which does not affect its positivity.

## 4

↑ **Parent:** [Paper 110](paper-110.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use natural logarithms. A $K_t$ [graph minor](../../../graph-theory.md#graph-minor) is represented by $t$ disjoint nonempty [branch sets of a graph minor](../../../graph-theory.md#branch-set-of-a-graph-minor), each inducing a [connected graph](../../../graph.md#connected-graph), with an [edge](../../../graph-theory.md#edge-of-a-graph) between every pair. The [complete graph minor density threshold](../../../graph-theory.md#complete-graph-minor-density-threshold) is defined over nonempty finite [graphs](../../../graph.md) by

$$
c(t)=\inf\{c:\text{for every nonempty finite }G,\ e(G)\geq c|G|\Longrightarrow G\succ K_t\}.
$$

It uses $e(G)/|G|$, half the average [degree of a vertex](../../../graph-theory.md#degree-graph-theory); the nonempty convention excludes the vacuous density inequality for the empty [graph](../../../graph.md). The PDF has the intended definition with a universal implication over $G$; the TeX transcription corrupts that definition.

**Probabilistic lower bound.** Put $N=\lfloor t\sqrt{\log t}/4\rfloor$ and take the [binomial random graph](../../../graph-theory.md#binomial-random-graph) $G(N,1/2)$. Its [edge](../../../graph-theory.md#edge-of-a-graph) count has mean $N(N-1)/4$. The [Chernoff bound](../../../probability-inequality.md#chernoff-bound) implies

$$
\mathbb P(e(G)\geq N^2/8)\longrightarrow1.
$$

We show that the [probability](../../../probability-theory.md#probability) of a $K_t$ [graph minor](../../../graph-theory.md#graph-minor) tends to zero. Ignore connectedness, which only enlarges the set of possible models, and assign each of the $N$ [vertices](../../../graph.md#vertex-graph-theory) one of $t$ branch labels or an unused label. There are at most $(t+1)^N$ assignments.

For any assignment with $t$ nonempty branch sets, at least $t/2$ of them have size at most $2N/t\leq\sqrt{\log t}/2$. Between any two such small sets $A,B$, the [probability](../../../probability-theory.md#probability) of no [edge](../../../graph-theory.md#edge-of-a-graph) is

$$
2^{-|A||B|}\geq \exp\left(-\frac{\log2}{4}\log t\right)\geq t^{-1/4}.
$$

The absence or presence of [edges](../../../graph-theory.md#edge-of-a-graph) between different pairs of branch sets depends on disjoint sets of random [edges](../../../graph-theory.md#edge-of-a-graph), so these events are independent. For this assignment the [probability](../../../probability-theory.md#probability) that all small pairs are adjacent is at most

$$
(1-t^{-1/4})^{\binom{\lfloor t/2\rfloor}{2}}
\leq\exp\left(-\binom{\lfloor t/2\rfloor}{2}t^{-1/4}\right).
$$

The [union bound](../../../probability-inequality.md#boole-s-inequality) over assignments is therefore at most

$$
\exp\left(N\log(t+1)-\binom{\lfloor t/2\rfloor}{2}t^{-1/4}\right)\longrightarrow0,
$$

since the positive term is $O(t(\log t)^{3/2})$ and the negative term has order $t^{7/4}$. There is consequently a [graph](../../../graph.md) with no $K_t$ [graph minor](../../../graph-theory.md#graph-minor) and with $e(G)/N\geq N/8$. Any constant having the universal forcing property must exceed this ratio. Since $N/8\geq t\sqrt{\log t}/64$ for large $t$,

$$
\boxed{c(t)\geq\beta t\sqrt{\log t}\quad\text{with }\beta=1/64.}
$$

**The auxiliary density lemma contains a typo.** Both the original PDF and the TeX print $e(G)\leq11k|G|$ in the hint. This cannot imply its conclusion: for $k\geq1$, an edgeless [graph](../../../graph.md) has only edgeless [graph minors](../../../graph-theory.md#graph-minor), and none satisfies $2\delta(H)\geq|H|+4k-1$. We use the intended [dense minor with bounded order and high minimum degree](../../../graph-theory.md#dense-minor-with-bounded-order-and-high-minimum-degree) lemma with the hypothesis $e(G)\geq11k|G|$ for nonempty $G$. The upper-bound argument below depends on that corrected supplied lemma; the literal printed hint is false.

**Probabilistic upper bound and the constant seven.** Suppose $G$ is nonempty and $e(G)\geq7t\sqrt{\log t}|G|$, and set

$$
k=\left\lfloor\frac7{11}t\sqrt{\log t}\right\rfloor,\qquad
\ell=\lceil\sqrt{\log t}\rceil.
$$

The corrected lemma gives a [graph minor](../../../graph-theory.md#graph-minor) $H$ of order $N\leq11k+2$ with $2\delta(H)\geq N+4k-1$. Since $\delta(H)\leq N-1$, we also have $N\geq4k+1$. For large $k$, every [vertex](../../../graph.md#vertex-graph-theory) has at most $N/3$ nonneighbours, counting itself, because

$$
N-\delta(H)\leq N/2-2k+1/2\leq N/3;
$$

the last inequality uses $N\leq11k+2\leq12k-3$. Moreover any two distinct [vertices](../../../graph.md#vertex-graph-theory) have at least

$$
2\delta(H)-N\geq4k-1
$$

[common neighbours](../../../graph-theory.md#common-neighbour).

Choose $2t$ disjoint random $\ell$-sets $A_1,\ldots,A_{2t}$ from $V(H)$, uniformly, which is possible since $2t\ell<4k-1\leq N$ for sufficiently large $t$. For a set $A$, let $U(A)$ be the set of [vertices](../../../graph.md#vertex-graph-theory) having no neighbour in $A$. For each [vertex](../../../graph.md#vertex-graph-theory), the [probability](../../../probability-theory.md#probability) that all members of a uniformly sampled $\ell$-set are its nonneighbours is at most $3^{-\ell}$, even when sampling without replacement. By linearity of [expected value](../../../probability-theory.md#expected-value),

$$
\mathbb E|U(A)|\leq N3^{-\ell}.
$$

Call $A$ good if $|U(A)|\leq N3^{-19\ell/20}$. The [Markov inequality](../../../probability-inequality.md#markov-inequality) shows that a random set is bad with [probability](../../../probability-theory.md#probability) at most $3^{-\ell/20}=o(1)$. Thus the expected number of bad sets among our $2t$ samples is $o(t)$.

Conditional on a fixed good $A_i$, the marginal distribution of $A_j$ is uniform among $\ell$-sets outside $A_i$. For there to be no [edge](../../../graph-theory.md#edge-of-a-graph) between them, all its members must lie in $U(A_i)$. Hence

$$
\mathbb P(A_i\text{ good and }e(A_i,A_j)=0)
\leq\left(\frac{N3^{-19\ell/20}}{N-\ell}\right)^\ell.
$$

Here $(N/(N-\ell))^\ell=\exp(O(\ell^2/N))=1+o(1)$. Consequently the expected number of nonadjacent pairs of good sets is at most

$$
\binom{2t}{2}(1+o(1))3^{-19\ell^2/20}
=O\left(t^{2-(19/20)\log3}\right)=o(t),
$$

since $(19/20)\log3>1$. Applying the [Markov inequality](../../../probability-inequality.md#markov-inequality) to both counts shows that there exists a choice with fewer than $t$ bad sets and at most $t$ nonadjacent pairs of good sets. Select $t$ of the good sets; they still have at most $t$ missing adjacencies.

Make each selected set connected by fixing one of its [vertices](../../../graph.md#vertex-graph-theory) as a root and, for each of its other members, adding one unused [common neighbour](../../../graph-theory.md#common-neighbour) of that member and the root. This uses at most $t(\ell-1)$ additional [vertices](../../../graph.md#vertex-graph-theory). Then for each pair with no original [edge](../../../graph-theory.md#edge-of-a-graph), choose one [vertex](../../../graph.md#vertex-graph-theory) in each set and add an unused [common neighbour](../../../graph-theory.md#common-neighbour) to one of the sets. The added [vertex](../../../graph.md#vertex-graph-theory) is joined to that set and to the other set, so it preserves connectedness and repairs their adjacency. At most $t$ such repairs are required.

Throughout this process the total number of occupied [vertices](../../../graph.md#vertex-graph-theory) is at most

$$
t\ell+t(\ell-1)+t=2t\ell<4k-1.
$$

Since every pair has at least $4k-1$ [common neighbours](../../../graph-theory.md#common-neighbour), an unused choice always exists. The final sets are disjoint connected [branch sets of a graph minor](../../../graph-theory.md#branch-set-of-a-graph-minor) with every pair adjacent. They represent $K_t$ in $H$, and hence in $G$, by transitivity of [graph minors](../../../graph-theory.md#graph-minor). This [random branch-set construction of a complete graph minor](../../../graph-theory.md#random-branch-set-construction-of-a-complete-graph-minor) proves

$$
\boxed{c(t)\leq7t\sqrt{\log t}\quad\text{for sufficiently large }t.}
$$

**The sharp linear threshold for a four-vertex complete minor.** We prove by induction that a [graph](../../../graph.md) on $n\geq4$ [vertices](../../../graph.md#vertex-graph-theory) with at least $2n-2$ [edges](../../../graph-theory.md#edge-of-a-graph) has a $K_4$ [graph minor](../../../graph-theory.md#graph-minor). The case $n=4$ is $K_4$ itself. If some [edge](../../../graph-theory.md#edge-of-a-graph) $uv$ has at most one [common neighbour](../../../graph-theory.md#common-neighbour), an [edge contraction](../../../graph-theory.md#edge-contraction) reduces the order by one and removes exactly $1+|N(u)\cap N(v)|\leq2$ [edges](../../../graph-theory.md#edge-of-a-graph). The contracted [graph](../../../graph.md) has at least $2(n-1)-2$ [edges](../../../graph-theory.md#edge-of-a-graph), so induction applies.

Otherwise every [edge](../../../graph-theory.md#edge-of-a-graph) is in at least two [triangles in a graph](../../../graph.md#triangle-in-a-graph). Choose a [vertex](../../../graph.md#vertex-graph-theory) $v$ incident with an [edge](../../../graph-theory.md#edge-of-a-graph). Each [vertex](../../../graph.md#vertex-graph-theory) $u\in N(v)$ has at least two [neighbours of a vertex](../../../graph-theory.md#neighbour-of-a-vertex) in $N(v)$, since these are the [common neighbours](../../../graph-theory.md#common-neighbour) of $u,v$. Thus $G[N(v)]$ has [minimum degree of a graph](../../../graph-theory.md#minimum-degree-of-a-graph) at least two. A longest path in this finite [graph](../../../graph.md) has an endpoint adjacent to an earlier nonconsecutive path [vertex](../../../graph.md#vertex-graph-theory), and hence contains a [cycle in a graph](../../../graph-theory.md#cycle-in-a-graph). Together with $v$, this [cycle in a graph](../../../graph-theory.md#cycle-in-a-graph) gives a [wheel graph](../../../graph-theory.md#wheel-graph) as a [subgraph](../../../graph-theory.md#subgraph). Divide its rim into three consecutive nonempty connected arcs; these arcs and $\{v\}$ form four pairwise adjacent [branch sets of a graph minor](../../../graph-theory.md#branch-set-of-a-graph-minor). Therefore

$$
\boxed{e(G)\geq2n-2\ \Longrightarrow\ G\succ K_4.}
$$

With $2n-3$ [edges](../../../graph-theory.md#edge-of-a-graph) the answer is **no**. Take the [join of graphs](../../../graph-theory.md#join-graph-theory) of $K_2$ and an [independent set](../../../graph-theory.md#independent-set-graph-theory) of $n-2$ [vertices](../../../graph.md#vertex-graph-theory). It has $1+2(n-2)=2n-3$ [edges](../../../graph-theory.md#edge-of-a-graph). Among four disjoint putative [branch sets of a graph minor](../../../graph-theory.md#branch-set-of-a-graph-minor), at most two can contain the two [vertices](../../../graph.md#vertex-graph-theory) of $K_2$. Any connected branch set avoiding them is a singleton in the [independent set](../../../graph-theory.md#independent-set-graph-theory). At least two such singleton sets would therefore have no [edge](../../../graph-theory.md#edge-of-a-graph) between them. This excludes a $K_4$ [graph minor](../../../graph-theory.md#graph-minor) for every $n\geq4$ and proves sharpness.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
