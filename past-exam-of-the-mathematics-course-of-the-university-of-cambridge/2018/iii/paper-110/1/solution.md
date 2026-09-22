<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $\alpha=1-1/r$. The [Erdős-Stone theorem](../../../../../erdos-stone-theorem.md) states that, for a fixed [graph](../../../../../graph-split.md) $F$ with [chromatic number](../../../../../chromatic-number.md) $\chi(F)=r+1\geq2$,

$$
\boxed{\operatorname{ex}(n,F)=\left(1-\frac1r+o(1)\right)\binom n2.}
$$

Here $\operatorname{ex}$ is the [extremal number](../../../../../extremal-number.md), and copies are [subgraphs](../../../../../subgraph.md), not necessarily [induced subgraphs](../../../../../induced-subgraph.md). We write $K_a(b)$ for the [balanced complete multipartite blow-up](../../../../../balanced-complete-multipartite-blow-up.md) with $a$ classes of $b$ [vertices](../../../../../vertex-graph-theory.md) each. All asymptotic errors below concern $n\to\infty$ with the forbidden [graphs](../../../../../graph-split.md) fixed.

**The stability subgraph.** We prove the [high-minimum-degree multipartite stability subgraph](../../../../../high-minimum-degree-multipartite-stability-subgraph.md) assertion directly from the [Erdős-Stone theorem](../../../../../erdos-stone-theorem.md). For $r=1$, the edgeless spanning [subgraph](../../../../../subgraph.md) suffices. Suppose $r\geq2$.

First repeatedly remove a [vertex](../../../../../vertex-graph-theory.md) whose [degree of a vertex](../../../../../degree-graph-theory.md) is less than $(\alpha-\varepsilon_n)$ times the current order, where $\varepsilon_n\to0$ sufficiently slowly. The [Erdős-Stone theorem](../../../../../erdos-stone-theorem.md) gives, uniformly for every $K_{r+1}(t)$-free [subgraph](../../../../../subgraph.md) $J$ of order at most $n$,

$$
e(J)\leq\frac\alpha2|J|^2+\eta_n n^2,\qquad \eta_n\to0.
$$

Indeed, apply the asymptotic bound at large orders; the contribution from bounded or sufficiently small orders is negligible relative to $n^2$. If $m$ [vertices](../../../../../vertex-graph-theory.md) survive, the removed [edges](../../../../../edge-of-a-graph.md) number at most

$$
(\alpha-\varepsilon_n)\sum_{j=m+1}^n j
=\frac{\alpha-\varepsilon_n}{2}(n^2-m^2)+O(n).
$$

