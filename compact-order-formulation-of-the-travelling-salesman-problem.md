# Compact order formulation of the travelling salesman problem

↑ **Parent:** [Travelling salesman problem](travelling-salesman-problem.md)

Use binary directed-edge variables $x_{ij}$, one incoming and one outgoing edge at each city, and integer order variables $1\leq u_i\leq n-1$ for cities other than a distinguished city. The constraints $u_i-u_j+(n-1)x_{ij}\leq n-2$ for distinct nondistinguished cities force order increase along every selected edge away from the distinguished city. Summing around any cycle avoiding that city gives a contradiction, so the degree equations describe a single tour. There are $O(n^2)$ nonzero constraint entries apart from the degree equations, also totaling $O(n^2)$ entries. With costs at most $2^n$, the objective requires $O(n^3)$ bits and the remaining sparse constraint encoding $O(n^2\log n)$ bits. Omitting zero matrix entries is essential for this particular size bound.

## ↑ Ancestors (5)

1. [Travelling salesman problem](travelling-salesman-problem.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-40/2/solution.md)
