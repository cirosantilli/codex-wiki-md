# Hill climbing

↑ **Parent:** [Local search](local-search.md)

A [local search](local-search.md) method that retains one current candidate and repeatedly chooses an improving neighbor of its objective. For a conflict-minimization [constraint satisfaction problem](constraint-satisfaction-problem.md), a candidate can assign all variables within their [constraint domains](constraint-domain.md) while violating some inter-variable constraints; the objective counts those violations. Zero conflicts certifies a solution, while a positive-conflict [local minimum](local-minimum.md) need not certify impossibility. Plateaus and local minima motivate sideways moves, randomized choices and restarting. Prescribed variables must remain fixed in every initialization and move.

**Table of contents**

- [Min-conflicts algorithm](min-conflicts-algorithm.md)

## ↑ Ancestors (6)

1. [Local search](local-search.md)
2. [Heuristic optimization](heuristic-optimization.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/artificial-intelligence/1/f/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/3/f/solution.md)
- [Queens completion problem](queens-completion-problem.md)
