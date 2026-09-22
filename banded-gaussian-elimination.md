# Banded Gaussian elimination

↑ **Parent:** [Gaussian elimination](gaussian-elimination.md)

For a [band matrix](band-matrix.md), elimination without pivoting retains bounded lower and upper bandwidths in its triangular factors. A tridiagonal system therefore needs only linear work and storage, as in the [Thomas algorithm](tridiagonal-matrix-algorithm.md). Pivoting can change the precise fill pattern and must be included in the bandwidth and cost analysis when required. The inverse need not be banded, so solving through the factors preserves sparsity that explicit inversion would lose.

## ↑ Ancestors (7)

1. [Gaussian elimination](gaussian-elimination.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Band matrix](band-matrix.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford/2008/2/a/solution.md)
