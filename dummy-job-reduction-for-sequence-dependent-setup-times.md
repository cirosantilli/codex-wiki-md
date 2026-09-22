# Dummy-job reduction for sequence-dependent setup times

↑ **Parent:** [Travelling salesman problem](travelling-salesman-problem.md)

Add a dummy job $0$. Give the arc $0\to i$ cost equal to job $i$'s initial setup, the arc $i\to j$ its changeover cost, and every arc $i\to0$ zero cost. A [Hamiltonian cycle](hamilton-cycle.md) through the dummy represents a schedule, starting just after $0$ and ending just before it. The total processing time is constant on a single machine, so minimizing cycle cost minimizes completion time. Dropping [subtour elimination constraints](subtour-elimination-constraints.md) gives an [assignment problem](assignment-problem.md) lower bound.

## ↑ Ancestors (5)

1. [Travelling salesman problem](travelling-salesman-problem.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/5/solution.md)
