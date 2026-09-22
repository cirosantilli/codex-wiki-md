# Maximum feasible subsystem

↑ **Parent:** [Linear programming](linear-programming.md)

Given finitely encoded linear inequalities, a [maximum feasible subsystem](maximum-feasible-subsystem.md) is a largest collection that can be simultaneously satisfied. Its decision version asks whether some $k$ inequalities admit a common solution. This is [NP-complete](np-completeness.md), despite [polynomial time](polynomial-time.md) feasibility testing for each fixed collection. For a graph, use nonnegative variables $x_v$, constraints $x_v\geq1$ for vertices, and $M>|V|$ copies of $x_u+x_v\leq1$ for each edge. A subsystem of size $M|E|+k$ must retain a copy of every edge constraint and at least $k$ vertex constraints; those vertices form an [independent set](independent-set-graph-theory.md). Conversely an [independent set](independent-set-graph-theory.md) of size $k$ supplies such a feasible subsystem by its indicator vector.

## ↑ Ancestors (5)

1. [Linear programming](linear-programming.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Maximum feasible subsystem](maximum-feasible-subsystem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-35/1/solution.md)
