# Nested dissection

↑ **Parent:** [Sparse Gaussian elimination](sparse-gaussian-elimination.md)

A [vertex separator](vertex-separator.md) divides the remaining unknowns into disconnected subdomains. Nested dissection recursively eliminates each subdomain before its separator, keeping interaction localized until late in the factorization. For a regular two-dimensional mesh with $N$ unknowns, separators have size $O(\sqrt N)$; the resulting direct factorization uses $O(N^{3/2})$ work and $O(N\log N)$ storage under the usual geometric separator assumptions.

## ↑ Ancestors (8)

1. [Sparse Gaussian elimination](sparse-gaussian-elimination.md)
2. [Gaussian elimination](gaussian-elimination.md)
3. [Numerical linear algebra](numerical-linear-algebra.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/6/solution.md)
