<h1 id="17i/solution">Solution</h1>

↑ **Parent:** [17I](../17i.md)

We first prove the required case of [Menger's theorem](../../../../../menger-theorem.md) directly. Split each vertex $v$ into $v_{
m in}$ and $v_{
m out}$ joined by a directed edge of capacity one. Replace every graph edge $uv$ by the two directed edges $u_{
m out}v_{
m in}$ and $v_{
m out}u_{
m in}$ of capacity $k$, add a source joined to every $a_{\rm in}$ for $a\in A$, and join every $b_{\rm out}$ for $b\in B$ to a sink, using unit capacities at the ends.

Starting with zero integral flow, repeatedly augment by one along a source-to-sink path in the residual directed graph. If fewer than $k$ augmentations have occurred and no augmenting path remains, let $R$ be the residual-reachable vertices. The capacity from $R$ to its complement equals the current flow: every forward edge in this cut is saturated and every reverse edge carries zero flow, by residual reachability. Since the cut has capacity below $k$, it uses no capacity-$k$ graph edge. The original vertices whose unit-capacity split or endpoint edges cross the cut form an $AB$-separator of size below $k$, contrary to the hypothesis. Hence at least $k$ augmentations occur. The resulting integral flow decomposes into $k$ source-to-sink paths, and the unit split capacities make their corresponding $AB$ paths vertex-disjoint. This proves

$$
\boxed{\text{there are }k\text{ vertex-disjoint }AB\text{-paths}.}
$$

The same augmenting-path proof, with the source vertex given capacity $k$, yields the [fan lemma](../../../../../fan-lemma.md): from a vertex $x$ to any set of at least $k$ vertices in a [k-connected graph](../../../../../k-connected-graph.md), there is a $k$-fan with distinct endpoints.

Now let $C$ be a longest cycle in a finite $k$-connected graph $G$. If $C$ is not Hamiltonian, choose $x\notin C$. A $k$-fan from $x$ to $C$ has $k$ distinct attachment vertices. If $|C|<2k$, two consecutive attachment vertices on $C$ are joined by an edge of $C$, because the $k$ cyclic gaps cannot all have length at least two. The two corresponding fan paths form, through $x$, an alternative path of length at least two between those adjacent vertices. Replacing their edge on $C$ by this path creates a longer cycle, a contradiction. Therefore

$$
\boxed{|C|\geq\min\{|G|,2k\}.}
$$

This is the [Dirac circumference theorem](../../../../../dirac-circumference-theorem.md); in particular, a $k$-connected graph contains a cycle of length at least $k$, and when $|G|\geq2k$ it **must** contain one of length at least $2k$.

For $k=3$, every 3-connected graph with at least six vertices consequently has a cycle of length at least six. This cannot be improved: the [complete bipartite graph](../../../../../complete-bipartite-graph.md) $K_{3,m}$ is 3-connected for $m\geq3$, but every cycle alternates between its two parts and therefore has length at most six. Taking $m$ arbitrarily large defeats every proposed bound above six. Hence

$$
\boxed{n=6.}
$$

## ↑ Ancestors (10)

1. [17I](../17i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
