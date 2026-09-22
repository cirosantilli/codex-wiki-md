# Leaf elimination of a tree-pattern positive-definite matrix

↑ **Parent:** [Sparse Gaussian elimination](sparse-gaussian-elimination.md)

Associate an undirected graph with a symmetric matrix's off-diagonal nonzero pattern. Eliminating vertex $i$ updates the remaining matrix by $a_{jk}\mapsto a_{jk}-a_{ji}a_{ik}/a_{ii}$. Only pairs of neighbors of $i$ can acquire [fill-in](fill-in.md). If the graph is a tree, remove leaves successively: each eliminated vertex has at most one remaining neighbor, so only a diagonal entry can change. Every [Schur complement](schur-complement.md) of a [positive-definite matrix](positive-definite-matrix.md) is positive definite, so no zero pivot forces a different ordering. Leaf removal therefore constructs a [perfect elimination ordering](perfect-elimination-ordering.md) and a fill-free factorization.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/4/solution.md)
