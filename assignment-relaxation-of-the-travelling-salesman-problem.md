# Assignment relaxation of the travelling salesman problem

↑ **Parent:** [Travelling salesman problem](travelling-salesman-problem.md)

Minimizing $\sum_{ij}c_{ij}x_{ij}$ over binary variables with one outgoing and one incoming edge at every [graph vertex](vertex-graph-theory.md), and $x_{ii}=0$, is an [assignment problem](assignment-problem.md). Its feasible solutions are [cycle covers of a directed graph](cycle-cover-of-a-directed-graph.md), whereas a [travelling salesman problem](travelling-salesman-problem.md) requires one [Hamiltonian cycle](hamilton-cycle.md). The relaxed minimum is therefore a [lower bound](lower-bound-in-a-partially-ordered-set.md) on the tour cost. If its optimum contains a proper subtour $C$, every tour omits at least one edge of $C$. Branching into subproblems that respectively forbid each edge of $C$ preserves every possible tour. Solving each child [assignment problem](assignment-problem.md) and pruning those whose bounds exceed the best tour yields a finite [branch and bound](branch-and-bound.md) algorithm. Equality also permits pruning when only one optimum is wanted.

## ↑ Ancestors (5)

1. [Travelling salesman problem](travelling-salesman-problem.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-37/3/solution.md)
