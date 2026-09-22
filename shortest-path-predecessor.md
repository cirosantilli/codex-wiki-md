# Shortest-path predecessor

↑ **Parent:** [Dijkstra algorithm](dijkstra-algorithm.md)

A shortest-path predecessor $\pi(v)$ records the previous [vertex](vertex-graph-theory.md) on a chosen route from source $s$ to $v$. When [edge relaxation](edge-relaxation.md) strictly improves $d(v)$ through $u\to v$, set $\pi(v)=u$. For a [multigraph](multigraph.md), store the actual [directed edge](directed-edge.md), since two [edges](edge-of-a-graph.md) with the same endpoints can have different weights. Initialize all [vertices](vertex-graph-theory.md), including the source, without a [shortest-path predecessor](shortest-path-predecessor.md). The authored implementation reconstructs a route by following these incoming [edges](edge-of-a-graph.md) backwards, then reversing their order.[Sedgewick and Wayne, DijkstraSP.java, edgeTo and pathTo](https://raw.githubusercontent.com/kevin-wayne/algs4/master/src/main/java/edu/princeton/cs/algs4/DijkstraSP.java)

At the end of the [edge relaxation](edge-relaxation.md) trace, $\pi(t)=a$, $\pi(a)=b$, and $\pi(b)=s$. Following them gives $t,a,b,s$, so the forward [directed path](directed-path.md) is $s\to b\to a\to t$, of cost $2-1+2=3$. This makes the distance useful: a number tells us the best cost, whereas the [shortest-path predecessors](shortest-path-predecessor.md) tell us which connections to take. In the [Dijkstra algorithm](dijkstra-algorithm.md), reconstruct a destination's shortest route after its label becomes permanent. In a [label-correcting shortest-path algorithm](label-correcting-shortest-path-algorithm.md), wait for convergence and the appropriate negative-cost [directed cycle](directed-cycle.md) check. During correction, a predecessor's label may have changed since its child's last update: immediately after $b\to a$ in the trace, the current chain to $t$ costs $3$ although $d(t)$ still records the earlier discovered route of cost $8$.

Strict improvement is a useful guard against [directed cycles](directed-cycle.md) in the recorded pointers. Consider $s\to a$ and $s\to b$ of cost zero, followed by $a\to b$ and $b\to a$, also of cost zero. After the first two [edge relaxations](edge-relaxation.md), both labels are zero and both [shortest-path predecessors](shortest-path-predecessor.md) are $s$. If equality also allows pointer replacement, the last two operations can set $\pi(b)=a$ and $\pi(a)=b$: following pointers loops forever despite correct distance labels. Keeping the old pointer on ties prevents this example; choosing among equal-cost routes requires a separate rule that preserves a route to the source. Strict improvement alone does not protect against reachable negative-cost [directed cycles](directed-cycle.md), which can force endless decreases. Equality on recorded [edges](edge-of-a-graph.md) plus the [Bellman inequalities](bellman-inequalities.md) certifies route costs only when the pointer chains actually terminate at the source.

For all-to-one distances to $r$, record a next [vertex](vertex-graph-theory.md) $j$ whenever relaxing $i\to j$ improves $d_i$. Follow these successors forward in the original [directed graph](directed-graph.md) to reach $r$. They are [shortest-path predecessors](shortest-path-predecessor.md) when viewed in the reversed [directed graph](directed-graph.md); keeping the direction convention explicit prevents returning a route whose arrows point the wrong way.

## ↑ Ancestors (7)

1. [Dijkstra algorithm](dijkstra-algorithm.md)
2. [Shortest path problem](shortest-path-problem.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Dijkstra algorithm](dijkstra-algorithm.md)
- [Edge relaxation](edge-relaxation.md)
- [Shortest-path predecessor](shortest-path-predecessor.md)
