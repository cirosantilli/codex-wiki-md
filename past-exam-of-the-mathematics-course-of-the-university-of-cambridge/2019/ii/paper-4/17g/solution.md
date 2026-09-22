<h1 id="17g/solution">Solution</h1>

↑ **Parent:** [17G](../17g.md)

The [Hall marriage theorem](../../../../../hall-s-marriage-theorem.md) states that a finite [bipartite graph](../../../../../bipartite-graph.md) with vertex classes $U$ and $V$ has a [matching in a graph](../../../../../matching-graph-theory.md) saturating $U$ if and only if

$$
|N(A)|\geq|A|
\qquad\text{for every }A\subseteq U.
$$

Necessity is immediate: distinct vertices of $A$ must be matched to distinct vertices of $N(A)$.

For sufficiency, induct on $|U|$. If every nonempty proper $A\subset U$ satisfies the strict bound $|N(A)|\geq|A|+1$, choose any edge $uv$ and delete its endpoints. Every $A\subseteq U\setminus\{u\}$ loses at most the neighbour $v$, so Hall's condition remains true; induction supplies a matching of the smaller graph, to which $uv$ is added.

Otherwise there is a nonempty proper tight set $A\subset U$ with $|N(A)|=|A|$. Hall's condition holds on the induced graph with parts $A,N(A)$, so induction matches $A$. For $B\subseteq U\setminus A$, Hall's condition on $A\cup B$ gives

$$
|A|+|B|
\leq|N(A\cup B)|
\leq|N(A)|+|N(B)\setminus N(A)|,
$$

and hence $|N(B)\setminus N(A)|\geq|B|$. Induction therefore matches $U\setminus A$ into $V\setminus N(A)$. The two matchings are disjoint and together saturate $U$, completing the proof through [Hall induction through a tight set](../../../../../hall-induction-through-a-tight-set.md).

Identify a subset of $[n]$ with its binary characteristic vector. Then $Q$ is the [hypercube graph](../../../../../hypercube-graph.md), and every edge changes set size by exactly one. The [induced subgraph](../../../../../induced-subgraph.md) on $X_{i-1}\cup X_i$ is therefore bipartite with those two levels as its vertex classes.

Let $\mathcal A\subseteq X_{i-1}$. Every member of $\mathcal A$ has $n-i+1$ neighbours in $X_i$, obtained by adding one element, while every member of $N(\mathcal A)$ is incident with at most $i$ of these edges. Double-counting the edges between the two families gives

$$
(n-i+1)|\mathcal A|\leq i|N(\mathcal A)|.
$$

Since $i\leq n/2$, we have $n-i+1\geq i$, and hence $|N(\mathcal A)|\geq|\mathcal A|$. Hall's theorem yields the requested [adjacent-level matching in a Boolean lattice](../../../../../adjacent-level-matching-in-a-boolean-lattice.md), saturating $X_{i-1}$.

Finally, every [chain in a partially ordered set](../../../../../chain-in-a-partially-ordered-set.md) in the [Boolean lattice](../../../../../boolean-lattice.md) contains at most one member of the middle level $X_{n/2}$. Any chain partition therefore uses at least

$$
\binom n{n/2}
$$

chains.

For every $i\leq n/2$, choose one of the matchings just constructed and orient its edges upward. These edges partition all levels at or below $n/2$ into chains ending at distinct middle-level sets. Taking complements gives, for every $i\geq n/2$, a matching from $X_{i+1}$ into $X_i$; orienting its edges upward extends those chains through all upper levels. Every subset belongs to exactly one resulting chain and every chain meets $X_{n/2}$ exactly once. Thus this [symmetric chain decomposition of a Boolean lattice](../../../../../symmetric-chain-decomposition-of-a-boolean-lattice.md) has one chain per middle-level set, and the minimum is

$$
\boxed{k=\binom n{n/2}.}
$$

## ↑ Ancestors (10)

1. [17G](../17g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
