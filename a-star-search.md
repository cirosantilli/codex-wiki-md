# A-star search

↑ **Parent:** [Best-first search](best-first-search.md)

[Best-first search](best-first-search.md) prioritizing the estimated total solution cost $f=g+h$, with $g$ the cost already incurred and $h$ a [heuristic function](heuristic-function.md) for the remaining cost. With nonnegative estimates, goal estimates zero, finite [branching factor](branching-factor.md) and step costs bounded below by a positive constant, the [tree search](tree-search.md) version using an [admissible heuristic](admissible-heuristic.md) returns a minimum-cost goal when it removes one for expansion. An optimal solution path always has a frontier node with $f\le C^*$; a more costly goal cannot be removed before it. The stated finiteness and lower-cost assumptions ensure finitely many earlier nodes when a finite solution exists. Repeated-state handling in [graph search](graph-search.md) needs reopening when a better path is found, unless a [consistent heuristic](consistent-heuristic.md) justifies finalizing expanded states.

**Table of contents**

- [Numerical upper-bound pruning without a solution witness](numerical-upper-bound-pruning-without-a-solution-witness.md)

## ↑ Ancestors (8)

1. [Best-first search](best-first-search.md)
2. [Graph search](graph-search.md)
3. [Graph](graph-split.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Goal state](goal-state.md)
- [Heuristic dominance](heuristic-dominance.md)
- [Informed search and exploration by Stuart Russell and Peter Norvig](informed-search-and-exploration-by-stuart-russell-and-peter-norvig.md)
- [Numerical upper-bound pruning without a solution witness](numerical-upper-bound-pruning-without-a-solution-witness.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/intelligent-systems/1/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/intelligent-systems/1/c/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/intelligent-systems/1/f/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/artificial-intelligence/1/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/1/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/1/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/artificial-intelligence/1/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/artificial-intelligence/1/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/artificial-intelligence/1/c/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/artificial-intelligence/1/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/2/e/solution.md)
- [Path cost](path-cost.md)
- [Search frontier](search-frontier.md)
- [Uniform-cost search](uniform-cost-search.md)
