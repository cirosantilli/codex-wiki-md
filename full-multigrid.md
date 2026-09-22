# Full multigrid

↑ **Parent:** [Multigrid method](multigrid-method.md)

Full multigrid solves first on a coarse mesh, interpolates that approximation to the next finer mesh, and applies a fixed number of [geometric multigrid V-cycles](geometric-multigrid-v-cycle.md) before proceeding to the next level. If interpolation introduces only the expected discretization-scale error and the cycle count reduces the inherited error sufficiently at every level, the final algebraic error matches the fine-grid discretization error. The geometric sum of level costs is then $O(N)$, unlike reducing an arbitrary fine-grid initial error by an arbitrarily small tolerance.

## ↑ Ancestors (6)

1. [Multigrid method](multigrid-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/7/solution.md)
