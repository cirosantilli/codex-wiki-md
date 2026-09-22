<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We first need the [minimal-member bound for a Razborov-closed family](../../../../../../minimal-member-bound-for-a-razborov-closed-family.md): an $r$-closed family has at most $(r-1)^k$ inclusion-minimal members of size $k$. Indeed, its minimal members of size at most $k$ cannot contain $r$ sets whose pairwise intersections lie inside a proper subset of another minimal member, since closure would then contain that proper subset. The resulting set-system bound is proved by induction on $r$: fix one member $D$, partition the remaining members according to their intersections $C\subseteq D$, delete $C$, and apply the $(r-1,k-|C|)$ bound in each class. Summing over $C$ gives

$$
\sum_{C\subseteq D}(r-2)^{k-|C|}
=(r-1)^k.
$$

If $\langle A\rangle$ is not the set of all graphs, no inclusion-minimal member of $A$ has size zero or one. Every $m$-clique in $\langle A\rangle$ contains a minimal $W\in A$, so the number of such cliques is at most

$$
\sum_{k=2}^l(r-1)^k\binom{n-k}{m-k}.
$$

Dividing by $\binom nm$ and using

$$
\frac{\binom{n-k}{m-k}}{\binom nm}
=\frac{(m)_k}{(n)_k}
\leq\left(\frac mn\right)^k,
$$

the assumed $2(r-1)m\leq n$ gives a proportion at most

$$
\sum_{k=2}^\infty2^{-k}=\frac12.
$$

**Thus either $\langle A\rangle$ is universal or it contains at most half of all $m$-cliques.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
