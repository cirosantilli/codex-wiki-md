<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $K_s(t)$ for the balanced [graph blow-up](../../../../../graph-blow-up.md) of a [complete graph](../../../../../complete-graph.md), with $s$ classes of size $t$; containment here is as a subgraph, not necessarily an induced subgraph. The logarithmic form of the [Erdős-Stone theorem](../../../../../erdos-stone-theorem.md) is: for fixed $r\ge1$ and $0<\epsilon<1/r$, there are $d=d(r,\epsilon)>0$ and $n_0$ such that

$$
e(G)\ge\left(1-\frac1r+\epsilon\right)\binom n2,\qquad n\ge n_0
\quad\Longrightarrow\quad K_{r+1}(\lfloor d\log n\rfloor)\subseteq G.
$$

Thus **the guaranteed balanced part size is at least $\lfloor d\log n\rfloor$**, with $d$ independent of $n$. We prove the [logarithmic Erdős-Stone theorem](../../../../../logarithmic-erdos-stone-theorem.md) by a density-to-cliques step and a constructive [dense clique family blow-up lemma](../../../../../dense-clique-family-blow-up-lemma.md).

First choose a fixed $m$ large enough that $t_r(m)/\binom m2\le1-1/r+\epsilon/2$, where $t_r(m)$ is the [edge](../../../../../edge-of-a-graph.md) count of the [Turán graph](../../../../../turan-graph.md). A uniformly chosen $m$-vertex subset has expected [edge](../../../../../edge-of-a-graph.md) count at least $(1-1/r+\epsilon)\binom m2$. If its induced [graph](../../../../../graph-split.md) contains no $K_{r+1}$, the [Turan theorem](../../../../../turan-s-theorem.md) bounds that count by $t_r(m)$. Since the count is always at most $\binom m2$, the probability that the subset contains an $(r+1)$-clique is at least $\epsilon/2$. Double counting the incidences between such subsets and their [cliques](../../../../../clique-graph-theory.md) gives, for $s=r+1$,

$$
k_s(G)\ge\frac\epsilon2\frac{\binom nm}{\binom{n-s}{m-s}}=\frac\epsilon2\frac{(n)_s}{(m)_s}\ge\eta n^s
$$

for a fixed $\eta>0$ and all sufficiently large $n$. Here $(x)_s=x(x-1)\cdots(x-s+1)$. This is [clique supersaturation by sampling](../../../../../clique-supersaturation-by-sampling.md).

We now prove the needed [dense clique family blow-up lemma](../../../../../dense-clique-family-blow-up-lemma.md), with the following stronger induction invariant. Given any family $\mathcal M$ of at least $\eta n^s$ distinct $s$-cliques, there is a complete $s$-partite subgraph with each class of size $\lfloor a_s(\eta)\log n\rfloor$, containing that many pairwise vertex-disjoint transversal members of $\mathcal M$, each with one vertex in every class. Extra [edges](../../../../../edge-of-a-graph.md) within its classes can be ignored. We may suppose $0<\eta<1/2$. For $s=1$, any $\eta n$ singletons suffice, and we may take $a_1(\eta)=1$ once $n$ is large.

For $s\ge2$, put $\theta=\eta/2$. Repeatedly delete every member of the current family containing an $(s-1)$-clique whose number of extensions is at most $\theta n$. Each such face is processed at most once, and there are at most $n^{s-1}$ possible faces. At most $\theta n^s$ members are deleted. The remaining family $\mathcal L$ has size at least $(\eta/2)n^s$, and every face that remains has more than $\theta n$ extensions. Its family of $(s-1)$-faces has size at least $s|\mathcal L|/n\ge(\eta/2)n^{s-1}$, since each face is in at most $n$ members.

Apply the induction hypothesis to these faces. It gives a complete $(s-1)$-partite subgraph with $m=\lfloor a_{s-1}(\eta/2)\log n\rfloor$ [vertices](../../../../../vertex-graph-theory.md) in each class and a matching $R_1,\ldots,R_m$ of transversal $(s-1)$-faces from the family. Form a [bipartite graph](../../../../../bipartite-graph.md) whose left [vertices](../../../../../vertex-graph-theory.md) are the $R_i$ and whose right [vertices](../../../../../vertex-graph-theory.md) are the original $n$ [vertices](../../../../../vertex-graph-theory.md); join $R_i$ to $v$ when $R_i\cup\{v\}\in\mathcal L$. Every left degree exceeds $\theta n$.

