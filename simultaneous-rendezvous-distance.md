# Simultaneous rendezvous distance

↑ **Parent:** [Search problem](search-problem.md)

Two controlled walkers on the same connected [undirected graph](undirected-graph.md) can each traverse one [edge](edge-of-a-graph.md) or wait in each unit-cost step. If they meet only by occupying the same [vertex](vertex-graph-theory.md) at the same time, their minimum meeting time is

$$
\left\lceil\frac{d(p,q)}2\right\rceil,
$$

where $d$ is the [shortest path](shortest-path.md) distance. A common meeting point after $t$ steps implies $d(p,q)\le2t$ by the [triangle inequality](triangle-inequality.md). Conversely, choose a middle [vertex](vertex-graph-theory.md) of a shortest connecting [graph path](path-in-a-graph.md); both walkers reach it within $\lceil d/2\rceil$ steps, and the earlier arrival waits. The wait is essential when the path length is an [odd integer](odd-integer.md). This distance on the joint [Cartesian product](cartesian-product.md) [state space](state-space.md) is a [consistent heuristic](consistent-heuristic.md): each joint move changes the walkers’ separation by at most two. Replacing $d$ by an obstacle-free [Manhattan distance](manhattan-distance.md) preserves [admissible heuristic](admissible-heuristic.md) and [consistent heuristic](consistent-heuristic.md) guarantees.

## ↑ Ancestors (6)

1. [Search problem](search-problem.md)
2. [Computational problem](computational-problem.md)
3. [Computational complexity theory](computational-complexity-theory.md)
4. [Theoretical computer science](theoretical-computer-science-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/2/c/solution.md)
