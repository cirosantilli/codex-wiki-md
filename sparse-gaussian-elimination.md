# Sparse Gaussian elimination

↑ **Parent:** [Gaussian elimination](gaussian-elimination.md)

A sparse direct solver performs [Gaussian elimination](gaussian-elimination.md) while storing and updating only the predicted nonzero entries. A symbolic phase predicts the factor pattern from an elimination ordering, and a numerical phase evaluates the factors. The ordering can greatly alter [fill-in](fill-in.md) and arithmetic work. For symmetric positive-definite systems, [Cholesky decomposition](cholesky-decomposition.md) avoids numerical pivoting; general systems require a balance between sparsity and stable pivot selection.

**Table of contents**

- [Leaf elimination of a tree-pattern positive-definite matrix](leaf-elimination-of-a-tree-pattern-positive-definite-matrix.md)
- [Symbolic factorization](symbolic-factorization.md)
- [Elimination tree](elimination-tree.md)
- [Nested dissection](nested-dissection.md)
- [Minimum degree algorithm](minimum-degree-algorithm.md)
- [Fill-in](fill-in.md)
- [Matrix graph](matrix-graph.md)
  - [Elimination graph](elimination-graph.md)
    - [Fill-path criterion for symmetric elimination](fill-path-criterion-for-symmetric-elimination.md)

## ↑ Ancestors (7)

1. [Gaussian elimination](gaussian-elimination.md)
2. [Numerical linear algebra](numerical-linear-algebra.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/6/solution.md)