The following [common neighbourhood from bipartite density](../../../../../common-neighbourhood-from-bipartite-density.md) estimate is elementary. In a bipartite [graph](../../../../../graph-split.md) with class sizes $m,n$ and at least $\theta mn$ [edges](../../../../../edge-of-a-graph.md), averaging over left subsets $S$ of size $u$ and using convexity of the integer sequence $j\mapsto\binom ju$ gives

$$
\max_{|S|=u}|N(S)|\ge\frac{\sum_{v\text{ on right}}\binom{d(v)}u}{\binom mu}
\ge n\frac{\binom{\lfloor\theta m\rfloor}u}{\binom mu}\ge n(\theta/2)^u
$$

whenever $1\le u\le\theta m/2$. The last inequality follows by comparing the $u$ factors in the two binomial coefficients; the integer convexity follows from the nondecreasing first differences $\binom j{u-1}$.

Choose

$$
a_s(\eta)=\min\left\{\frac{\theta a_{s-1}(\eta/2)}8,\ \frac1{2\log(2/\theta)}\right\},\qquad u=\lfloor a_s(\eta)\log n\rfloor.
$$

For large $n$, $m\ge\tfrac12a_{s-1}(\eta/2)\log n$, so $u\le\theta m/4$. The estimate supplies $u$ selected faces with a common extension set of size at least $n(\theta/2)^u\ge\sqrt n$. This extension set is disjoint from the selected faces: a [vertex](../../../../../vertex-graph-theory.md) in any one of them cannot extend that face. Their union has $u$ [vertices](../../../../../vertex-graph-theory.md) in each of the old $s-1$ classes, with all required cross [edges](../../../../../edge-of-a-graph.md); choose $u$ distinct common extension [vertices](../../../../../vertex-graph-theory.md) as a new class. Attaching one different extension [vertex](../../../../../vertex-graph-theory.md) to each selected face also gives $u$ disjoint members of $\mathcal L$. This completes the induction, with positive constants independent of $n$. Apply it to the [clique](../../../../../clique-graph-theory.md) family above and take $d=a_{r+1}(\eta)$.

The logarithmic order cannot be increased in a uniform forcing result. Put $\rho=1-1/r+\epsilon<1$, choose $p$ strictly between $\rho$ and one, and take a [binomial random graph](../../../../../binomial-random-graph.md). Its [edge](../../../../../edge-of-a-graph.md) density exceeds $\rho$ with probability tending to one, by the variance estimate for a sum of independent [edge](../../../../../edge-of-a-graph.md) indicators. With $s=r+1$, the expected number of ordered embeddings of $K_s(t)$ is at most

$$
n^{st}p^{\binom s2t^2}.
$$

For $t=\lceil C\log n\rceil$ and $C>2/((s-1)\log(1/p))$, the logarithm of this bound is negative of order $(\log n)^2$. [Markov's inequality](../../../../../markov-inequality.md) therefore makes the probability of any such copy tend to zero. Both events hold simultaneously for some [graphs](../../../../../graph-split.md) of every sufficiently large order. **There are [graphs](../../../../../graph-split.md) meeting the density hypothesis whose largest balanced blow-up has part size $O(\log n)$.** This upper bound concerns what density can force; it is not an upper bound for every dense [graph](../../../../../graph-split.md), since a complete [graph](../../../../../graph-split.md) has much larger blow-ups.

Finally, $H_k$ is the [square of a cycle](../../../../../square-of-a-cycle.md), for $k\ge3$. Any three consecutive [vertices](../../../../../vertex-graph-theory.md) form a [triangle in a graph](../../../../../triangle-in-a-graph.md). In a proper three-colouring, once the first three colours are fixed, each subsequent [vertex](../../../../../vertex-graph-theory.md) must repeat the colour three positions earlier. Closing the cycle is possible precisely when $3\mid k$. Conversely, repeating the three colours gives such a colouring whenever $3\mid k$. In that case $H_k$ embeds in $K_3(k/3)$, and the density $0.51\binom n2$ exceeds the bipartite [Turan theorem](../../../../../turan-s-theorem.md) threshold by a fixed amount, so the theorem forces $H_k$ eventually. If $3\nmid k$, the balanced [Turán graphs](../../../../../turan-graph.md) $T_3(n)$ have density at least $2/3$ and contain no [graph](../../../../../graph-split.md) of chromatic number greater than three. They give a counterexample sequence. **Exactly the cycle lengths $k\ge3$ divisible by three have the required property.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
