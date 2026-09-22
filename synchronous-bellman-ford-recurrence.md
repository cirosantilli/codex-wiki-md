# Synchronous Bellman-Ford recurrence

↑ **Parent:** [Bellman-Ford algorithm](bellman-ford-algorithm.md)

For the single-source problem, let $D_k(v)$ be the minimum cost of a [directed walk](directed-walk.md) from $s$ to $v$ using at most $k$ [edges](edge-of-a-graph.md). Set $D_0(s)=0$ and $D_0(v)=\infty$ for $v\ne s$, use $\infty+c=\infty$ for finite $c$, and let a [minimum](minimum-of-a-subset-of-a-total-order.md) over an empty [set](set-split.md) be $\infty$. Then

$$
D_k(v)=\min\left\{D_{k-1}(v),\ \min_{(u,v)\in E}\bigl(D_{k-1}(u)+w_{uv}\bigr)\right\}.
$$

Every entry on the right comes from the previous round, requiring separate old and new arrays. The proof is the last-[edge](edge-of-a-graph.md) decomposition: a permitted [directed walk](directed-walk.md) either already uses at most $k-1$ [edges](edge-of-a-graph.md), or ends with some $u\to v$ after a prefix using at most $k-1$. Conversely, each candidate describes a permitted [directed walk](directed-walk.md). This [dynamic programming](dynamic-programming.md) viewpoint gives an exact meaning to every intermediate label, even when negative-cost [directed cycles](directed-cycle.md) exist. Apply the formula to the source too: its initial zero is not a permanent constraint.

If no negative-cost [directed cycle](directed-cycle.md) is reachable from $s$, removing repeated-[vertex](vertex-graph-theory.md) portions of a [directed walk](directed-walk.md) cannot increase its cost. Whenever a destination is reachable, some shortest [directed path](directed-path.md) therefore uses at most $|V|-1$ [edges](edge-of-a-graph.md), and $D_{|V|-1}(v)=\delta(s,v)$. Unreachable [vertices](vertex-graph-theory.md) keep distance $\infty$. For in-place passes, every finite label still comes from a discovered [directed walk](directed-walk.md); moreover, pass $k$ has offered every prefix of length $k$ of a shortest [directed path](directed-path.md), regardless of scan order. Its labels can improve faster than the synchronous labels, while the same $|V|-1$ upper bound on passes remains valid. This is why repeated local corrections eventually settle a global [shortest path problem](shortest-path-problem-split.md).

## ↑ Ancestors (7)

1. [Bellman-Ford algorithm](bellman-ford-algorithm.md)
2. [Shortest path problem](shortest-path-problem-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Bellman-Ford algorithm](bellman-ford-algorithm.md)
