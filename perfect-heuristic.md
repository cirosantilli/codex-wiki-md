# Perfect heuristic

↑ **Parent:** [Heuristic function](heuristic-function.md)

The exact minimum remaining [path cost](path-cost.md) from a state to a [goal state](goal-state.md), with value $\infty$ when no goal is reachable. For nonnegative step costs, $h^*(g)=0$ at goals and $h^*(s)\le c(s,s')+h^*(s')$ on every transition. Thus a [perfect heuristic](perfect-heuristic.md) is a [consistent heuristic](consistent-heuristic.md) and an [admissible heuristic](admissible-heuristic.md). It measures remaining cost; a [greedy best-first search](greedy-best-first-search.md) decision using only this number can still take an excessively costly incoming [edge](edge-of-a-graph.md).

## ↑ Ancestors (7)

1. [Heuristic function](heuristic-function.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Greedy perfect-heuristic descent](greedy-perfect-heuristic-descent.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/1/b/solution.md)
- [Perfect heuristic](perfect-heuristic.md)
