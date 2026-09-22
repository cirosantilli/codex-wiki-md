<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We prove [edit-distance stability for clique-free graphs](../../../../../edit-distance-stability-for-clique-free-graphs.md) by induction on $r$, using the [symmetric difference](../../../../../symmetric-difference.md) of [edge](../../../../../edge-of-a-graph.md) sets as the distance. For $r=1$, a $K_2$-free [graph](../../../../../graph-split.md) is edgeless, and there is nothing to change. For $r\ge2$, choose a [vertex](../../../../../vertex-graph-theory.md) of maximum degree $d$, let $A$ be its neighbourhood and put $B=V(G)\setminus A$. Then $G[A]$ is $K_r$-free. Write

$$
D=t_r(n)-e(G),\qquad D_A=t_{r-1}(d)-e(G[A]),\qquad b=e(G[B]),\qquad m=|A||B|-e_G(A,B).
$$

Both deficits are nonnegative by the [Turan theorem](../../../../../turan-s-theorem.md). Since every [vertex](../../../../../vertex-graph-theory.md) of $B$ has degree at most $d=|A|$,

$$
e_G(A,B)+2b\le |B|d,\qquad m\ge2b.
$$

The complete $r$-partite [graph](../../../../../graph-split.md) formed from an $(r-1)$-partite [Turán graph](../../../../../turan-graph.md) on $A$ and the new class $B$ has at most $t_r(n)$ [edges](../../../../../edge-of-a-graph.md). Thus $L=t_r(n)-t_{r-1}(d)-|A||B|\ge0$, and direct subtraction gives

$$
D=L+D_A+m-b.
$$

By induction, edit $G[A]$ into a complete $(r-1)$-partite [graph](../../../../../graph-split.md) using at most $3D_A$ changes. Delete the $b$ [edges](../../../../../edge-of-a-graph.md) inside $B$, and add the $m$ missing [edges](../../../../../edge-of-a-graph.md) between $A$ and $B$. The resulting [graph](../../../../../graph-split.md) is complete $r$-partite on the same [vertex](../../../../../vertex-graph-theory.md) set, and

$$
3D_A+b+m\le3D_A+3(m-b)+3L=3D\le3k,
$$

where the inequality uses $m\ge2b$. **The required edit distance is at most $3k$.** Empty partition classes are allowed; a sufficiently dense nondegenerate case has the usual full complement of classes.

For the odd-cycle conclusion, use two standard consequences of the [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md), stated explicitly. The [triangle removal lemma](../../../../../triangle-removal-lemma.md) says that for every $\alpha>0$, some $\beta>0$ ensures that a [graph](../../../../../graph-split.md) with at most $\beta n^3$ [triangles in a graph](../../../../../triangle-in-a-graph.md) can be made triangle-free by deleting at most $\alpha\binom n2$ [edges](../../../../../edge-of-a-graph.md), for all sufficiently large $n$. Also, for each fixed odd length $\ell\ge3$ and each $\beta>0$, there is $\zeta>0$ such that a [graph](../../../../../graph-split.md) with at least $\beta n^3$ [triangles in a graph](../../../../../triangle-in-a-graph.md) contains at least $\zeta n^\ell$ copies of $C_\ell$.

For clarity, the latter [odd-cycle copies from positive triangle density](../../../../../odd-cycle-copies-from-positive-triangle-density.md) consequence follows by applying regularity with error small relative to $\beta$, removing exceptional, irregular and very sparse pairs, and retaining a [triangle in a graph](../../../../../triangle-in-a-graph.md) among the remaining regular dense pairs. The [graph embedding lemma for regular pairs](../../../../../graph-embedding-lemma-for-regular-pairs.md) counts a positive constant times $n^\ell$ embeddings of any fixed [graph](../../../../../graph-split.md) properly three-coloured into those three clusters, including $C_\ell$. Dividing by the fixed number of descriptions of a cycle gives the same conclusion for unlabelled copies.

Apply [triangle in a graph](../../../../../triangle-in-a-graph.md) removal with $\alpha=\epsilon$, and take the resulting $\beta$. A $C_{2013}$-free [graph](../../../../../graph-split.md) cannot have $\beta n^3$ [triangles in a graph](../../../../../triangle-in-a-graph.md) for large $n$, by the preceding consequence. Delete at most $\epsilon\binom n2$ [edges](../../../../../edge-of-a-graph.md) to obtain a triangle-free $G'$. With $N=\binom n2$,

$$
e(G')\ge(1/2-2\epsilon)N,\qquad t_2(n)-e(G')\le2\epsilon N+n/4.
$$

Apply the proved stability result with $r=2$. The resulting complete bipartite [graph](../../../../../graph-split.md) $H$ satisfies

$$
|E(G)\mathbin\triangle E(H)|\le\epsilon N+3(2\epsilon N+n/4)=7\epsilon N+3n/4.
$$

Choose $n_0(\epsilon)$ also large enough that $3n/4\le4\epsilon N$. **Then the distance is at most $11\epsilon\binom n2$.**

For the unheaded continuation, use the same $\beta$ and its associated $\zeta$, and set $\delta=\zeta/2$. Having at most $\delta n^{2013}$ cycles rules out $\beta n^3$ [triangles in a graph](../../../../../triangle-in-a-graph.md) just as before. The identical deletion and stability calculation applies. **A sufficiently small $\delta=\delta(\epsilon)>0$ gives the same $11\epsilon$ bound.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
