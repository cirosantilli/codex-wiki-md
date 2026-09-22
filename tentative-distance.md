# Tentative distance

↑ **Parent:** [Dijkstra algorithm](dijkstra-algorithm.md)

A tentative distance $d(v)$ is the cheapest cost so far recorded by a [shortest path problem](shortest-path-problem-split.md) [algorithm](algorithm-split.md). For the single-source convention, initialize $d(s)=0$ and $d(v)=\infty$ elsewhere. Every finite label is the cost of a discovered route from $s$ to $v$, so

$$
\delta(s,v)\le d(v).
$$

It is an [upper bound](upper-bound-in-a-partially-ordered-set.md) supplied by an actual route, not a guess that might be too low. The [loop invariant](loop-invariant.md) follows directly from [edge relaxation](edge-relaxation.md): extending a discovered route to $u$ by $u\to v$ supplies another discovered route. The usual label initialization and this safety property are stated and proved in the authored MIT notes.[MIT 6.006, Lecture 16, p. 1: relaxation safety](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/6277a1f06100c26a7ff21031af6757b5_MIT6_006F11_lec16.pdf)

In the trace under [edge relaxation](edge-relaxation.md), $d(t)=10$ first records the direct [directed path](directed-path.md) $s\to t$. Later $d(t)=8$ records $s\to a\to t$, and finally $d(t)=3$ records $s\to b\to a\to t$. Each label is a usable route cost, but the first two are not shortest. An infinite [tentative distance](tentative-distance.md) means no route has yet been discovered; only a completed search establishes unreachability. The isolated [vertex](vertex-graph-theory.md) $z$ in that example remains at $\infty$.

In a [directed graph](directed-graph.md), the discovered route is formally a [directed walk](directed-walk.md), which may repeat [vertices](vertex-graph-theory.md); in the pictured acyclic [graph](graph-split.md) it is always a [directed path](directed-path.md). Negative-cost [directed cycles](directed-cycle.md) can keep supplying cheaper [directed walks](directed-walk.md) without a finite optimum. In the all-to-one convention, the same meaning applies to discovered routes _from_ $i$ _to_ $r$. Do not confuse either version with the [lower bounds](lower-bound-in-a-partially-ordered-set.md) supplied by feasible potentials in the [Bellman inequalities](bellman-inequalities.md): one records something achievable, the other rules out anything cheaper.

## ↑ Ancestors (7)

1. [Dijkstra algorithm](dijkstra-algorithm.md)
2. [Shortest path problem](shortest-path-problem-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Bellman-Ford algorithm](bellman-ford-algorithm.md)
- [Binary heap](binary-heap.md)
- [Dijkstra algorithm](dijkstra-algorithm.md)
- [Edge relaxation](edge-relaxation.md)
- [Tentative distance](tentative-distance.md)
