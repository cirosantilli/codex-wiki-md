# Greedy perfect-heuristic descent

↑ **Parent:** [Greedy best-first search](greedy-best-first-search.md)

In a finite reachable [search problem](search-problem.md) with strictly positive step costs and a reachable goal, [greedy best-first search](greedy-best-first-search.md) using a [perfect heuristic](perfect-heuristic.md) selects one parent–child chain until it reaches a [goal state](goal-state.md). At a selected nonterminal state $s$, an optimal first transition has $h^*(s')=h^*(s)-c(s,s')<h^*(s)$. Every older [search frontier](search-frontier.md) entry has estimate at least $h^*(s)$, so the next selected entry must be a newly generated child with smaller estimate. Repeating proves the chain property. In an infinite finitely branching problem, a positive uniform lower bound on costs also bounds the chain length by the initial remaining cost divided by that lower bound. Zero-cost ties can break the chain property; the lemma does not establish least accumulated [path cost](path-cost.md).

## ↑ Ancestors (9)

1. [Greedy best-first search](greedy-best-first-search.md)
2. [Best-first search](best-first-search.md)
3. [Graph search](graph-search.md)
4. [Graph](graph-split.md)
5. [Graph theory](graph-theory-split.md)
6. [Foundations of mathematics](foundations-of-mathematics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/1/b/solution.md)
