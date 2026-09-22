<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A path in a [causal directed acyclic graph](../../../../../../causal-directed-acyclic-graph.md) is active given a conditioning set $K$ when every noncollider on the path is outside $K$ and every collider has itself or a descendant in $K$. Two vertex sets are [d-separated](../../../../../../d-separation.md) by $K$ when no path between them is active given $K$. The [global Markov property of a directed acyclic graph](../../../../../../global-markov-property-of-a-directed-acyclic-graph.md) then turns d-separation into conditional independence.

In the displayed graph, the edges are

$$
X_1\to X_2,
\quad X_1\to X_3,
\quad X_2\to X_3,
\quad X_3\to X_4,
\quad U\to X_2,
\quad U\to X_4.
$$

Every observed pair except $(X_1,X_4)$ and $(X_2,X_4)$ is joined by a direct edge, which remains active under conditioning on any other observed variables. The pair $(X_2,X_4)$ is always joined by the fork $X_2\leftarrow U\to X_4$, because the unobserved noncollider $U$ cannot be conditioned on.

For $(X_1,X_4)$, if $X_3$ is not conditioned on, $X_1\to X_3\to X_4$ is active. If $X_3$ is conditioned on, the path

$$
X_1\to X_2\leftarrow U\to X_4
$$

becomes active because its collider $X_2$ has conditioned descendant $X_3$; conditioning on $X_2$ itself also opens it. Thus every observed pair is d-connected given every subset of the other observed variables. Any conditional independence between two nonempty observed subvectors would imply one between each selected pair, so the graph entails none.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
