# Shortest-path pursuit distance bound

↑ **Parent:** [Shortest path problem](shortest-path-problem-split.md)

Suppose two pieces occupy a common [connected component of a graph](component-graph-theory.md) in an unweighted [undirected graph](undirected-graph.md). For [integers](integer-split.md) $a>b\ge0$, in each round an evader moves at most $b$ [edges](edge-of-a-graph.md), then a pursuer moves up to $a$ [edges](edge-of-a-graph.md) along a [shortest path](shortest-path.md) to the new evader position, stopping upon capture. Let $d_t$ be their finite [graph distance](distance-graph-theory.md) at a surviving round boundary.

The [triangle inequality](triangle-inequality.md) bounds the separation after the evader moves by $d_t+b$. If that separation is at most $a$, the pursuer captures it. Otherwise the pursuer reduces it by exactly $a$, giving

$$
1\le d_{t+1}\le d_t-(a-b).
$$

Hence every surviving history has at most $\lfloor(d_0-1)/(a-b)\rfloor$ rounds. With a finite [branching factor](branching-factor.md), the surviving [search tree](search-tree.md) is finite and [depth-first tree search](depth-first-tree-search.md) becomes a [complete search algorithm](complete-search-algorithm.md). This does not make its first goal optimal for arbitrary rewards. Initial [reachability](reachability-in-a-graph.md) is essential: an infinite [graph distance](distance-graph-theory.md) supplies no decreasing finite bound.

## ↑ Ancestors (6)

1. [Shortest path problem](shortest-path-problem-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/artificial-intelligence/1/h/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/artificial-intelligence/1/i/solution.md)
