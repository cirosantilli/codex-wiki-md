# Dijkstra algorithm

↑ **Parent:** [Shortest path problem](shortest-path-problem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dijkstra's_algorithm)

The [Dijkstra algorithm](dijkstra-algorithm.md) solves the single-source [shortest path problem](shortest-path-problem.md) in a finite [graph](graph-split.md) with nonnegative [edge](edge-of-a-graph.md) weights, finding distances to all reachable [vertices](vertex-graph-theory.md). Start with [tentative distance](tentative-distance.md) $d(A)=0$ and $d(v)=\infty$ elsewhere. Repeatedly choose the unfinalized [vertex](vertex-graph-theory.md) with least [tentative distance](tentative-distance.md), declare that label permanent, and perform [edge relaxation](edge-relaxation.md) on its outgoing [edges](edge-of-a-graph.md). For an [undirected graph](undirected-graph.md), inspect both directions. A finite [tentative distance](tentative-distance.md) always records the cost of a discovered [graph path](path-in-a-graph.md), but can improve before finalization.

In our example, finalizing $A$ discovers $C$ at $1$, $B$ at $4$, and $D$ at $10$. Choose $C$ next: [edge relaxation](edge-relaxation.md) through $C$ lowers $B$ to $1+2=3$ and $D$ to $1+5=6$. Choose $B$: [edge relaxation](edge-relaxation.md) through $B$ lowers $D$ to $3+1=4$. Finally choose $D$. The permanent distances are therefore $A:0$, $C:1$, $B:3$, $D:4$; the evolving [tentative distances](tentative-distance.md) were $B:4\to3$ and $D:10\to6\to4$.

<a id="image-tentative-distances-fall-until-the-dijkstra-algorithm-makes-each-label-permanent"></a>
![](dijkstra-distance-frontier.png)

**[Figure 5](#image-tentative-distances-fall-until-the-dijkstra-algorithm-makes-each-label-permanent). Tentative distances fall until the Dijkstra algorithm makes each label permanent**.

Store a [shortest-path predecessor](shortest-path-predecessor.md) whenever [edge relaxation](edge-relaxation.md) improves a label. The final table contains enough information to reconstruct routes, rather than merely their costs:

| [Vertex](vertex-graph-theory.md) | Distance from $A$ | [Shortest-path predecessor](shortest-path-predecessor.md) | Finalization order |
| --- | --- | --- | --- |
| $A$ | $0$ | None: source | $1$ |
| $C$ | $1$ | $A$ | $2$ |
| $B$ | $3$ | $C$ | $3$ |
| $D$ | $4$ | $B$ | $4$ |

Following [shortest-path predecessors](shortest-path-predecessor.md) backwards gives $D,B,C,A$; reversing the order gives $A,C,B,D$. If only this destination matters, stop when $D$ is finalized. Stopping when $D$ is first discovered would incorrectly return $10$. If the smallest remaining [tentative distance](tentative-distance.md) is $\infty$, all remaining [vertices](vertex-graph-theory.md) are unreachable.

Why is the permanent choice safe? Suppose the selected [vertex](vertex-graph-theory.md) $u$ had a cheaper [graph path](path-in-a-graph.md). Let $y$ be the first unfinalized [vertex](vertex-graph-theory.md) on that [graph path](path-in-a-graph.md). Its preceding [vertex](vertex-graph-theory.md) was finalized, so [edge relaxation](edge-relaxation.md) has already offered $y$ a label no larger than that prefix's cost. Nonnegative remaining [edge](edge-of-a-graph.md) weights make the whole cost at least this prefix's cost; selection gives $d(u)\le d(y)$. A cheaper [graph path](path-in-a-graph.md) would contradict these comparisons. Zero weights are allowed; ties can be resolved arbitrarily. This is the reason the [label-setting shortest-path algorithm](label-setting-shortest-path-algorithm.md) works, rather than a lucky feature of the drawing.

Negative weights break that reasoning. In a [directed graph](directed-graph.md) with $s\to u$ costing $2$, $s\to v$ costing $5$, and $v\to u$ costing $-4$, the [Dijkstra algorithm](dijkstra-algorithm.md) would finalize $u$ at $2$ before discovering the cheaper cost $1$. The [Bellman-Ford algorithm](bellman-ford-algorithm.md) handles negative [edge](edge-of-a-graph.md) weights when no relevant negative [directed cycle](directed-cycle.md) exists.

With an [adjacency list](adjacency-list.md) and an indexed [binary heap](binary-heap.md) implementing a [priority queue](priority-queue.md), the [time complexity](time-complexity.md) is $O((|V|+|E|)\log |V|)$ for $|V|\ge2$, using [Big O notation](big-o-notation.md). Each [vertex](vertex-graph-theory.md) is extracted at most once, each [edge](edge-of-a-graph.md) is inspected once per direction, and each successful [edge relaxation](edge-relaxation.md) decreases a heap key in $O(\log |V|)$ time. This assumes constant-cost arithmetic and comparisons; exact computation with very large weights adds their representation cost. The queue uses $O(|V|)$ space beyond the [graph](graph-split.md). Simply scanning all remaining [vertices](vertex-graph-theory.md) gives $O(|V|^2+|E|)$ instead.[Princeton, DijkstraSP implementation](https://algs4.cs.princeton.edu/44sp/DijkstraSP.java.html)[Princeton, indexed binary heap operations](https://algs4.cs.princeton.edu/code/javadoc/edu/princeton/cs/algs4/IndexMinPQ.html)

The 1959 paper presents the [shortest path problem](shortest-path-problem.md) as its second problem, after the [minimum spanning tree](minimum-spanning-tree.md) problem, and grows known shortest routes in increasing distance order.[Dijkstra, A note on two problems in connexion with graphs, pp. 269–271](https://www.cs.yale.edu/homes/lans/readings/routing/dijkstra-routing-1959.pdf) In his later recollection, Dijkstra dated the shortest-route discovery to 1956: a demonstration for the ARMAC computer used a simplified Dutch railway map and printed the route between towns. A practical request became an enduring [algorithm](algorithm.md) because the same distance rule applies to any suitable [graph](graph-split.md).[Dijkstra's recollection, published in 1983](https://garfield.library.upenn.edu/classics1983/A1983QA19900001.pdf)

**Table of contents**

- [Tentative distance](tentative-distance.md)
- [Edge relaxation](edge-relaxation.md)
- [Shortest-path predecessor](shortest-path-predecessor.md)

## ↑ Ancestors (6)

1. [Shortest path problem](shortest-path-problem.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Binary heap](binary-heap.md)
- [Breadth-first search](breadth-first-search.md)
- [Dijkstra algorithm](dijkstra-algorithm.md)
- [Edge relaxation](edge-relaxation.md)
- [Graph theory](graph-theory-split.md)
- [Label-setting shortest-path algorithm](label-setting-shortest-path-algorithm.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-31/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-35/2/solution.md)
- [Shortest-path predecessor](shortest-path-predecessor.md)
- [Shortest path problem](shortest-path-problem.md)
