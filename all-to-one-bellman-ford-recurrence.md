# All-to-one Bellman-Ford recurrence

↑ **Parent:** [Bellman-Ford algorithm](bellman-ford-algorithm.md)

Keep the original all-to-one orientation of the [Bellman inequalities](bellman-inequalities.md): $d_i^{(k)}$ concerns routes _from_ $i$ _to_ a fixed sink $r$, and $c_{ij}$ belongs to the original [directed edge](directed-edge.md) $i\to j$. Initialize $d_r^{(0)}=0$ and $d_i^{(0)}=\infty$ for $i\ne r$. The synchronous [dynamic programming](dynamic-programming.md) recurrence is

$$
d_i^{(k)}=\min\left\{d_i^{(k-1)},\ \min_{(i,j)\in E}\bigl(c_{ij}+d_j^{(k-1)}\bigr)\right\}.
$$

It prepends the first [edge](edge-of-a-graph.md) of a route instead of appending the last: $d_i^{(k)}$ is the minimum cost of a [directed walk](directed-walk.md) from $i$ to $r$ using at most $k$ [edges](edge-of-a-graph.md). In particular, improving $d_j$ can improve labels on incoming [directed edges](directed-edge.md) $i\to j$. The same original [directed edge](directed-edge.md) therefore updates its tail in this convention, whereas single-source [edge relaxation](edge-relaxation.md) updates its head.

If no negative-cost [directed cycle](directed-cycle.md) can reach $r$, $|V|-1$ rounds suffice for every distance to $r$, and $d_r^{(k)}=0$ automatically. This hypothesis concerns [directed paths](directed-path.md) _from the cycle to the sink_, not paths from the sink to the cycle. In the base example with its original arrows and sink $T$, the distances in order $(S,A,B,C,T)$ are $(7,3,5,2,0)$. Once $C\to A$ of weight $-4$ is added, $S,A,B,C$ instead have distance $-\infty$ to $T$, while $T$ keeps distance $0$ and $U$ keeps $\infty$.

More generally, $\delta(i,r)=-\infty$ precisely when $i$ can reach a negative-cost [directed cycle](directed-cycle.md) that can reach $r$. Thus the affected [vertices](vertex-graph-theory.md) are the ancestors of such a [directed cycle](directed-cycle.md). A negative-cost [directed cycle](directed-cycle.md) unable to reach $r$ is irrelevant. Reversing all arrows makes $r$ a single source, turns these ancestors into descendants, and makes the detection and forward [graph search](graph-search.md) above directly applicable. The right panel of the figure uses that reversal with sink $S$; its distances to $S$ equal the left panel's distances from $S$.

Do not force the root to remain zero outside the hypothesis. Consider the two [directed edges](directed-edge.md) $r\to a$ of cost $0$ and $a\to r$ of cost $-1$, with sink $r$. The recurrence gives $d_a^{(1)}=-1$ and $d_r^{(2)}=-1$: the latter records one lap of a negative-cost [directed cycle](directed-cycle.md) through $r$. Repetition makes both unrestricted distances $-\infty$. Clamping $d_r$ at zero and omitting its update would instead leave the stationary labels $(d_r,d_a)=(0,-1)$, concealing that behaviour. Initialization specifies the cost of the empty [directed walk](directed-walk.md); it does not forbid cheaper nonempty returns to the root. Cycle detection must test every relevant [directed edge](directed-edge.md), including those whose relaxation updates the root.

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
