# Geometric multigrid V-cycle

↑ **Parent:** [Multigrid method](multigrid-method.md)

A geometric multigrid V-cycle pre-smooths an approximate solution, restricts its residual, recursively solves the coarse error equation once from zero, prolongs and adds that error correction, and post-smooths. The recursion ends in a direct solve on a small coarsest grid. With fixed sweep counts and bounded stencil work, coarsening in $d$ dimensions gives total work $O(N)\sum_{j\geq0}2^{-dj}=O(N)$ per cycle. A mesh-independent convergence factor also requires compatible coarse approximation and effective smoothing; linear work alone does not prove convergence.

## ↑ Ancestors (6)

1. [Multigrid method](multigrid-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Full multigrid](full-multigrid.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/7/solution.md)