Comparing with $e(G_n)=\alpha n^2/2+o(n^2)$ shows that $\varepsilon_n(n^2-m^2)=o(\varepsilon_n n^2)$, provided $\varepsilon_n$ dominates $\eta_n$, the initial relative error, and $1/n$. Consequently $m=n-o(n)$. The surviving [induced subgraph](../../../../../induced-subgraph.md) $G'$ satisfies $\delta(G')\geq(\alpha-o(1))m$ and $e(G')=\alpha m^2/2+o(m^2)$.

By the [Erdős-Stone theorem](../../../../../erdos-stone-theorem.md), $G'$ contains $K_r(L)$ for some $L=L_n\to\infty$ as slowly as necessary. This follows because $\alpha$ exceeds the [extremal number](../../../../../extremal-number.md) density for each fixed $K_r(L)$ by the positive gap $1/(r(r-1))$. Choose $L$ so slowly that $rL=o(m)$ and $\binom Lt^r=o(m)$, and denote its root classes by $A_1,\ldots,A_r$.

An outside [vertex](../../../../../vertex-graph-theory.md) having at least $t$ [neighbours of a vertex](../../../../../neighbour-of-a-vertex.md) in every $A_i$ determines one choice of a $t$-subset in each $A_i$. At most $t-1$ outside [vertices](../../../../../vertex-graph-theory.md) can determine any fixed choice, since otherwise these [vertices](../../../../../vertex-graph-theory.md) and the chosen root sets form $K_{r+1}(t)$. Thus at most $(t-1)\binom Lt^r=o(m)$ outside [vertices](../../../../../vertex-graph-theory.md) have this property. Exclude those [vertices](../../../../../vertex-graph-theory.md) and the root classes; put each remaining [vertex](../../../../../vertex-graph-theory.md) in a class $C_i$ for which it has fewer than $t$ [neighbours of a vertex](../../../../../neighbour-of-a-vertex.md) in $A_i$.

Write $\delta(G')\geq(\alpha-\gamma_n)m$, with $\gamma_n\to0$. Counting missing incidences with $A_i$ gives

$$
(L-t+1)|C_i|\leq\sum_{u\in A_i}(m-d(u))\leq L(1/r+\gamma_n)m.
$$

Since $\sum_i|C_i|=m-o(m)$, it follows that $|C_i|=m/r+o(m)$ for every $i$. The total missing incidences from all root [vertices](../../../../../vertex-graph-theory.md) to assigned [vertices](../../../../../vertex-graph-theory.md) are at most $(1+r\gamma_n)Lm$. At least $(L-t+1)(m-o(m))$ of them are incidences with a [vertex](../../../../../vertex-graph-theory.md)'s own assigned root class. Hence only $o(Lm)$ missing incidences go to other root classes.

Choose $\rho_n\to0$ slowly and discard the $o(m)$ assigned [vertices](../../../../../vertex-graph-theory.md) with more than $\rho_n L$ missing incidences to other root classes. Each remaining [vertex](../../../../../vertex-graph-theory.md) of $C_i$ is adjacent to all but at most $\rho_n L$ [vertices](../../../../../vertex-graph-theory.md) of every $A_j$, $j\ne i$. If its class contained a [complete bipartite graph](../../../../../complete-bipartite-graph.md) $K_{t,t}$, the $2t$ [vertices](../../../../../vertex-graph-theory.md) of this copy would have at least $L-2t\rho_n L\geq t$ common [neighbours of a vertex](../../../../../neighbour-of-a-vertex.md) in each other root class. These sets extend the copy to $K_{r+1}(t)$, a contradiction. By the bipartite case of the [Erdős-Stone theorem](../../../../../erdos-stone-theorem.md), the number of internal [edges](../../../../../edge-of-a-graph.md) in each surviving class is $o(m^2)$.

The surviving [graph](../../../../../graph-split.md) still has $\alpha m^2/2+o(m^2)$ [edges](../../../../../edge-of-a-graph.md), whereas the total possible cross-class [edges](../../../../../edge-of-a-graph.md), with these balanced classes, is $\alpha m^2/2+o(m^2)$. Thus only $o(m^2)$ cross-class [edges](../../../../../edge-of-a-graph.md) are missing. Discard the $o(m)$ [vertices](../../../../../vertex-graph-theory.md) missing more than $\sigma_n m$ cross-class [edges](../../../../../edge-of-a-graph.md), with $\sigma_n\to0$ slowly, and delete all internal [edges](../../../../../edge-of-a-graph.md). The resulting $r$-partite [subgraph](../../../../../subgraph.md) $H$ has classes $H_i$ of size $n/r+o(n)$ and

$$
\boxed{|H|=n-o(n),\qquad \delta(H)=(1-1/r+o(1))n.}
$$

For the lower bound, every surviving [vertex](../../../../../vertex-graph-theory.md) misses only $o(n)$ [vertices](../../../../../vertex-graph-theory.md) outside its class; the upper bound follows from the class sizes. This also records the uniform cross-class error that we need next.

**Minimum degree in an extremal graph.** Fix $F$ with $\chi(F)=r+1$. Choose $t$ large enough that $F$ embeds in $K_{r+1}(t)$. An extremal $F$-free [graph](../../../../../graph-split.md) $G$ is therefore $K_{r+1}(t)$-free, and its [edge](../../../../../edge-of-a-graph.md) count has the required asymptotics by the [Erdős-Stone theorem](../../../../../erdos-stone-theorem.md). For $r\geq2$ take $H$ as above.

For any [vertex](../../../../../vertex-graph-theory.md) $v$, remove $v$ and introduce a new [vertex](../../../../../vertex-graph-theory.md) $v^*$ whose [vertex neighbourhood](../../../../../vertex-neighbourhood.md) consists precisely of the [vertices](../../../../../vertex-graph-theory.md) in $H_2\cup\cdots\cup H_r$ other than $v$. The new [degree of a vertex](../../../../../degree-graph-theory.md) is $\alpha n-o(n)$. This new [graph](../../../../../graph-split.md) remains $F$-free. Indeed, a new copy of $F$ must use $v^*$, and all its [neighbours of a vertex](../../../../../neighbour-of-a-vertex.md) in that copy lie in the other classes of $H$. There are only boundedly many of them. Each misses only $o(n)$ [vertices](../../../../../vertex-graph-theory.md) in $H_1$, so an unused [vertex](../../../../../vertex-graph-theory.md) $w\in H_1$ is adjacent to all of them. Replacing $v^*$ by $w$ would give $F$ in $G-v$, which is impossible.

Extremality now forces $d_G(v)\geq\alpha n-o(n)$, uniformly in $v$. The upper bound for the [minimum degree of a graph](../../../../../minimum-degree-of-a-graph.md) follows from $\delta(G)\leq2e(G)/n$. For $r=1$, $e(G)=o(n^2)$ already gives $0\leq\delta(G)=o(n)$. Thus

$$
\boxed{\delta(G)=(1-1/r+o(1))n.}
$$

This is the [minimum degree of an extremal forbidden-subgraph graph](../../../../../minimum-degree-of-an-extremal-forbidden-subgraph-graph.md) principle.

**The exact extremal graph for disjoint cliques.** Define

$$
J_s(n)=K_{s-1}+T_r(n-s+1),\qquad
b_s(n)=\binom{s-1}{2}+(s-1)(n-s+1)+e(T_r(n-s+1)).
$$

The plus sign denotes the [join of graphs](../../../../../join-graph-theory.md). The [Turán graph](../../../../../turan-graph.md) contains no $K_{r+1}$, so every such [clique](../../../../../clique-graph-theory.md) in $J_s(n)$ uses a [vertex](../../../../../vertex-graph-theory.md) of $K_{s-1}$. Therefore $J_s(n)$ contains no $s$ vertex-disjoint such [cliques](../../../../../clique-graph-theory.md), and the [extremal number](../../../../../extremal-number.md) is at least $b_s(n)$.

Induct on $s$, with $s=1$ supplied by the [Turan theorem](../../../../../turan-s-theorem.md), including its equality characterization. Let $s\geq2$ and let $G$ be extremal for $sK_{r+1}$. The preceding results give $\delta(G)\geq\alpha n-o(n)$ and the $r$-partite [subgraph](../../../../../subgraph.md) $H$. Keep its classes $H_i$ fixed and assign each of the remaining $o(n)$ [vertices](../../../../../vertex-graph-theory.md) to a class in which it has fewest [neighbours of a vertex](../../../../../neighbour-of-a-vertex.md) in $H$. Write the resulting classes as $C_i$; all have size $n/r+o(n)$. Choose a positive $\tau_n\to0$ so slowly that $\tau_n n$ dominates the outside count, every cross-class error in $H$, and every error in the [minimum degree of a graph](../../../../../minimum-degree-of-a-graph.md) bound.

Suppose some [vertex](../../../../../vertex-graph-theory.md) $x\in C_i$ has at least $\tau_n n$ internal [neighbours of a vertex](../../../../../neighbour-of-a-vertex.md). If $x\notin H$, the assignment rule shows that $x$ has at least $\tau_n n-o(n)$ [neighbours of a vertex](../../../../../neighbour-of-a-vertex.md) in every $H_j$. If $x\in H_i$, it has this many in $H_i$ and $n/r-o(n)$ in the other $H_j$. If $G-x$ contained $s-1$ disjoint $K_{r+1}$, we could choose one [vertex](../../../../../vertex-graph-theory.md) in each $N(x)\cap H_j$, successively avoiding those copies and the $o(n)$ missing cross-neighbours of the already chosen [vertices](../../../../../vertex-graph-theory.md). This produces a further $K_{r+1}$ through $x$. For $r=1$, this just chooses an unused neighbour of $x$. Hence $G-x$ is $(s-1)K_{r+1}$-free, and induction gives

$$
e(G)\leq b_{s-1}(n-1)+(n-1)=b_s(n).
$$

Since the candidate attains $b_s(n)$, equality holds throughout: $x$ is a [universal vertex](../../../../../universal-vertex.md) and $G-x$ is the inductively unique extremal [graph](../../../../../graph-split.md). Thus $G$ is isomorphic to $J_s(n)$.

It remains to show that this case must occur. Otherwise all internal [vertex degrees](../../../../../degree-graph-theory.md) are less than $\tau_n n=o(n)$. Together with the lower bound on $\delta(G)$ and $|C_i|=n/r+o(n)$, this implies that every [vertex](../../../../../vertex-graph-theory.md) misses only $o(n)$ [vertices](../../../../../vertex-graph-theory.md) outside its own class. If some $C_i$ contains a [matching in a graph](../../../../../matching-graph-theory.md) of $s$ [edges](../../../../../edge-of-a-graph.md), extend its [edges](../../../../../edge-of-a-graph.md) one by one to $K_{r+1}$, choosing one [vertex](../../../../../vertex-graph-theory.md) from each other class. At every step only $o(n)$ cross-neighbours and boundedly many used [vertices](../../../../../vertex-graph-theory.md) are excluded. This gives $s$ disjoint forbidden [cliques](../../../../../clique-graph-theory.md), a contradiction.

A [maximal matching](../../../../../maximal-matching.md) in each class therefore has at most $s-1$ [edges](../../../../../edge-of-a-graph.md), and its at most $2(s-1)$ endpoints form a [vertex cover](../../../../../vertex-cover.md) of the internal [edges](../../../../../edge-of-a-graph.md). Their internal [vertex degrees](../../../../../degree-graph-theory.md) are all $o(n)$, so the total internal [edge](../../../../../edge-of-a-graph.md) count is $o(n)$. The cross-class [edge](../../../../../edge-of-a-graph.md) count is at most $e(T_r(n))$, whence

$$
e(G)\leq e(T_r(n))+o(n).
$$

But the balanced part sizes of the [Turán graph](../../../../../turan-graph.md) give

$$
b_s(n)-e(T_r(n))=\frac{s-1}{r}n+O(1),
$$

contradicting extremality for $s\geq2$. This argument also works for $r=1$. Consequently, for all sufficiently large $n$,

$$
\boxed{\operatorname{ex}(n,sK_{r+1})=b_s(n),\quad G\cong K_{s-1}+T_r(n-s+1).}
$$

The uniqueness is up to [isomorphic graphs](../../../../../graph-isomorphism.md), as usual for an [extremal graph for disjoint cliques](../../../../../extremal-graph-for-disjoint-cliques.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 110](../../paper-110-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
