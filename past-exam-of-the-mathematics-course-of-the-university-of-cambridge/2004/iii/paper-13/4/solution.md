<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $\operatorname{CLIQUE}_{n,m}$ be the [monotone Boolean function](../../../../../monotone-boolean-function.md) of the [edge](../../../../../edge-of-a-graph.md) indicators asserting that an $n$-[vertex](../../../../../vertex-graph-theory.md) [graph](../../../../../graph-split.md) contains an $m$-[clique](../../../../../clique-graph-theory.md). We prove a [superpolynomial monotone clique lower bound](../../../../../superpolynomial-monotone-clique-lower-bound.md) using a finite [lattice](../../../../../lattice.md) of approximations. The only circuit theorem assumed is the [Razborov gate-by-gate approximation lemma](../../../../../razborov-gate-by-gate-approximation-lemma.md).

Fix integers $\ell,r\geq2$. Consider upward-closed [set families](../../../../../set-family.md) $A$ of subsets of $[n]$ of size at most $\ell$. Impose the [Razborov closure](../../../../../razborov-closure.md) rule: if $W_1,\ldots,W_r\in A$ have pairwise intersections contained in $W$, adjoin $W$ whenever $|W|\leq\ell$. Also normalize a family containing a set of size zero or one to the full family, since its clique predicate is identically true. Represent it by

$$
\langle A\rangle=\{G:G[W]\text{ is complete for some }W\in A\}.
$$

Closed families form the [finite lattice approximation for monotone clique circuits](../../../../../finite-lattice-approximation-for-monotone-clique-circuits.md), with meet $A\cap B$ and join $\operatorname{cl}(A\cup B)$. An input [edge](../../../../../edge-of-a-graph.md) is represented by the family of its supersets up to size $\ell$. The constant predicates have the empty and full families. The assumed approximation theorem says that a size-$S$ circuit's output disagreement is covered by at most $S$ local gate errors:

$$
\delta_\wedge(A,B)=(\langle A\rangle\cap\langle B\rangle)\setminus\langle A\cap B\rangle,
\qquad
\delta_\vee(A,B)=\langle\operatorname{cl}(A\cup B)\rangle\setminus(\langle A\rangle\cup\langle B\rangle).
$$

We need the [Erdős–Rado sunflower lemma](../../../../../erdos-rado-sunflower-lemma.md): an $s$-[uniform set family](../../../../../uniform-set-family.md) with more than $s!(r-1)^s$ members contains $r$ members with a common pairwise intersection. Its short induction proves the bound. A maximal disjoint subfamily either has $r$ members, already the required empty-core [delta-system](../../../../../delta-system.md), or its union has at most $s(r-1)$ points and meets every member. Some point then occurs in more than $(s-1)!(r-1)^{s-1}$ members. Delete it, apply the induction hypothesis, and restore it to the core. Thus an $r$-closed family has at most

$$
a_s\leq s!(r-1)^s
$$

inclusion-minimal $s$-sets: a sunflower among those members would force its proper core and contradict minimality. This is the [sunflower bound for minimal members of a Razborov-closed family](../../../../../sunflower-bound-for-minimal-members-of-a-razborov-closed-family.md).

For positive inputs choose a uniform $m$-subset $Z$ and the [graph](../../../../../graph-split.md) $K_Z$ having exactly the [edges](../../../../../edge-of-a-graph.md) of its [clique](../../../../../clique-graph-theory.md). Put $q=\ell rm/n$ and suppose $q\leq1/2$. A nonuniversal family has no minimal member of size at most one, so it accepts at most

$$
\sum_{s=2}^\ell s!(r-1)^s\left(\frac mn\right)^s
\leq\sum_{s=2}^\ell q^s\leq2q^2
$$

of positive inputs. Here $\mathbb P(W\subseteq Z)=(m)_{|W|}/(n)_{|W|}\leq(m/n)^{|W|}$.

If $K_Z$ is in a meet-error set, it contains minimal witnesses $X\in A,Y\in B$. Their union must have size greater than $\ell$, since otherwise upward closure would put it in $A\cap B$. At least one witness therefore has size greater than $\ell/2$. The same counting and the [union bound](../../../../../boole-s-inequality.md) give the [positive clique error of a truncated lattice meet](../../../../../positive-clique-error-of-a-truncated-lattice-meet.md):

$$
\mathbb P(K_Z\in\delta_\wedge(A,B))
\leq2\sum_{s>\ell/2}s!(r-1)^s(m/n)^s
\leq4q^{\ell/2}.
$$

For negative inputs independently assign one of $m-1$ colours to each [vertex](../../../../../vertex-graph-theory.md), joining differently coloured [vertices](../../../../../vertex-graph-theory.md). Every resulting [complete multipartite graph](../../../../../complete-multipartite-graph.md) is $m$-[clique](../../../../../clique-graph-theory.md)-free. Consider one forcing step adjoining $W$. If its [clique](../../../../../clique-graph-theory.md) is newly accepted, $W$ is rainbow while all witnesses $W_i$ are not. Condition on the colours of $W$. The sets $W_i\setminus W$ are disjoint, so their non-rainbow events are [conditionally independent](../../../../../conditional-independence.md). For each witness, every possible collision either involves two random petal colours or one petal colour and one fixed core colour; its probability is at most

$$
\frac{\binom\ell2}{m-1}.
$$

When this is at most $1/2$, a step makes a negative error with probability at most $2^{-r}$. Upward closure itself introduces no extra accepted [graphs](../../../../../graph-split.md), and normalization introduces no extra error beyond the forcing step that produced a set of size at most one. At most $\sum_{j=0}^\ell\binom nj\leq n^{\ell+1}$ sets can be forced. The [negative colouring error of a forced-set closure](../../../../../negative-colouring-error-of-a-forced-set-closure.md) is therefore

$$
\mathbb P(G_{\mathrm{colour}}\in\delta_\vee(A,B))\leq n^{\ell+1}2^{-r}.
$$

Set $m=r=\lfloor n^{1/4}\rfloor$ and $\ell=\lfloor\log_2n\rfloor$. For sufficiently large $n$, both probability conditions hold and $2q^2<1/2$. If the output approximation is nonuniversal, it misses at least half the positive inputs, so the [Razborov gate-by-gate approximation lemma](../../../../../razborov-gate-by-gate-approximation-lemma.md) forces $1/2\leq4Sq^{\ell/2}$. If it is universal, it accepts every negative colouring input, forcing $1\leq Sn^{\ell+1}2^{-r}$. Consequently

$$
S\geq\min\left\{\frac1{8q^{\ell/2}},\frac{2^r}{n^{\ell+1}}\right\}.
$$

Since $\log(1/q)\geq\frac12\log n-\log\ell$ and $r$ grows faster than $(\log n)^2$, both terms imply

$$
\boxed{S\geq\exp(c(\log n)^2)=n^{c\log n}}
$$

for an absolute positive $c$ and all sufficiently large $n$. This is superpolynomial in the $\binom n2$ input bits. The argument concerns AND/OR [monotone circuits](../../../../../monotone-circuit.md); it gives no such bound for circuits allowed negation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
