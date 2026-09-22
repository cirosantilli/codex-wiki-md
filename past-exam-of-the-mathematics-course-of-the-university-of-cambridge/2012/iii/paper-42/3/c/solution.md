<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $C^*$ be an optimal metric tour. Removing any one of its edges gives a [spanning tree](../../../../../../spanning-tree.md), so the [minimum spanning tree](../../../../../../minimum-spanning-tree.md) $T$ satisfies $c(T)\leq c(C^*)$. The [handshaking lemma](../../../../../../degree-sum-formula.md) shows that its odd-degree set $U$ has even size.

Follow $C^*$ and retain only vertices of $U$, shortcutting between consecutive retained vertices. This produces a cyclic order on $U$ of total cost at most $c(C^*)$. If $U$ is nonempty, the alternating edges of that cyclic order form two [perfect matchings](../../../../../../perfect-matching.md); their costs sum to the cycle cost. One has cost at most $c(C^*)/2$, so a [minimum-weight perfect matching](../../../../../../minimum-weight-perfect-matching.md) $M$ has

$$
\boxed{c(M)\leq\tfrac12c(C^*).}
$$

For $|U|=2$, count the same undirected edge twice in the cyclic order; each alternating matching consists of one copy. For $U=\varnothing$, use the empty matching.

The multigraph with edges $T\uplus M$ is connected because it contains $T$. Each odd-degree vertex receives exactly one matching edge, and the other degrees are unchanged, so every degree is even. It therefore has an [Euler circuit](../../../../../../euler-circuit.md). Constructively, follow unused edges until returning to the starting vertex; parity prevents getting stuck elsewhere. If unused edges remain, connectivity supplies a vertex of the current circuit incident with one, and its additional closed trail can be spliced into the circuit. Repetition gives a circuit using every edge exactly once, including parallel copies.

Shortcut repeated vertices of this [Euler circuit](../../../../../../euler-circuit.md) to obtain a metric tour. Its cost is at most

$$
\boxed{c(T)+c(M)\leq\tfrac32c(C^*).}
$$

Computing a [minimum spanning tree](../../../../../../minimum-spanning-tree.md), a [minimum-weight perfect matching](../../../../../../minimum-weight-perfect-matching.md), an [Euler circuit](../../../../../../euler-circuit.md) and the shortcut tour is polynomial-time; weighted [perfect matching](../../../../../../perfect-matching.md) is a standard polynomial-time graph optimization problem. Thus **the [Christofides algorithm](../../../../../../christofides-algorithm.md) is a $3/2$-[approximation algorithm](../../../../../../approximation-algorithm.md) for symmetric metric tours**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
