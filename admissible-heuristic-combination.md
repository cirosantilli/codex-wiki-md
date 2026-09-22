# Admissible heuristic combination

↑ **Parent:** [Admissible heuristic](admissible-heuristic.md)

If $h_1,h_2\le h^*$, their pointwise minimum, pointwise maximum and each [convex combination](convex-combination.md) $\alpha h_1+(1-\alpha)h_2$ with $0\le\alpha\le1$ are [admissible heuristics](admissible-heuristic.md). Each inequality follows directly by comparison with $h^*$. The maximum has [heuristic dominance](heuristic-dominance.md) over the minimum and every such [convex combination](convex-combination.md).

A sum need not be an [admissible heuristic](admissible-heuristic.md): two exact estimates of the same cost-one remaining action sum to two. A sufficient condition for a valid additive construction is separate nonnegative action-cost allocations $c_1,c_2$ with $c_1+c_2\le c$, and estimates bounded by the corresponding optimal allocated costs. Every goal-reaching [graph path](path-in-a-graph.md) then costs at least $h_1+h_2$ under its original costs. Taking the minimum proves admissibility without counting the same work twice.

If $h_1,h_2$ are [consistent heuristics](consistent-heuristic.md), their maximum, minimum and fixed [convex combinations](convex-combination.md) are also [consistent heuristics](consistent-heuristic.md). For the maximum, choose an index attaining it at the source and bound its successor by the successor maximum. For the minimum, choose an index attaining it at the successor and bound the source minimum by that component. For a [convex combination](convex-combination.md), multiply the two consistency inequalities by their nonnegative weights and add them. All these combinations vanish at goals when the inputs do.

## ↑ Ancestors (7)

1. [Admissible heuristic](admissible-heuristic.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/2/d/solution.md)
