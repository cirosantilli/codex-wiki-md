# Bellman-Ford negative-cycle detection

↑ **Parent:** [Bellman-Ford algorithm](bellman-ford-algorithm.md)

A negative-cost [directed cycle](directed-cycle.md) matters to a particular destination $v$ precisely when it is reachable from $s$ and can itself reach $v$.[6.006 Introduction to Algorithms, Fall 2011 by Massachusetts Institute of Technology, 6.006 course staff; MIT 6.006, Lecture 17, p. 1: cycle between source and destination; p. 4: reachable-cycle corollary](6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-17-shortest-paths-iii-bellman-ford.md) Repeating it $m$ times adds $m$ times its negative total cost to a route. Thus the [infimum](infimum.md) of [directed walk](directed-walk.md) costs is $-\infty$, rather than the cost of a finite shortest [directed walk](directed-walk.md). The distinction is about [reachability](reachability-in-a-graph.md), not simply the presence of a negative [edge](edge-of-a-graph.md) or a negative-cost [directed cycle](directed-cycle.md) anywhere in the [graph](graph-split.md).

Add $C\to A$ of weight $-4$ to the worked example. Now $A\to B\to C\to A$ has total weight $-2+3-4=-3$. Add also an isolated [vertex](vertex-graph-theory.md) $U$ with a [self-loop](loop-graph-theory.md) of weight $-1$. From $S$, the distances of $A,B,C,T$ are $-\infty$, because all four are reachable from the first negative-cost [directed cycle](directed-cycle.md). The source retains distance $0$: no [directed edge](directed-edge.md) leads back to $S$. The unreachable $U$ retains distance $\infty$, despite its negative-cost [self-loop](loop-graph-theory.md).

<a id="image-relevant-negative-cost-directed-cycles-descendants-from-a-source-become-ancestors-when-every-directed-edge-is-reversed"></a>
![](bellman-ford-negative-cycle-reachability.png)

**[Figure 4](#image-relevant-negative-cost-directed-cycles-descendants-from-a-source-become-ancestors-when-every-directed-edge-is-reversed). Relevant negative-cost directed cycles: descendants from a source become ancestors when every directed edge is reversed**.

For example, $m$ extra laps before proceeding to $T$ give costs $7-3m$. This construction also shows why requiring a [directed path](directed-path.md) with no repeated [vertices](vertex-graph-theory.md) would change the problem: only [directed walks](directed-walk.md) permit arbitrarily many laps. Merely finding one reachable negative-cost [directed cycle](directed-cycle.md) does not justify setting every reachable label to $-\infty$; $S$ in the figure is a counterexample.

To detect and classify, perform $|V|-1$ full passes without clamping any label, then test all [directed edges](directed-edge.md) against a fixed copy of the resulting labels. Collect heads $v$ of [edges](edge-of-a-graph.md) $u\to v$ satisfying $d(u)<\infty$ and $d(u)+w_{uv}<d(v)$. An empty collection certifies that no negative-cost [directed cycle](directed-cycle.md) is reachable from $s$. Otherwise run [graph search](graph-search.md) forwards from all collected [vertices](vertex-graph-theory.md): precisely the reached [vertices](vertex-graph-theory.md) have distance $-\infty$. A [vertex](vertex-graph-theory.md) unreachable from $s$ still has distance $\infty$; each remaining [vertex](vertex-graph-theory.md) has its finite shortest distance.

Why is this classification exact? Every unaffected reachable [vertex](vertex-graph-theory.md) already has its shortest distance after $|V|-1$ passes, since any route ending there avoids reachable negative-cost [directed cycles](directed-cycle.md). Thus it cannot be the head of a strict improvement, or be reached from such a head. Conversely, all [vertices](vertex-graph-theory.md) on a reachable negative-cost [directed cycle](directed-cycle.md) have finite labels by that time. If none of its [edges](edge-of-a-graph.md) could improve a label, summing $d(v)\le d(u)+w_{uv}$ around it would imply $0\le\sum w_{uv}<0$. At least one of its heads is therefore collected, and the forward [graph search](graph-search.md) reaches the entire [directed cycle](directed-cycle.md) and every affected descendant. Detecting a [directed cycle](directed-cycle.md) alone and marking its descendants are separate tasks; finite intermediate labels in the affected region are not answers.

## ↑ Ancestors (7)

1. [Bellman-Ford algorithm](bellman-ford-algorithm.md)
2. [Shortest path problem](shortest-path-problem-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
